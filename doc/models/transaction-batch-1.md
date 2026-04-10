
# Transaction Batch 1

*This model accepts additional fields of type Object.*

## Structure

`TransactionBatch1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `String` | Optional | Batch ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ProductTransactionId` | `String` | Optional | Product Transaction Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getProductTransactionId() | setProductTransactionId(String productTransactionId) |
| `ProcessingStatusId` | `Integer` | Optional | Processing Status Id<br><br>**Constraints**: `>= 1`, `<= 5` | Integer getProcessingStatusId() | setProcessingStatusId(Integer processingStatusId) |
| `BatchNum` | `Integer` | Optional | Batch Number | Integer getBatchNum() | setBatchNum(Integer batchNum) |
| `IsOpen` | `Double` | Optional | 1 = Batch is_open, 0 = Batch is closed. Only 1 open batch per product_transaction_id.<br><br>**Constraints**: `>= 0`, `<= 1` | Double getIsOpen() | setIsOpen(Double isOpen) |
| `SettlementFileName` | `String` | Optional | Settlement File Name | String getSettlementFileName() | setSettlementFileName(String settlementFileName) |
| `BatchCloseTs` | `Double` | Optional | Batch Close Ts in unix | Double getBatchCloseTs() | setBatchCloseTs(Double batchCloseTs) |
| `BatchCloseDetail` | `String` | Optional | Batch Close Detail | String getBatchCloseDetail() | setBatchCloseDetail(String batchCloseDetail) |
| `TotalSaleAmount` | `Integer` | Optional | Total Sale Amount | Integer getTotalSaleAmount() | setTotalSaleAmount(Integer totalSaleAmount) |
| `TotalSaleCount` | `Integer` | Optional | Total Sale Count | Integer getTotalSaleCount() | setTotalSaleCount(Integer totalSaleCount) |
| `TotalRefundAmount` | `Integer` | Optional | Total Refund Amount | Integer getTotalRefundAmount() | setTotalRefundAmount(Integer totalRefundAmount) |
| `TotalRefundCount` | `Integer` | Optional | Total Refund Count | Integer getTotalRefundCount() | setTotalRefundCount(Integer totalRefundCount) |
| `TotalVoidAmount` | `Integer` | Optional | Total Void Amount | Integer getTotalVoidAmount() | setTotalVoidAmount(Integer totalVoidAmount) |
| `TotalVoidCount` | `Integer` | Optional | Total Void Count | Integer getTotalVoidCount() | setTotalVoidCount(Integer totalVoidCount) |
| `TotalBlindRefundAmount` | `Integer` | Optional | Total Blind Refund Amount | Integer getTotalBlindRefundAmount() | setTotalBlindRefundAmount(Integer totalBlindRefundAmount) |
| `TotalBlindRefundCount` | `Integer` | Optional | Total Blind Refund Count | Integer getTotalBlindRefundCount() | setTotalBlindRefundCount(Integer totalBlindRefundCount) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "processing_status_id": 2,
  "batch_num": 4,
  "is_open": 0,
  "settlement_file_name": "settement_file.txt",
  "batch_close_ts": 1531423693,
  "batch_close_detail": "BATCH_MISMATCH",
  "total_sale_amount": 2342,
  "total_sale_count": 21,
  "total_refund_amount": 2342,
  "total_refund_count": 18,
  "total_void_amount": 2342,
  "total_void_count": 17,
  "total_blind_refund_amount": 2342,
  "total_blind_refund_count": 16,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

