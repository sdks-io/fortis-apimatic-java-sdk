
# List 15

*This model accepts additional fields of type Object.*

## Structure

`List15`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AccountHolderName` | `String` | Optional | Account holder name<br><br>> The Name as it appears on Card.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `32` | String getAccountHolderName() | setAccountHolderName(String accountHolderName) |
| `ExpDate` | `String` | Optional | The Expiration Date for the credit card. | String getExpDate() | setExpDate(String expDate) |
| `Cvv` | `String` | Optional | CVV<br><br>**Constraints**: *Maximum Length*: `4` | String getCvv() | setCvv(String cvv) |
| `AccountNumber` | `String` | Optional | Account number<br><br>> A credit card number. Length 13-19.<br><br>**Constraints**: *Minimum Length*: `4`, *Maximum Length*: `19`, *Pattern*: `^[\d]+$` | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `BillingAddress` | [`BillingAddress9`](../../doc/models/billing-address-9.md) | Optional | - | BillingAddress9 getBillingAddress() | setBillingAddress(BillingAddress9 billingAddress) |
| `ContactId` | `String` | Optional | Used to associate the Ticket with a Contact.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getContactId() | setContactId(String contactId) |
| `ContactApiId` | `String` | Optional | Used to associate the Ticket with a Contact. | String getContactApiId() | setContactApiId(String contactApiId) |
| `LocationId` | [`List15LocationId`](../../doc/models/containers/list-15-location-id.md) | Optional | This is a container for any-of cases. | List15LocationId getLocationId() | setLocationId(List15LocationId locationId) |
| `LocationApiId` | `String` | Optional | Location Api Id | String getLocationApiId() | setLocationApiId(String locationApiId) |
| `Id` | `String` | Optional | A unique, system-generated identifier for the Ticket.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "account_holder_name": "John Smith",
  "exp_date": "0722",
  "account_number": "545454545454545",
  "contact_id": "11e95f8ec39de8fbdb0a4f1a",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "cvv": "cvv6",
  "billing_address": {
    "postal_code": "postal_code0",
    "street": "street8",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

