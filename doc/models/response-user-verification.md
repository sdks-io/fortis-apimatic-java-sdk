
# Response User Verification

## Structure

`ResponseUserVerification`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type123Enum`](../../doc/models/type-123-enum.md) | Optional | Resource Type<br><br>**Default**: `Type123Enum.USERVERIFICATION` | Type123Enum getType() | setType(Type123Enum type) |
| `Data` | [`Data32`](../../doc/models/data-32.md) | Optional | - | Data32 getData() | setData(Data32 data) |

## Example (as JSON)

```json
{
  "type": "UserVerification",
  "data": {
    "id": "id0",
    "user_id": "user_id8",
    "hash": "hash6",
    "created_ts": 114
  }
}
```

