
# Response Send Verification

## Structure

`ResponseSendVerification`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type135Enum`](../../doc/models/type-135-enum.md) | Optional | Resource Type<br><br>**Default**: `Type135Enum.SENDVERIFICATION` | Type135Enum getType() | setType(Type135Enum type) |
| `Data` | [`Data32`](../../doc/models/data-32.md) | Optional | - | Data32 getData() | setData(Data32 data) |

## Example (as JSON)

```json
{
  "type": "SendVerification",
  "data": {
    "id": "id0",
    "user_id": "user_id8",
    "hash": "hash6",
    "created_ts": 114
  }
}
```

