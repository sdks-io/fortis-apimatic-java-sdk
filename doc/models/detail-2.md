
# Detail 2

*This model accepts additional fields of type Object.*

## Structure

`Detail2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ProcessorBatchNumber` | `String` | Optional | Processor Batch Number | String getProcessorBatchNumber() | setProcessorBatchNumber(String processorBatchNumber) |
| `ProductCode` | `String` | Optional | Product Code | String getProductCode() | setProductCode(String productCode) |
| `DepositDetailType` | `String` | Optional | Deposit Detail Type | String getDepositDetailType() | setDepositDetailType(String depositDetailType) |
| `Amount` | `Double` | Optional | Amount | Double getAmount() | setAmount(Double amount) |
| `Memo` | `String` | Optional | Memo | String getMemo() | setMemo(String memo) |
| `ReportedDate` | `String` | Optional | Reported Date<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getReportedDate() | setReportedDate(String reportedDate) |
| `SettledDate` | `String` | Optional | Settled Date<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getSettledDate() | setSettledDate(String settledDate) |
| `Mid` | `String` | Optional | Merchant ID | String getMid() | setMid(String mid) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "amount": 2487.24,
  "reported_date": "2021-12-01",
  "settled_date": "2021-12-01",
  "processor_batch_number": "processor_batch_number6",
  "product_code": "product_code8",
  "deposit_detail_type": "deposit_detail_type6",
  "memo": "memo6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

