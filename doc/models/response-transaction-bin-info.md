
# Response Transaction Bin Info

*This model accepts additional fields of type Object.*

## Structure

`ResponseTransactionBinInfo`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type113`](../../doc/models/type-113.md) | Optional | - | Type113 getType() | setType(Type113 type) |
| `Data` | [`Data28`](../../doc/models/data-28.md) | Optional | - | Data28 getData() | setData(Data28 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "TransactionBinInfo",
  "data": {
    "issuer_bank_name": "issuer_bank_name6",
    "country_code": "country_code0",
    "detail_card_product": "detail_card_product2",
    "detail_card_indicator": "detail_card_indicator2",
    "fsa_indicator": "fsa_indicator8",
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

