
# V1 Tickets Request

## Structure

`V1TicketsRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AccountHolderName` | `String` | Optional | Account holder name<br><br>> The Name as it appears on Card.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `32` | String getAccountHolderName() | setAccountHolderName(String accountHolderName) |
| `ExpDate` | `String` | Required | The Expiration Date for the credit card. | String getExpDate() | setExpDate(String expDate) |
| `Cvv` | `String` | Optional | CVV<br><br>**Constraints**: *Maximum Length*: `4` | String getCvv() | setCvv(String cvv) |
| `AccountNumber` | `String` | Required | Account number<br><br>> A credit card number. Length 13-19.<br><br>**Constraints**: *Minimum Length*: `4`, *Maximum Length*: `19`, *Pattern*: `^[\d]+$` | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `BillingAddress` | [`BillingAddress5`](../../doc/models/billing-address-5.md) | Optional | Billing Address Object | BillingAddress5 getBillingAddress() | setBillingAddress(BillingAddress5 billingAddress) |
| `ContactId` | `String` | Optional | Used to associate the Ticket with a Contact.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getContactId() | setContactId(String contactId) |
| `ContactApiId` | `String` | Optional | Used to associate the Ticket with a Contact. | String getContactApiId() | setContactApiId(String contactApiId) |
| `LocationId` | [`V1TicketsRequestLocationId`](../../doc/models/containers/v1-tickets-request-location-id.md) | Optional | This is a container for any-of cases. | V1TicketsRequestLocationId getLocationId() | setLocationId(V1TicketsRequestLocationId locationId) |
| `LocationApiId` | `String` | Optional | Location Api Id | String getLocationApiId() | setLocationApiId(String locationApiId) |

## Example (as JSON)

```json
{
  "account_holder_name": "John Smith",
  "exp_date": "0722",
  "account_number": "545454545454545",
  "contact_id": "11e95f8ec39de8fbdb0a4f1a",
  "cvv": "cvv6",
  "billing_address": {
    "postal_code": "postal_code0",
    "street": "street8"
  },
  "contact_api_id": "contact_api_id6"
}
```

