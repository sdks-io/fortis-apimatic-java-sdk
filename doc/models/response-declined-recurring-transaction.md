
# Response Declined Recurring Transaction

## Structure

`ResponseDeclinedRecurringTransaction`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type15Enum`](../../doc/models/type-15-enum.md) | Optional | Resource Type<br><br>**Default**: `Type15Enum.DECLINEDRECURRINGTRANSACTION` | Type15Enum getType() | setType(Type15Enum type) |
| `Data` | [`Data3`](../../doc/models/data-3.md) | Optional | - | Data3 getData() | setData(Data3 data) |

## Example (as JSON)

```json
{
  "type": "DeclinedRecurringTransaction",
  "data": {
    "id": "id0",
    "declined_transaction_id": "declined_transaction_id6",
    "payment_transaction_id": "payment_transaction_id4",
    "status": "paid",
    "recurring_id": "recurring_id4"
  }
}
```

