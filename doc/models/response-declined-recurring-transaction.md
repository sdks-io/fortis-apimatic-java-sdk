
# Response Declined Recurring Transaction

*This model accepts additional fields of type Object.*

## Structure

`ResponseDeclinedRecurringTransaction`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type15`](../../doc/models/type-15.md) | Optional | - | Type15 getType() | setType(Type15 type) |
| `Data` | [`Data3`](../../doc/models/data-3.md) | Optional | - | Data3 getData() | setData(Data3 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "DeclinedRecurringTransaction",
  "data": {
    "id": "id0",
    "declined_transaction_id": "declined_transaction_id6",
    "payment_transaction_id": "payment_transaction_id4",
    "status": "paid",
    "recurring_id": "recurring_id4",
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

