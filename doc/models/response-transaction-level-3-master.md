
# Response Transaction Level 3 Master

*This model accepts additional fields of type Object.*

## Structure

`ResponseTransactionLevel3Master`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type114`](../../doc/models/type-114.md) | Optional | - | Type114 getType() | setType(Type114 type) |
| `Data` | [`Data29`](../../doc/models/data-29.md) | Optional | - | Data29 getData() | setData(Data29 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "TransactionLevel3Master",
  "data": {
    "id": "id0",
    "transaction_id": "transaction_id8",
    "level3_data": {
      "destination_country_code": "destination_country_code4",
      "duty_amount": 182,
      "freight_amount": 60,
      "national_tax": 999999998900,
      "sales_tax": 999999998900,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
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

