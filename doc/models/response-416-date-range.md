
# Response 416 Date Range

*This model accepts additional fields of type Object.*

## Structure

`Response416DateRange`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `StatusCode` | `Integer` | Optional | Response code | Integer getStatusCode() | setStatusCode(Integer statusCode) |
| `Error` | `String` | Optional | Requested Range Not Satisfiable | String getError() | setError(String error) |
| `Message` | `String` | Optional | The "fieldDate" should be less or equal to "ISODate". | String getMessage() | setMessage(String message) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "statusCode": 416,
  "error": "Requested Range Not Satisfiable",
  "message": "The \"startDate\" should be less or equal \"2019-08-20T03:00:00.000Z\".",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

