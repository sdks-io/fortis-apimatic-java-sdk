
# Detail

*This model accepts additional fields of type Object.*

## Structure

`Detail`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Message` | `String` | Optional | - | String getMessage() | setMessage(String message) |
| `Path` | `List<String>` | Optional | - | List<String> getPath() | setPath(List<String> path) |
| `Type` | `String` | Optional | - | String getType() | setType(String type) |
| `Context` | [`Context`](../../doc/models/context.md) | Optional | - | Context getContext() | setContext(Context context) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "message": "\"fieldName\" is required",
  "type": "any.required",
  "path": [
    "path8",
    "path9"
  ],
  "context": {
    "key": "key2",
    "label": "label2",
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

