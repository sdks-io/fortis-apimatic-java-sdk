
# Line Item 19

*This model accepts additional fields of type Object.*

## Structure

`LineItem19`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AlternateTaxId` | `String` | Optional | Tax identification number of the merchant that reported the alternate tax amount.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `15` | String getAlternateTaxId() | setAlternateTaxId(String alternateTaxId) |
| `DebitCredit` | `Object` | Optional | - | Object getDebitCredit() | setDebitCredit(Object debitCredit) |
| `Description` | `String` | Required | Description of the item.<br><br>**Constraints**: *Maximum Length*: `26` | String getDescription() | setDescription(String description) |
| `DiscountAmount` | `Integer` | Optional | Total discount amount applied against the line item total ,Can accept Two (2) decimal places.<br><br>**Constraints**: `<= 99999999999900` | Integer getDiscountAmount() | setDiscountAmount(Integer discountAmount) |
| `DiscountRate` | `Integer` | Optional | Discount rate for the line item ,Can accept Two (2) decimal places.<br><br>**Constraints**: `<= 9999900` | Integer getDiscountRate() | setDiscountRate(Integer discountRate) |
| `ProductCode` | `String` | Required | Merchant-defined description code of the item.<br><br>**Constraints**: *Maximum Length*: `12` | String getProductCode() | setProductCode(String productCode) |
| `Quantity` | `Integer` | Optional | Quantity of the item, can accept Four (4) decimal places.<br><br>**Constraints**: `<= 99999` | Integer getQuantity() | setQuantity(Integer quantity) |
| `TaxAmount` | `Integer` | Optional | Amount of any value added taxes, can accept Two (2) decimal places.<br><br>**Constraints**: `>= 0`, `<= 99999999999` | Integer getTaxAmount() | setTaxAmount(Integer taxAmount) |
| `TaxRate` | `Integer` | Optional | Tax rate used to calculate the sales tax amount, can accept 2 decimal places.<br><br>**Constraints**: `<= 999900` | Integer getTaxRate() | setTaxRate(Integer taxRate) |
| `TaxTypeApplied` | `String` | Optional | Type of value-added taxes that are being used (Conditional If tax amount is supplied)<br><br>> This field is only required when Merchant is directed to include by Mastercard.<br><br>**Constraints**: *Maximum Length*: `4` | String getTaxTypeApplied() | setTaxTypeApplied(String taxTypeApplied) |
| `TaxTypeId` | `String` | Optional | Indicates the type of tax collected in relationship to a specific tax amount (Conditional If tax amount is supplied)<br><br>**Constraints**: *Maximum Length*: `2` | String getTaxTypeId() | setTaxTypeId(String taxTypeId) |
| `UnitCode` | `String` | Required | Units of measurement as used in international trade. (See Codes for Units of Measurement below for unit code abbreviations)<br><br>**Constraints**: *Maximum Length*: `3` | String getUnitCode() | setUnitCode(String unitCode) |
| `UnitCost` | `int` | Required | Unit cost of the item ,Can accept Four (4) decimal places.<br><br>**Constraints**: `<= 99999999999900` | int getUnitCost() | setUnitCost(int unitCost) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "alternate_tax_id": "1234",
  "description": "cool drink",
  "discount_amount": 10,
  "discount_rate": 11,
  "product_code": "coke12345678",
  "quantity": 5,
  "tax_amount": 3,
  "tax_rate": 0,
  "tax_type_applied": "22",
  "tax_type_id": "a1",
  "unit_code": "gll",
  "unit_cost": 10,
  "debit_credit": {
    "key1": "val1",
    "key2": "val2"
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

