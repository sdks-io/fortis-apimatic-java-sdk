
# V1 Elements Transaction Intention Request

*This model accepts additional fields of type Object.*

## Structure

`V1ElementsTransactionIntentionRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Action` | `Object` | Optional | - | Object getAction() | setAction(Object action) |
| `DigitalWalletsOnly` | `Boolean` | Optional | **Default**: `false` | Boolean getDigitalWalletsOnly() | setDigitalWalletsOnly(Boolean digitalWalletsOnly) |
| `Methods` | [`List<Method50>`](../../doc/models/method-50.md) | Optional | By default the system will try to offer all the availables payment methods from your account. However, if you need to display only cc or ach only use the corresponding product transaction id.<br><br>**Constraints**: *Minimum Items*: `1`, *Unique Items Required* | List<Method50> getMethods() | setMethods(List<Method50> methods) |
| `Amount` | `Integer` | Optional | The total transaction amount to be charged with the transaction intention. Allowed on the actions: `sale`, `auth-only`, `refund`<br><br>**Constraints**: `>= 1`, `<= 999999999` | Integer getAmount() | setAmount(Integer amount) |
| `TaxAmount` | `Integer` | Optional | Amount of Sales Tax. If supplied, this amount should be already included in the transaction amount. Allowed on the actions: `sale`, `auth-only`, `refund`<br><br>**Constraints**: `>= 1`, `<= 999999999` | Integer getTaxAmount() | setTaxAmount(Integer taxAmount) |
| `SecondaryAmount` | `Integer` | Optional | secondary_amount is used as a mechanism for partners to collect platform or SaAs fees at a transaction level. This field is intended for use with ISV integrations not standalone merchant integrations. Allowed on the actions: `sale`, `auth-only`.<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getSecondaryAmount() | setSecondaryAmount(Integer secondaryAmount) |
| `LocationId` | `String` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `ContactId` | `String` | Optional | Contact ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getContactId() | setContactId(String contactId) |
| `SaveAccount` | `Boolean` | Optional | Specifies to tokenize card/bank information within the transaction. Allowed on the actions: `sale`, `auth-only`, `avs-only`, `refund`. Do not include with `tokeniation` action. | Boolean getSaveAccount() | setSaveAccount(Boolean saveAccount) |
| `SaveAccountTitle` | `String` | Optional | Specifies to tokenize card/bank information within the transaction. Allowed on the actions: `sale`, `auth-only`, `avs-only`, `refund`. Do not include with `tokeniation` action.<br><br>**Constraints**: *Maximum Length*: `16` | String getSaveAccountTitle() | setSaveAccountTitle(String saveAccountTitle) |
| `Title` | `String` | Optional | A title for the token.<br><br>**Constraints**: *Maximum Length*: `16` | String getTitle() | setTitle(String title) |
| `AchSecCode` | `Object` | Optional | - | Object getAchSecCode() | setAchSecCode(Object achSecCode) |
| `BankFundedOnlyOverride` | `Boolean` | Optional | Bank Funded Only Override. Force the use of a bank funded debit card on debit repayment type transactions. | Boolean getBankFundedOnlyOverride() | setBankFundedOnlyOverride(Boolean bankFundedOnlyOverride) |
| `AllowPartialAuthorizationOverride` | `Boolean` | Optional | Allow partial Authorization Override. Must have Fortis approval for production access. | Boolean getAllowPartialAuthorizationOverride() | setAllowPartialAuthorizationOverride(Boolean allowPartialAuthorizationOverride) |
| `AutoDeclineCvvOverride` | `Boolean` | Optional | Auto Decline Cvv Override | Boolean getAutoDeclineCvvOverride() | setAutoDeclineCvvOverride(Boolean autoDeclineCvvOverride) |
| `AutoDeclineStreetOverride` | `Boolean` | Optional | Auto Decline Street Override | Boolean getAutoDeclineStreetOverride() | setAutoDeclineStreetOverride(Boolean autoDeclineStreetOverride) |
| `AutoDeclineZipOverride` | `Boolean` | Optional | Auto Decline Zip Override | Boolean getAutoDeclineZipOverride() | setAutoDeclineZipOverride(Boolean autoDeclineZipOverride) |
| `Message` | `String` | Optional | A custom text message that displays after the payment is processed.<br><br>**Constraints**: *Maximum Length*: `120` | String getMessage() | setMessage(String message) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "digitalWalletsOnly": false,
  "amount": 1099,
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "contact_id": "11e95f8ec39de8fbdb0a4f1a",
  "action": {
    "key1": "val1",
    "key2": "val2"
  },
  "methods": [
    {
      "type": "ach",
      "product_transaction_id": "product_transaction_id4",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "type": "ach",
      "product_transaction_id": "product_transaction_id4",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "tax_amount": 52,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

