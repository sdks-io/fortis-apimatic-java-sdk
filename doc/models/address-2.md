
# Address 2

Address

*This model accepts additional fields of type Object.*

## Structure

`Address2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `City` | `String` | Optional | City name<br><br>**Constraints**: *Maximum Length*: `36`, *Pattern*: `^[\w\#\,\.\-\'\&\s\/]+$` | String getCity() | setCity(String city) |
| `State` | `String` | Optional | State name<br><br>**Constraints**: *Minimum Length*: `2`, *Maximum Length*: `2` | String getState() | setState(String state) |
| `PostalCode` | `String` | Optional | Postal code<br><br>**Constraints**: *Minimum Length*: `3`, *Maximum Length*: `10`, *Pattern*: `^[a-zA-Z0-9\-\s]+$` | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `Object` | Optional | - | Object getCountry() | setCountry(Object country) |
| `Street` | `String` | Optional | Street<br><br>**Constraints**: *Maximum Length*: `32`, *Pattern*: `^[\w\#\,\.\-\'\&\s\/]+$` | String getStreet() | setStreet(String street) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "city": "Novi",
  "state": "MI",
  "postal_code": "48375",
  "country": {
    "key1": "val1",
    "key2": "val2"
  },
  "street": "street0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

