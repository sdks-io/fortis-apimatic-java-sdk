
# Response 401 Token Exception

*This model accepts additional fields of type Object.*

## Structure

`Response401TokenException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `StatusCode` | `Integer` | Optional | Response code | Integer getStatusCode() | setStatusCode(Integer statusCode) |
| `Error` | `String` | Optional | Unauthorized | String getError() | setError(String error) |
| `Message` | `String` | Optional | Invalid token | String getMessageField() | setMessageField(String messageField) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "statusCode": 401,
  "error": "Unauthorized",
  "message": "Invalid token",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

