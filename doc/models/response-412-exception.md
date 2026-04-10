
# Response 412 Exception

*This model accepts additional fields of type Object.*

## Structure

`Response412Exception`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | `String` | Optional | - | String getType() | setType(String type) |
| `Id` | `String` | Optional | - | String getId() | setId(String id) |
| `StatusCode` | `Integer` | Optional | Response code | Integer getStatusCode() | setStatusCode(Integer statusCode) |
| `Title` | `String` | Optional | Error description | String getTitle() | setTitle(String title) |
| `Detail` | `String` | Optional | Error details | String getDetail() | setDetail(String detail) |
| `Meta` | [`Meta`](../../doc/models/meta.md) | Optional | - | Meta getMeta() | setMeta(Meta meta) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "clj4ge1234004t9ptdoz34567",
  "id": "clj4ge1234004t9ptdoz34567",
  "statusCode": 412,
  "title": "Precondition Failed",
  "detail": "\"fieldName\" is required",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

