
# Billing Address 9

*This model accepts additional fields of type Object.*

## Structure

`BillingAddress9`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PostalCode` | `String` | Optional | The Zip or 'Postal Code' portion of the address associated with the Credit Card.<br><br>**Constraints**: *Minimum Length*: `3`, *Maximum Length*: `10`, *Pattern*: `^[a-zA-Z0-9\-\s]+$` | String getPostalCode() | setPostalCode(String postalCode) |
| `Street` | `String` | Optional | The Street portion of the address associated with the Credit Card.<br><br>**Constraints**: *Maximum Length*: `32`, *Pattern*: `^[\w\#\,\.\-\'\&\s\/]+$` | String getStreet() | setStreet(String street) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "postal_code": "48375",
  "street": "street4",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

