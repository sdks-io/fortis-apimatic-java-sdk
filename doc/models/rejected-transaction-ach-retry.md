
# Rejected Transaction Ach Retry

*This model accepts additional fields of type Object.*

## Structure

`RejectedTransactionAchRetry`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RejectedTransactionId` | `String` | Optional | Rejected Transaction ID.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getRejectedTransactionId() | setRejectedTransactionId(String rejectedTransactionId) |
| `ReturnFee` | `Integer` | Optional | Return Fee.<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getReturnFee() | setReturnFee(Integer returnFee) |
| `Id` | `String` | Optional | Transaction ACH Retry ID.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `RetryTransactionId` | `String` | Optional | Retry Transaction ID.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getRetryTransactionId() | setRetryTransactionId(String retryTransactionId) |
| `ReturnFeeTransactionId` | `String` | Optional | Return Fee Transaction ID.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getReturnFeeTransactionId() | setReturnFeeTransactionId(String returnFeeTransactionId) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "rejected_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "retry_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "return_fee_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "return_fee": 200,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

