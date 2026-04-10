
# Response Remove Verification

*This model accepts additional fields of type Object.*

## Structure

`ResponseRemoveVerification`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type134`](../../doc/models/type-134.md) | Optional | - | Type134 getType() | setType(Type134 type) |
| `Data` | [`Data32`](../../doc/models/data-32.md) | Optional | - | Data32 getData() | setData(Data32 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "RemoveVerification",
  "data": {
    "id": "id0",
    "user_id": "user_id8",
    "hash": "hash6",
    "created_ts": 114,
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

