
# Response User Api Key

## Structure

`ResponseUserApiKey`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type128Enum`](../../doc/models/type-128-enum.md) | Optional | Resource Type<br><br>**Default**: `Type128Enum.USERAPIKEY` | Type128Enum getType() | setType(Type128Enum type) |
| `Data` | [`Data33`](../../doc/models/data-33.md) | Optional | - | Data33 getData() | setData(Data33 data) |

## Example (as JSON)

```json
{
  "type": "UserApiKey",
  "data": {
    "user_api_key": "user_api_key2"
  }
}
```

