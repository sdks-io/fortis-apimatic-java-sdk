
# Data 4

*This model accepts additional fields of type Object.*

## Structure

`Data4`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `DeclinedRecurringTransactionId` | `String` | Optional | Declined Recurring Transaction Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getDeclinedRecurringTransactionId() | setDeclinedRecurringTransactionId(String declinedRecurringTransactionId) |
| `AccountNumber` | `String` | Optional | Account Number<br><br>**Constraints**: *Minimum Length*: `13`, *Maximum Length*: `19` | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `AccountHolderName` | `String` | Optional | Account Holder Name | String getAccountHolderName() | setAccountHolderName(String accountHolderName) |
| `ExpDate` | `String` | Optional | Exp Date<br><br>**Constraints**: *Maximum Length*: `4` | String getExpDate() | setExpDate(String expDate) |
| `TransactionAmount` | `Integer` | Optional | Transaction Amount<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getTransactionAmount() | setTransactionAmount(Integer transactionAmount) |
| `Description` | `String` | Optional | Description<br><br>**Constraints**: *Maximum Length*: `255` | String getDescription() | setDescription(String description) |
| `BillingAddress` | [`BillingAddress7`](../../doc/models/billing-address-7.md) | Optional | - | BillingAddress7 getBillingAddress() | setBillingAddress(BillingAddress7 billingAddress) |
| `Tags` | `List<String>` | Optional | Tags | List<String> getTags() | setTags(List<String> tags) |
| `Id` | `String` | Optional | Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `FirstSix` | `String` | Optional | First Six<br><br>**Constraints**: *Maximum Length*: `6` | String getFirstSix() | setFirstSix(String firstSix) |
| `LastFour` | `String` | Optional | Last Four<br><br>**Constraints**: *Maximum Length*: `4` | String getLastFour() | setLastFour(String lastFour) |
| `Routing` | `String` | Optional | Routing | String getRouting() | setRouting(String routing) |
| `StatusId` | `Double` | Optional | Status Id | Double getStatusId() | setStatusId(Double statusId) |
| `ReasonCodeId` | `Object` | Optional | - | Object getReasonCodeId() | setReasonCodeId(Object reasonCodeId) |
| `TypeId` | `Double` | Optional | Type Id | Double getTypeId() | setTypeId(Double typeId) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "declined_recurring_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "account_number": "5454545454545454",
  "account_holder_name": "John Doe",
  "exp_date": "0722",
  "transaction_amount": 0,
  "description": "Description",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "first_six": "700953",
  "last_four": "3657",
  "created_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

