
# Response Async Status

## Structure

`ResponseAsyncStatus`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`TypeEnum`](../../doc/models/type-enum.md) | Optional | Resource Type<br><br>**Default**: `TypeEnum.ASYNCSTATUS` | TypeEnum getType() | setType(TypeEnum type) |
| `Data` | [`Data`](../../doc/models/data.md) | Optional | - | Data getData() | setData(Data data) |

## Example (as JSON)

```json
{
  "type": "AsyncStatus",
  "data": {
    "code": "00001e1c-0000-0000-0000-000000000000",
    "type": "type0",
    "id": "id0",
    "progress": 100,
    "error": "error4"
  }
}
```

