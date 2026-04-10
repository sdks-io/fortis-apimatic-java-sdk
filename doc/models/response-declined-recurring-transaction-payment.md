
# Response Declined Recurring Transaction Payment

*This model accepts additional fields of type Object.*

## Structure

`ResponseDeclinedRecurringTransactionPayment`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type20`](../../doc/models/type-20.md) | Optional | - | Type20 getType() | setType(Type20 type) |
| `Data` | [`Data4`](../../doc/models/data-4.md) | Optional | - | Data4 getData() | setData(Data4 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "DeclinedRecurringTransactionPayment",
  "data": {
    "declined_recurring_transaction_id": "declined_recurring_transaction_id6",
    "account_number": "account_number0",
    "account_holder_name": "account_holder_name0",
    "exp_date": "exp_date8",
    "transaction_amount": 88,
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

