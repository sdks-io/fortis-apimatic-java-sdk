
# Response Signature

## Structure

`ResponseSignature`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type72Enum`](../../doc/models/type-72-enum.md) | Optional | Resource Type<br><br>**Default**: `Type72Enum.SIGNATURE` | Type72Enum getType() | setType(Type72Enum type) |
| `Data` | [`Data21`](../../doc/models/data-21.md) | Optional | - | Data21 getData() | setData(Data21 data) |

## Example (as JSON)

```json
{
  "type": "Signature",
  "data": {
    "signature": "signature8",
    "resource": "AccountVault",
    "resource_id": "resource_id6",
    "id": "id0",
    "created_ts": 114
  }
}
```

