
# Response Fullboarding

*This model accepts additional fields of type Object.*

## Structure

`ResponseFullboarding`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type30`](../../doc/models/type-30.md) | Optional | - | Type30 getType() | setType(Type30 type) |
| `Data` | [`Data9`](../../doc/models/data-9.md) | Optional | - | Data9 getData() | setData(Data9 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "Fullboarding",
  "data": {
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
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

