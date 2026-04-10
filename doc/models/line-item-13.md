
# Line Item 13

*This model accepts additional fields of type Object.*

## Structure

`LineItem13`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Description` | `String` | Optional | Description of the item.<br><br>**Constraints**: *Maximum Length*: `26` | String getDescription() | setDescription(String description) |
| `CommodityCode` | `String` | Optional | An international description code of the individual good or service being supplied.<br><br>**Constraints**: *Maximum Length*: `12` | String getCommodityCode() | setCommodityCode(String commodityCode) |
| `DiscountAmount` | `Integer` | Optional | Total discount amount applied against the line item total ,Can accept Two (2) decimal places.<br><br>**Constraints**: `<= 99999999999900` | Integer getDiscountAmount() | setDiscountAmount(Integer discountAmount) |
| `OtherTaxAmount` | `Integer` | Optional | Used if city or multiple county taxes need to be broken out separately ,Can accept Two (2) decimal places.<br><br>**Constraints**: `<= 99999999999900` | Integer getOtherTaxAmount() | setOtherTaxAmount(Integer otherTaxAmount) |
| `ProductCode` | `String` | Optional | Merchant-defined description code of the item.<br><br>**Constraints**: *Maximum Length*: `12` | String getProductCode() | setProductCode(String productCode) |
| `Quantity` | `Integer` | Optional | Quantity of the item, can accept Four (4) decimal places.<br><br>**Constraints**: `<= 99999` | Integer getQuantity() | setQuantity(Integer quantity) |
| `TaxAmount` | `Integer` | Optional | Amount of any value added taxes, can accept Two (2) decimal places.<br><br>**Constraints**: `>= 0`, `<= 99999999999` | Integer getTaxAmount() | setTaxAmount(Integer taxAmount) |
| `TaxRate` | `Integer` | Optional | Tax rate used to calculate the sales tax amount, can accept 2 decimal places.<br><br>**Constraints**: `<= 999999` | Integer getTaxRate() | setTaxRate(Integer taxRate) |
| `UnitCode` | `String` | Optional | Units of measurement as used in international trade. (See Codes for Units of Measurement below for unit code abbreviations)<br><br>**Constraints**: *Minimum Length*: `3`, *Maximum Length*: `3` | String getUnitCode() | setUnitCode(String unitCode) |
| `UnitCost` | `Integer` | Optional | Unit cost of the item ,Can accept Four (4) decimal places.<br><br>**Constraints**: `<= 99999999999900` | Integer getUnitCost() | setUnitCost(Integer unitCost) |
| `AlternateTaxId` | `String` | Optional | Tax identification number of the merchant that reported the alternate tax amount.<br><br>**Constraints**: *Maximum Length*: `15` | String getAlternateTaxId() | setAlternateTaxId(String alternateTaxId) |
| `DebitCredit` | `Object` | Optional | - | Object getDebitCredit() | setDebitCredit(Object debitCredit) |
| `DiscountRate` | `Integer` | Optional | Discount rate for the line item ,Can accept Two (2) decimal places.<br><br>**Constraints**: `<= 9999999` | Integer getDiscountRate() | setDiscountRate(Integer discountRate) |
| `TaxTypeApplied` | `String` | Optional | Type of value-added taxes that are being used (Conditional If tax amount is supplied)<br><br>> This field is only required when Merchant is directed to include by Mastercard.<br><br>**Constraints**: *Maximum Length*: `4` | String getTaxTypeApplied() | setTaxTypeApplied(String taxTypeApplied) |
| `TaxTypeId` | `String` | Optional | Indicates the type of tax collected in relationship to a specific tax amount (Conditional If tax amount is supplied)<br><br>**Constraints**: *Minimum Length*: `2`, *Maximum Length*: `2` | String getTaxTypeId() | setTaxTypeId(String taxTypeId) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "description": "cool drink",
  "commodity_code": "cc123456",
  "discount_amount": 0,
  "other_tax_amount": 0,
  "product_code": "fanta123456",
  "quantity": 12,
  "tax_amount": 4,
  "tax_rate": 0,
  "unit_code": "gll",
  "unit_cost": 3,
  "alternate_tax_id": "1234",
  "discount_rate": 11,
  "tax_type_applied": "22",
  "tax_type_id": "11",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

