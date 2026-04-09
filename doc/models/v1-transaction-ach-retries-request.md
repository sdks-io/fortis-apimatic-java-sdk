
# V1 Transaction Ach Retries Request

## Structure

`V1TransactionAchRetriesRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RejectedTransactionId` | `String` | Required | Rejected Transaction ID.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getRejectedTransactionId() | setRejectedTransactionId(String rejectedTransactionId) |
| `ReturnFee` | `Integer` | Optional | Return Fee.<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getReturnFee() | setReturnFee(Integer returnFee) |

## Example (as JSON)

```json
{
  "rejected_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "return_fee": 82
}
```

