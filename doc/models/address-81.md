
# Address 81

Array of merchant addresses.

## Structure

`Address81`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AddressLine1` | `String` | Required | Line 1 of address.<br><br>**Constraints**: *Maximum Length*: `100` | String getAddressLine1() | setAddressLine1(String addressLine1) |
| `AddressLine2` | `String` | Optional | Line 2 of address.<br><br>**Constraints**: *Maximum Length*: `20` | String getAddressLine2() | setAddressLine2(String addressLine2) |
| `City` | `String` | Required | City of address.<br><br>**Constraints**: *Maximum Length*: `50` | String getCity() | setCity(String city) |
| `StateProvince` | `String` | Required | State or province of address.<br><br>**Constraints**: *Maximum Length*: `2` | String getStateProvince() | setStateProvince(String stateProvince) |
| `PostalCode` | `String` | Required | Postal code of address.<br><br>**Constraints**: *Maximum Length*: `10` | String getPostalCode() | setPostalCode(String postalCode) |
| `CountryCode` | `String` | Required | Country of address.<br><br>**Constraints**: *Maximum Length*: `2` | String getCountryCode() | setCountryCode(String countryCode) |
| `AddressType` | [`AddressTypeEnum`](../../doc/models/address-type-enum.md) | Required | Address type of address.<br><br>**Constraints**: *Maximum Length*: `20` | AddressTypeEnum getAddressType() | setAddressType(AddressTypeEnum addressType) |

## Example (as JSON)

```json
{
  "address_line_1": "121 E Main",
  "address_line_2": "Apt 707",
  "city": "Dallas",
  "state_province": "TX",
  "postal_code": "75087",
  "country_code": "US",
  "address_type": "location"
}
```

