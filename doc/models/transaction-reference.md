
# Transaction Reference

## Structure

`TransactionReference`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `String` | Optional | ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `TransactionId` | `String` | Optional | Transaction ID | String getTransactionId() | setTransactionId(String transactionId) |
| `PreviousTransactionId` | `String` | Optional | Previous Transaction ID | String getPreviousTransactionId() | setPreviousTransactionId(String previousTransactionId) |
| `TransactionAmount` | `Integer` | Optional | Transaction Amount | Integer getTransactionAmount() | setTransactionAmount(Integer transactionAmount) |
| `PreviousTransactionAmount` | `Integer` | Optional | Previous Transaction Amount | Integer getPreviousTransactionAmount() | setPreviousTransactionAmount(Integer previousTransactionAmount) |
| `PreviousTransactionCreatedTs` | `Double` | Optional | Previous Transaction Created Timestamp | Double getPreviousTransactionCreatedTs() | setPreviousTransactionCreatedTs(Double previousTransactionCreatedTs) |
| `ReferenceType` | `String` | Optional | Reference Type | String getReferenceType() | setReferenceType(String referenceType) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |

## Example (as JSON)

```json
{
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "transaction_id": "transaction_id2",
  "previous_transaction_id": "previous_transaction_id8",
  "transaction_amount": 188,
  "previous_transaction_amount": 176
}
```

