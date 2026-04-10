
# Product Invoice 1

*This model accepts additional fields of type Object.*

## Structure

`ProductInvoice1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Title` | `String` | Optional | Title<br><br>**Constraints**: *Maximum Length*: `36` | String getTitle() | setTitle(String title) |
| `QuoteNumberFormat` | `String` | Optional | Quote Number Format<br><br>**Constraints**: *Maximum Length*: `36` | String getQuoteNumberFormat() | setQuoteNumberFormat(String quoteNumberFormat) |
| `QuoteNumberStart` | `Double` | Optional | Quote Number Start<br><br>**Constraints**: `>= 1`, `<= 999999999` | Double getQuoteNumberStart() | setQuoteNumberStart(Double quoteNumberStart) |
| `QuoteNumberIncrement` | `Double` | Optional | Quote Number Increment<br><br>**Constraints**: `>= 1`, `<= 999999999` | Double getQuoteNumberIncrement() | setQuoteNumberIncrement(Double quoteNumberIncrement) |
| `QuoteNumberCurrent` | `Double` | Optional | Quote Number Current | Double getQuoteNumberCurrent() | setQuoteNumberCurrent(Double quoteNumberCurrent) |
| `InvoiceNumberFormat` | `String` | Optional | Invoice Number Format<br><br>**Constraints**: *Maximum Length*: `36` | String getInvoiceNumberFormat() | setInvoiceNumberFormat(String invoiceNumberFormat) |
| `InvoiceNumberStart` | `Double` | Optional | Invoice Number Start<br><br>**Constraints**: `>= 1`, `<= 999999999` | Double getInvoiceNumberStart() | setInvoiceNumberStart(Double invoiceNumberStart) |
| `InvoiceNumberIncrement` | `Double` | Optional | Invoice Number Increment<br><br>**Constraints**: `>= 1`, `<= 999999999` | Double getInvoiceNumberIncrement() | setInvoiceNumberIncrement(Double invoiceNumberIncrement) |
| `InvoiceNumberCurrent` | `Double` | Optional | Invoice Number Current | Double getInvoiceNumberCurrent() | setInvoiceNumberCurrent(Double invoiceNumberCurrent) |
| `TaxRate` | `Double` | Optional | Tax Rate<br><br>**Constraints**: `>= 0`, `<= 99.99` | Double getTaxRate() | setTaxRate(Double taxRate) |
| `TaxFee` | `Integer` | Optional | Tax Fee<br><br>**Constraints**: `<= 999999999999` | Integer getTaxFee() | setTaxFee(Integer taxFee) |
| `MonthlyFee` | `Integer` | Optional | Monthly Fees<br><br>**Constraints**: `>= 0`, `<= 99999` | Integer getMonthlyFee() | setMonthlyFee(Integer monthlyFee) |
| `PerInvoiceFee` | `Integer` | Optional | Per Invoice Fee<br><br>**Constraints**: `>= 0`, `<= 99999` | Integer getPerInvoiceFee() | setPerInvoiceFee(Integer perInvoiceFee) |
| `PerQuoteFee` | `Integer` | Optional | Per Quote fee<br><br>**Constraints**: `>= 0`, `<= 99999` | Integer getPerQuoteFee() | setPerQuoteFee(Integer perQuoteFee) |
| `RequirePayInFull` | `Boolean` | Optional | Require Pay In Full | Boolean getRequirePayInFull() | setRequirePayInFull(Boolean requirePayInFull) |
| `Selectable` | `Double` | Optional | Selectable | Double getSelectable() | setSelectable(Double selectable) |
| `Reportable` | `Double` | Optional | Reportable | Double getReportable() | setReportable(Double reportable) |
| `PortfolioId` | `String` | Optional | Portfolio Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getPortfolioId() | setPortfolioId(String portfolioId) |
| `LocationId` | `String` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `Id` | `String` | Optional | Product Invoice Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `ModifiedUserId` | `String` | Optional | Last User ID that updated the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getModifiedUserId() | setModifiedUserId(String modifiedUserId) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "title": "Sample title",
  "quote_number_start": 1.0,
  "quote_number_increment": 1.0,
  "quote_number_current": 1.0,
  "invoice_number_start": 1,
  "invoice_number_increment": 1,
  "invoice_number_current": 1,
  "tax_rate": 0,
  "tax_fee": 0,
  "monthly_fee": 0,
  "per_invoice_fee": 0,
  "per_quote_fee": 0,
  "require_pay_in_full": true,
  "selectable": 1,
  "reportable": 1,
  "portfolio_id": "11e95f8ec39de8fbdb0a4f1a",
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "modified_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "quote_number_format": "quote_number_format6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

