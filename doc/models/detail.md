
# Detail

## Structure

`Detail`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Message` | `String` | Optional | - | String getMessage() | setMessage(String message) |
| `Path` | `List<String>` | Optional | - | List<String> getPath() | setPath(List<String> path) |
| `Type` | `String` | Optional | - | String getType() | setType(String type) |
| `Context` | [`Context`](../../doc/models/context.md) | Optional | - | Context getContext() | setContext(Context context) |

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
    "label": "label2"
  }
}
```

