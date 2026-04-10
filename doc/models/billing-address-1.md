
# Billing Address 1

Billing Address Object

*This model accepts additional fields of type Object.*

## Structure

`BillingAddress1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `City` | `String` | Optional | The City portion of the address associated with the Credit Card (CC) or Bank Account (ACH).<br><br>**Constraints**: *Maximum Length*: `36`, *Pattern*: `^[\w\#\,\.\-\'\&\s\/]+$` | String getCity() | setCity(String city) |
| `State` | `String` | Optional | The State portion of the address associated with the Credit Card (CC) or Bank Account (ACH).<br><br>**Constraints**: *Maximum Length*: `24` | String getState() | setState(String state) |
| `PostalCode` | `String` | Optional | The Zip or 'Postal Code' portion of the address associated with the Credit Card (CC) or Bank Account (ACH).<br><br>> Required for CC transactions if vt_require_zip is true on producttransaction(Merchant Deposit Account).<br><br>**Constraints**: *Minimum Length*: `3`, *Maximum Length*: `10`, *Pattern*: `^[a-zA-Z0-9\-\s]+$` | String getPostalCode() | setPostalCode(String postalCode) |
| `Street` | `String` | Optional | The Street portion of the address associated with the Credit Card (CC) or Bank Account (ACH).<br><br>> Required for CC transactions if vt_require_street is true on producttransaction(Merchant Deposit Account).<br><br>**Constraints**: *Maximum Length*: `32`, *Pattern*: `^[\w\#\,\.\-\'\&\s\/]+$` | String getStreet() | setStreet(String street) |
| `Phone` | `String` | Optional | The Phone # to be used to contact Payer if there are any issues processing a transaction. Country code not included<br><br>**Constraints**: *Minimum Length*: `10`, *Maximum Length*: `10`, *Pattern*: `^\d{10}$` | String getPhone() | setPhone(String phone) |
| `Country` | `String` | Optional | The alpha 3 format country code. | String getCountry() | setCountry(String country) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "city": "Novi",
  "state": "Michigan",
  "postal_code": "48375",
  "phone": "3339998822",
  "country": "USA",
  "street": "street6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

