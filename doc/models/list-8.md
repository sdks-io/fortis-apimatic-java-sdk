
# List 8

## Structure

`List8`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `String` | Optional | Deposit Id | String getId() | setId(String id) |
| `CompanyId` | `String` | Optional | Company Id | String getCompanyId() | setCompanyId(String companyId) |
| `MerchantId` | `String` | Optional | Merchant Id | String getMerchantId() | setMerchantId(String merchantId) |
| `Service` | `String` | Optional | Service | String getService() | setService(String service) |
| `DepositTypes` | [`List<DepositTypeEnum>`](../../doc/models/deposit-type-enum.md) | Optional | - | List<DepositTypeEnum> getDepositTypes() | setDepositTypes(List<DepositTypeEnum> depositTypes) |
| `DepositAmount` | `Double` | Optional | Deposit Amount | Double getDepositAmount() | setDepositAmount(Double depositAmount) |
| `BatchAmount` | `Double` | Optional | Batch Amount | Double getBatchAmount() | setBatchAmount(Double batchAmount) |
| `AdjustmentAmount` | `Double` | Optional | Adjustment Amount | Double getAdjustmentAmount() | setAdjustmentAmount(Double adjustmentAmount) |
| `RetainedAmount` | `Double` | Optional | Retained Amount | Double getRetainedAmount() | setRetainedAmount(Double retainedAmount) |
| `ConveyedAmount` | `Double` | Optional | Conveyed Amount | Double getConveyedAmount() | setConveyedAmount(Double conveyedAmount) |
| `FeeAmount` | `Double` | Optional | Fee Amount | Double getFeeAmount() | setFeeAmount(Double feeAmount) |
| `ReferenceNumber` | `String` | Optional | Reference Number | String getReferenceNumber() | setReferenceNumber(String referenceNumber) |
| `TraceNumber` | `String` | Optional | - | String getTraceNumber() | setTraceNumber(String traceNumber) |
| `Currency` | `String` | Optional | Currency | String getCurrency() | setCurrency(String currency) |
| `CreatedTs` | `Integer` | Optional | Created Timestamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ReportedDate` | `String` | Optional | Reported Date<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getReportedDate() | setReportedDate(String reportedDate) |
| `TransactionDate` | `String` | Optional | Transaction Date<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getTransactionDate() | setTransactionDate(String transactionDate) |
| `DepositAccount` | `String` | Optional | Deposit Account | String getDepositAccount() | setDepositAccount(String depositAccount) |
| `Details` | [`List<Detail2>`](../../doc/models/detail-2.md) | Optional | - | List<Detail2> getDetails() | setDetails(List<Detail2> details) |

## Example (as JSON)

```json
{
  "company_id": "8410111",
  "merchant_id": "88441",
  "deposit_amount": 2487.24,
  "batch_amount": 2487.24,
  "adjustment_amount": 2487.24,
  "retained_amount": 2487.24,
  "conveyed_amount": 2487.24,
  "fee_amount": 2487.24,
  "reference_number": "400000",
  "trace_number": "400000",
  "currency": "USD",
  "created_ts": 1422040992,
  "reported_date": "2021-12-01",
  "transaction_date": "2021-12-01",
  "id": "id0",
  "service": "service0",
  "deposit_types": [
    "fee",
    "deposit"
  ]
}
```

