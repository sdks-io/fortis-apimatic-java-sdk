
# Response Transaction Intention

*This model accepts additional fields of type Object.*

## Structure

`ResponseTransactionIntention`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type28`](../../doc/models/type-28.md) | Optional | - | Type28 getType() | setType(Type28 type) |
| `Data` | [`Data8`](../../doc/models/data-8.md) | Optional | - | Data8 getData() | setData(Data8 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "TransactionIntention",
  "data": {
    "action": {
      "key1": "val1",
      "key2": "val2"
    },
    "digitalWalletsOnly": false,
    "methods": [
      {
        "type": "ach",
        "product_transaction_id": "product_transaction_id4",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      }
    ],
    "amount": 236,
    "tax_amount": 218,
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

