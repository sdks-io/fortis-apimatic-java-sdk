
# Response 417 Filter Channels

*This model accepts additional fields of type Object.*

## Structure

`Response417FilterChannels`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `StatusCode` | `Integer` | Optional | Response code | Integer getStatusCode() | setStatusCode(Integer statusCode) |
| `Error` | `String` | Optional | Expectation Failed | String getError() | setError(String error) |
| `Message` | `String` | Optional | Channel filters are not set for this project | String getMessage() | setMessage(String message) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "statusCode": 417,
  "error": "Expectation Failed",
  "message": "Channel filters are not set for this project",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

