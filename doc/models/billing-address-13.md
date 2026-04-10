
# Billing Address 13

*This model accepts additional fields of type Object.*

## Structure

`BillingAddress13`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `City` | `String` | Optional | The city of the Cardholder billing address associated with the card used for this purchase.<br><br>This field is required unless market or regional mandate restricts sending this information.<br><br>**Constraints**: *Maximum Length*: `50` | String getCity() | setCity(String city) |
| `CountryCode` | `String` | Optional | The ISO 3166-1 alpha-3 or alpha-2 country of the Cardholder billing address associated with the card used for this purchase.<br><br>The field is required if Cardholder Billing Address State is present and unless market or regional mandate restricts sending this information.<br><br>**Constraints**: *Maximum Length*: `3` | String getCountryCode() | setCountryCode(String countryCode) |
| `AddressLine1` | `String` | Optional | First line of the street address or equivalent local portion of the Cardholder billing address associated with the card use for this purchase.<br><br>This field is required unless market or regional mandate restricts sending this information.<br><br>**Constraints**: *Maximum Length*: `50` | String getAddressLine1() | setAddressLine1(String addressLine1) |
| `AddressLine2` | `String` | Optional | Second line of the street address or equivalent local portion of the Cardholder billing address associated with the card use for this purchase.<br><br>This field is required unless market or regional mandate restricts sending this information.<br><br>**Constraints**: *Maximum Length*: `50` | String getAddressLine2() | setAddressLine2(String addressLine2) |
| `AddressLine3` | `String` | Optional | Third line of the street address or equivalent local portion of the Cardholder billing address associated with the card use for this purchase.<br><br>This field is required unless market or regional mandate restricts sending this information.<br><br>**Constraints**: *Maximum Length*: `50` | String getAddressLine3() | setAddressLine3(String addressLine3) |
| `PostalCode` | `String` | Optional | ZIP or other postal code of the Cardholder billing address associated with the card used for this purchase.<br><br>This field is required unless market or regional mandate restricts sending this information.<br><br>**Constraints**: *Maximum Length*: `16` | String getPostalCode() | setPostalCode(String postalCode) |
| `State` | `String` | Optional | The state or province of the Cardholder billing address associated with the card used for this purchase. The value should be the country subdivision code defined in ISO 3166-2.<br><br>This field is required unless State is not applicable for this country and unless market or regional mandate restricts sending this information.<br><br>**Constraints**: *Maximum Length*: `3` | String getState() | setState(String state) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "city": "Plano",
  "country_code": "USA",
  "address_line_1": "6111 W Plano Parkway",
  "address_line_2": "Suite 2700",
  "postal_code": "75093",
  "state": "TX",
  "address_line_3": "address_line_32",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

