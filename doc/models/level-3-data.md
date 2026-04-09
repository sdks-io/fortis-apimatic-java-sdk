
# Level 3 Data

Level 3 data object

## Structure

`Level3Data`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `DestinationCountryCode` | `String` | Optional | Code of the country where the goods are being shipped.<br><br>**Constraints**: *Minimum Length*: `3`, *Maximum Length*: `3` | String getDestinationCountryCode() | setDestinationCountryCode(String destinationCountryCode) |
| `DutyAmount` | `Integer` | Optional | Fee amount associated with the import of the purchased goods ,Can accept Two (2) decimal places<br><br>**Constraints**: `>= 0`, `<= 99999999999900` | Integer getDutyAmount() | setDutyAmount(Integer dutyAmount) |
| `FreightAmount` | `Integer` | Optional | Freight or shipping portion of the total transaction amount ,Can accept Two (2) decimal places.<br><br>**Constraints**: `>= 0`, `<= 99999999999900` | Integer getFreightAmount() | setFreightAmount(Integer freightAmount) |
| `NationalTax` | `Integer` | Optional | National tax for the transaction ,Can accept Two (2) decimal places.<br><br>**Constraints**: `<= 999999999900` | Integer getNationalTax() | setNationalTax(Integer nationalTax) |
| `SalesTax` | `Integer` | Optional | Sales tax for the transaction ,Can accept Two (2) decimal places.<br><br>**Constraints**: `<= 999999999900` | Integer getSalesTax() | setSalesTax(Integer salesTax) |
| `ShipfromZipCode` | `String` | Optional | Postal/ZIP code of the address from where the purchased goods are being shipped.<br><br>**Constraints**: *Maximum Length*: `10` | String getShipfromZipCode() | setShipfromZipCode(String shipfromZipCode) |
| `ShiptoZipCode` | `String` | Optional | Postal/ZIP code of the address where purchased goods will be delivered.<br><br>**Constraints**: *Maximum Length*: `10` | String getShiptoZipCode() | setShiptoZipCode(String shiptoZipCode) |
| `TaxAmount` | `Integer` | Optional | Amount of any value added taxes ,Can accept Two (2) decimal places.<br><br>**Constraints**: `>= 0`, `<= 99999999999` | Integer getTaxAmount() | setTaxAmount(Integer taxAmount) |
| `TaxExempt` | [`TaxExemptEnum`](../../doc/models/tax-exempt-enum.md) | Optional | Sales Tax Exempt. Allowed values: “1”, “0”. | TaxExemptEnum getTaxExempt() | setTaxExempt(TaxExemptEnum taxExempt) |
| `CustomerVatRegistration` | `String` | Optional | Customer VAT Registration<br><br>**Constraints**: *Maximum Length*: `13` | String getCustomerVatRegistration() | setCustomerVatRegistration(String customerVatRegistration) |
| `MerchantVatRegistration` | `String` | Optional | Merchant VAT Registration<br><br>**Constraints**: *Maximum Length*: `20` | String getMerchantVatRegistration() | setMerchantVatRegistration(String merchantVatRegistration) |
| `OrderDate` | `String` | Optional | Order Date<br><br>**Constraints**: *Minimum Length*: `6`, *Maximum Length*: `6` | String getOrderDate() | setOrderDate(String orderDate) |
| `SummaryCommodityCode` | `String` | Optional | Summary Commodity Code<br><br>**Constraints**: *Maximum Length*: `4` | String getSummaryCommodityCode() | setSummaryCommodityCode(String summaryCommodityCode) |
| `TaxRate` | `Integer` | Optional | Tax rate used to calculate the sales tax amount, can accept 2 decimal places.<br><br>**Constraints**: `<= 999900` | Integer getTaxRate() | setTaxRate(Integer taxRate) |
| `UniqueVatRefNumber` | `String` | Optional | Unique VAT Reference Number<br><br>**Constraints**: *Maximum Length*: `15` | String getUniqueVatRefNumber() | setUniqueVatRefNumber(String uniqueVatRefNumber) |
| `LineItems` | [`List<LineItem13>`](../../doc/models/line-item-13.md) | Optional | Array of line items in transaction | List<LineItem13> getLineItems() | setLineItems(List<LineItem13> lineItems) |

## Example (as JSON)

```json
{
  "destination_country_code": "840",
  "duty_amount": 0,
  "freight_amount": 0,
  "national_tax": 2,
  "sales_tax": 200,
  "shipfrom_zip_code": "AZ1234",
  "shipto_zip_code": "FL1234",
  "tax_amount": 10,
  "tax_exempt": "0",
  "customer_vat_registration": "12345678",
  "merchant_vat_registration": "123456",
  "order_date": "171006",
  "summary_commodity_code": "C1K2",
  "tax_rate": 0,
  "unique_vat_ref_number": "vat1234"
}
```

