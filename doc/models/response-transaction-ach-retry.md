
# Response Transaction Ach Retry

## Structure

`ResponseTransactionAchRetry`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type99Enum`](../../doc/models/type-99-enum.md) | Optional | Resource Type<br><br>**Default**: `Type99Enum.TRANSACTIONACHRETRY` | Type99Enum getType() | setType(Type99Enum type) |
| `Data` | [`Data26`](../../doc/models/data-26.md) | Optional | - | Data26 getData() | setData(Data26 data) |

## Example (as JSON)

```json
{
  "type": "TransactionAchRetry",
  "data": {
    "rejected_transaction_id": "rejected_transaction_id4",
    "return_fee": 208,
    "id": "id0",
    "retry_transaction_id": "retry_transaction_id6",
    "return_fee_transaction_id": "return_fee_transaction_id4"
  }
}
```

