
# File 5

*This model accepts additional fields of type Object.*

## Structure

`File5`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `FileName` | `String` | Optional | The file name including the extension | String getFileName() | setFileName(String fileName) |
| `Content` | `String` | Optional | File contents as a base64 encoded string | String getContent() | setContent(String content) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "file_name": "file_name6",
  "content": "content6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

