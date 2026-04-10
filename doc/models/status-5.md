
# Status 5

*This model accepts additional fields of type Object.*

## Structure

`Status5`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ResponseCode` | `String` | Optional | Response code for API response.<br><br>**Constraints**: *Maximum Length*: `20` | String getResponseCode() | setResponseCode(String responseCode) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "response_code": "Received",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

