
# Response Paylink

*This model accepts additional fields of type Object.*

## Structure

`ResponsePaylink`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type53`](../../doc/models/type-53.md) | Optional | - | Type53 getType() | setType(Type53 type) |
| `Data` | [`Data16`](../../doc/models/data-16.md) | Optional | - | Data16 getData() | setData(Data16 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "Paylink",
  "data": {
    "location_id": "location_id4",
    "cc_product_transaction_id": "cc_product_transaction_id2",
    "email": "email6",
    "amount_due": 196,
    "location_api_id": "location_api_id0",
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

