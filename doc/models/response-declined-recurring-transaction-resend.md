
# Response Declined Recurring Transaction Resend

## Structure

`ResponseDeclinedRecurringTransactionResend`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type21Enum`](../../doc/models/type-21-enum.md) | Optional | Resource Type<br><br>**Default**: `Type21Enum.DECLINEDRECURRINGTRANSACTIONRESEND` | Type21Enum getType() | setType(Type21Enum type) |
| `Data` | [`Data5`](../../doc/models/data-5.md) | Optional | - | Data5 getData() | setData(Data5 data) |

## Example (as JSON)

```json
{
  "type": "DeclinedRecurringTransactionResend",
  "data": {
    "id": "id0",
    "email_log_id": "email_log_id2",
    "success": false,
    "email": "email6"
  }
}
```

