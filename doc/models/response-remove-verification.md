
# Response Remove Verification

## Structure

`ResponseRemoveVerification`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type134Enum`](../../doc/models/type-134-enum.md) | Optional | Resource Type<br><br>**Default**: `Type134Enum.REMOVEVERIFICATION` | Type134Enum getType() | setType(Type134Enum type) |
| `Data` | [`Data32`](../../doc/models/data-32.md) | Optional | - | Data32 getData() | setData(Data32 data) |

## Example (as JSON)

```json
{
  "type": "RemoveVerification",
  "data": {
    "id": "id0",
    "user_id": "user_id8",
    "hash": "hash6",
    "created_ts": 114
  }
}
```

