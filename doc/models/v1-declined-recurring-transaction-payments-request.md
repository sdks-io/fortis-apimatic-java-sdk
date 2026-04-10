
# V1 Declined Recurring Transaction Payments Request

*This model accepts additional fields of type Object.*

## Structure

`V1DeclinedRecurringTransactionPaymentsRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `DeclinedRecurringTransactionId` | `String` | Required | Declined Recurring Transaction Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getDeclinedRecurringTransactionId() | setDeclinedRecurringTransactionId(String declinedRecurringTransactionId) |
| `AccountNumber` | `String` | Required | Account Number<br><br>**Constraints**: *Minimum Length*: `13`, *Maximum Length*: `19` | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `AccountHolderName` | `String` | Optional | Account Holder Name | String getAccountHolderName() | setAccountHolderName(String accountHolderName) |
| `ExpDate` | `String` | Required | Exp Date<br><br>**Constraints**: *Maximum Length*: `4` | String getExpDate() | setExpDate(String expDate) |
| `TransactionAmount` | `int` | Required | Transaction Amount<br><br>**Constraints**: `>= 0`, `<= 999999999` | int getTransactionAmount() | setTransactionAmount(int transactionAmount) |
| `Description` | `String` | Optional | Description<br><br>**Constraints**: *Maximum Length*: `255` | String getDescription() | setDescription(String description) |
| `BillingAddress` | [`BillingAddress7`](../../doc/models/billing-address-7.md) | Optional | - | BillingAddress7 getBillingAddress() | setBillingAddress(BillingAddress7 billingAddress) |
| `Tags` | `List<String>` | Optional | Tags | List<String> getTags() | setTags(List<String> tags) |
| `ReplaceAccountVault` | `Boolean` | Optional | Replace AccountVault | Boolean getReplaceAccountVault() | setReplaceAccountVault(Boolean replaceAccountVault) |
| `SaveAccount` | `Boolean` | Optional | Specifies to save account to contacts profile if account_number/track_data is present with either contact_id or contact_api_id in params. | Boolean getSaveAccount() | setSaveAccount(Boolean saveAccount) |
| `SaveAccountTitle` | `String` | Optional | If saving token while running a transaction, this will be the title of the token.<br><br>**Constraints**: *Maximum Length*: `16` | String getSaveAccountTitle() | setSaveAccountTitle(String saveAccountTitle) |
| `SubtotalAmount` | `Integer` | Optional | Subtotal Amount<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getSubtotalAmount() | setSubtotalAmount(Integer subtotalAmount) |
| `SurchargeAmount` | `Integer` | Optional | Surcharge Amount<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getSurchargeAmount() | setSurchargeAmount(Integer surchargeAmount) |
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
  "save_account_title": "John Account",
  "subtotal_amount": 599,
  "surcharge_amount": 599,
  "billing_address": {
    "postal_code": "postal_code0",
    "street": "street8",
    "city": "city2",
    "state": "state6",
    "phone": "phone2",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "tags": [
    "tags3",
    "tags4"
  ],
  "replace_account_vault": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

