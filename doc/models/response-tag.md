
# Response Tag

## Structure

`ResponseTag`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type77Enum`](../../doc/models/type-77-enum.md) | Optional | Resource Type<br><br>**Default**: `Type77Enum.TAG` | Type77Enum getType() | setType(Type77Enum type) |
| `Data` | [`Data22`](../../doc/models/data-22.md) | Optional | - | Data22 getData() | setData(Data22 data) |

## Example (as JSON)

```json
{
  "type": "Tag",
  "data": {
    "location_id": "location_id4",
    "title": "title6",
    "id": "id0",
    "created_ts": 114,
    "modified_ts": 190
  }
}
```

