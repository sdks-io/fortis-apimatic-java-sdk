
# Address 4

*This model accepts additional fields of type Object.*

## Structure

`Address4`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `City` | `String` | Optional | City of contact<br><br>**Constraints**: *Maximum Length*: `36`, *Pattern*: `^[\w\#\,\.\-\'\&\s\/]+$` | String getCity() | setCity(String city) |
| `State` | `String` | Optional | State of contact<br><br>**Constraints**: *Maximum Length*: `24` | String getState() | setState(String state) |
| `PostalCode` | `String` | Optional | Postal code of contact<br><br>**Constraints**: *Minimum Length*: `3`, *Maximum Length*: `10`, *Pattern*: `^[a-zA-Z0-9\-\s]+$` | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `String` | Optional | The alpha 2 or alpha 3 format country code. If alpha 3 is provided, it will be converted to alpha 2. | String getCountry() | setCountry(String country) |
| `Street` | `String` | Optional | Street of contact<br><br>**Constraints**: *Maximum Length*: `32`, *Pattern*: `^[\w\#\,\.\-\'\&\s\/]+$` | String getStreet() | setStreet(String street) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "city": "Novi",
  "state": "Michigan",
  "postal_code": "48375",
  "country": "USA",
  "street": "street2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

