
# Response 401 Token Exception

## Structure

`Response401tokenException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `StatusCode` | `Integer` | Optional | Response code | Integer getStatusCode() | setStatusCode(Integer statusCode) |
| `Error` | `String` | Optional | Unauthorized | String getError() | setError(String error) |
| `Message` | `String` | Optional | Invalid token | String getMessageField() | setMessageField(String messageField) |

## Example (as JSON)

```json
{
  "statusCode": 401,
  "error": "Unauthorized",
  "message": "Invalid token"
}
```

