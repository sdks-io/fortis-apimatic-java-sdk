
# Data 9

*This model accepts additional fields of type Object.*

## Structure

`Data9`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Result` | [`Result`](../../doc/models/result.md) | Optional | - | Result getResult() | setResult(Result result) |
| `Status` | [`Status5`](../../doc/models/status-5.md) | Optional | - | Status5 getStatus() | setStatus(Status5 status) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "result": {
    "client_app_id": "client_app_id2",
    "dba_name": "dba_name4",
    "email": "email0",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "status": {
    "response_code": "response_code0",
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

