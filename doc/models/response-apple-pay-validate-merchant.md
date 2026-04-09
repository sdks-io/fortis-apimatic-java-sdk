
# Response Apple Pay Validate Merchant

## Structure

`ResponseApplePayValidateMerchant`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type136Enum`](../../doc/models/type-136-enum.md) | Optional | Resource Type<br><br>**Default**: `Type136Enum.APPLEPAYVALIDATEMERCHANT` | Type136Enum getType() | setType(Type136Enum type) |
| `Data` | [`Data37`](../../doc/models/data-37.md) | Optional | - | Data37 getData() | setData(Data37 data) |

## Example (as JSON)

```json
{
  "type": "ApplePayValidateMerchant",
  "data": {
    "merchantSession": "merchantSession0"
  }
}
```

