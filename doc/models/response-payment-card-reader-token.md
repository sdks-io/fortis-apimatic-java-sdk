
# Response Payment Card Reader Token

*This model accepts additional fields of type Object.*

## Structure

`ResponsePaymentCardReaderToken`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type58`](../../doc/models/type-58.md) | Optional | - | Type58 getType() | setType(Type58 type) |
| `Data` | [`Data17`](../../doc/models/data-17.md) | Optional | - | Data17 getData() | setData(Data17 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "PaymentCardReaderToken",
  "data": {
    "token": "token4",
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

