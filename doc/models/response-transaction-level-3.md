
# Response Transaction Level 3

## Structure

`ResponseTransactionLevel3`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type116Enum`](../../doc/models/type-116-enum.md) | Optional | Resource Type<br><br>**Default**: `Type116Enum.TRANSACTIONLEVEL3` | Type116Enum getType() | setType(Type116Enum type) |
| `Data` | [`Data29`](../../doc/models/data-29.md) | Optional | - | Data29 getData() | setData(Data29 data) |

## Example (as JSON)

```json
{
  "type": "TransactionLevel3",
  "data": {
    "id": "id0",
    "transaction_id": "transaction_id8",
    "level3_data": {
      "destination_country_code": "destination_country_code4",
      "duty_amount": 182,
      "freight_amount": 60,
      "national_tax": 999999998900,
      "sales_tax": 999999998900
    }
  }
}
```

