
# Response Tag

*This model accepts additional fields of type Object.*

## Structure

`ResponseTag`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type77`](../../doc/models/type-77.md) | Optional | - | Type77 getType() | setType(Type77 type) |
| `Data` | [`Data22`](../../doc/models/data-22.md) | Optional | - | Data22 getData() | setData(Data22 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "Tag",
  "data": {
    "location_id": "location_id4",
    "title": "title6",
    "id": "id0",
    "created_ts": 114,
    "modified_ts": 190,
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

