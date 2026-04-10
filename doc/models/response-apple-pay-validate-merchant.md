
# Response Apple Pay Validate Merchant

*This model accepts additional fields of type Object.*

## Structure

`ResponseApplePayValidateMerchant`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type136`](../../doc/models/type-136.md) | Optional | - | Type136 getType() | setType(Type136 type) |
| `Data` | [`Data37`](../../doc/models/data-37.md) | Optional | - | Data37 getData() | setData(Data37 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "ApplePayValidateMerchant",
  "data": {
    "merchantSession": "merchantSession0",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

