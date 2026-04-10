
# Response Device Term

*This model accepts additional fields of type Object.*

## Structure

`ResponseDeviceTerm`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type22`](../../doc/models/type-22.md) | Optional | - | Type22 getType() | setType(Type22 type) |
| `Data` | [`Data6`](../../doc/models/data-6.md) | Optional | - | Data6 getData() | setData(Data6 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "DeviceTerm",
  "data": {
    "location_id": "location_id4",
    "terminal_id": "terminal_id6",
    "require_signature": false,
    "device_term_api_id": "device_term_api_id0",
    "terms_conditions": "terms_conditions0",
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

