
# Response Location Info

## Structure

`ResponseLocationInfo`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type44Enum`](../../doc/models/type-44-enum.md) | Optional | Resource Type<br><br>**Default**: `Type44Enum.LOCATIONINFO` | Type44Enum getType() | setType(Type44Enum type) |
| `Data` | [`Data11`](../../doc/models/data-11.md) | Optional | - | Data11 getData() | setData(Data11 data) |

## Example (as JSON)

```json
{
  "type": "LocationInfo",
  "data": {
    "id": "id0",
    "created_ts": 114,
    "modified_ts": 190,
    "account_number": "account_number0",
    "address": {
      "city": "city6",
      "state": "state2",
      "postal_code": "postal_code8",
      "country": "US",
      "street": "street6"
    }
  }
}
```

