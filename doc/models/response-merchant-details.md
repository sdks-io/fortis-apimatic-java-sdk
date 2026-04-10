
# Response Merchant Details

*This model accepts additional fields of type Object.*

## Structure

`ResponseMerchantDetails`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type137`](../../doc/models/type-137.md) | Optional | - | Type137 getType() | setType(Type137 type) |
| `Data` | [`Data38`](../../doc/models/data-38.md) | Optional | - | Data38 getData() | setData(Data38 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "MerchantDetails",
  "data": {
    "resultCode": false,
    "merchantID": "merchantID8",
    "applePay": false,
    "googlePay": false,
    "applePayDomains": [
      {
        "key1": "val1",
        "key2": "val2"
      }
    ],
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

