
# Response Fullboarding

## Structure

`ResponseFullboarding`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type30Enum`](../../doc/models/type-30-enum.md) | Optional | Resource Type<br><br>**Default**: `Type30Enum.FULLBOARDING` | Type30Enum getType() | setType(Type30Enum type) |
| `Data` | [`Data9`](../../doc/models/data-9.md) | Optional | - | Data9 getData() | setData(Data9 data) |

## Example (as JSON)

```json
{
  "type": "Fullboarding",
  "data": {
    "result": {
      "client_app_id": "client_app_id2",
      "dba_name": "dba_name4",
      "email": "email0"
    },
    "status": {
      "response_code": "response_code0"
    }
  }
}
```

