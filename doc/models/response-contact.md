
# Response Contact

*This model accepts additional fields of type Object.*

## Structure

`ResponseContact`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type10`](../../doc/models/type-10.md) | Optional | - | Type10 getType() | setType(Type10 type) |
| `Data` | [`Data2`](../../doc/models/data-2.md) | Optional | - | Data2 getData() | setData(Data2 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "Contact",
  "data": {
    "location_id": "location_id4",
    "account_number": "account_number0",
    "contact_api_id": "contact_api_id4",
    "first_name": "first_name0",
    "last_name": "last_name8",
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

