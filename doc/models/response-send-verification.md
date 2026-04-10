
# Response Send Verification

*This model accepts additional fields of type Object.*

## Structure

`ResponseSendVerification`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type135`](../../doc/models/type-135.md) | Optional | - | Type135 getType() | setType(Type135 type) |
| `Data` | [`Data32`](../../doc/models/data-32.md) | Optional | - | Data32 getData() | setData(Data32 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "SendVerification",
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

