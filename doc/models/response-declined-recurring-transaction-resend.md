
# Response Declined Recurring Transaction Resend

*This model accepts additional fields of type Object.*

## Structure

`ResponseDeclinedRecurringTransactionResend`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type21`](../../doc/models/type-21.md) | Optional | - | Type21 getType() | setType(Type21 type) |
| `Data` | [`Data5`](../../doc/models/data-5.md) | Optional | - | Data5 getData() | setData(Data5 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "DeclinedRecurringTransactionResend",
  "data": {
    "id": "id0",
    "email_log_id": "email_log_id2",
    "success": false,
    "email": "email6",
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

