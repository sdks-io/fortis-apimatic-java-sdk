
# Location 52

*This model accepts additional fields of type Object.*

## Structure

`Location52`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AddressLine1` | `String` | Optional | Merchant's business address line 1.<br><br>**Constraints**: *Maximum Length*: `100` | String getAddressLine1() | setAddressLine1(String addressLine1) |
| `AddressLine2` | `String` | Optional | Merchant's business address line 2.<br><br>**Constraints**: *Maximum Length*: `20` | String getAddressLine2() | setAddressLine2(String addressLine2) |
| `City` | `String` | Optional | Merchant's business city.<br><br>**Constraints**: *Maximum Length*: `50` | String getCity() | setCity(String city) |
| `StateProvince` | `String` | Optional | Merchant's business two-digit state or province code.<br><br>**Constraints**: *Maximum Length*: `2` | String getStateProvince() | setStateProvince(String stateProvince) |
| `PostalCode` | `String` | Optional | Merchant's business postal code.<br><br>**Constraints**: *Maximum Length*: `10` | String getPostalCode() | setPostalCode(String postalCode) |
| `PhoneNumber` | `String` | Optional | Merchant's business phone number.<br><br>**Constraints**: *Maximum Length*: `20` | String getPhoneNumber() | setPhoneNumber(String phoneNumber) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "address_line_1": "1200 West Hartford Pkwy",
  "address_line_2": "Suite 2000",
  "city": "Dover",
  "state_province": "DE",
  "postal_code": "55022",
  "phone_number": "555-555-1212",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

