
# Response Transaction

## Structure

`ResponseTransaction`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type110Enum`](../../doc/models/type-110-enum.md) | Optional | Resource Type<br><br>**Default**: `Type110Enum.TRANSACTION` | Type110Enum getType() | setType(Type110Enum type) |
| `Data` | [`Data27`](../../doc/models/data-27.md) | Optional | - | Data27 getData() | setData(Data27 data) |

## Example (as JSON)

```json
{
  "type": "Transaction",
  "data": {
    "additional_amounts": [
      {
        "type": "cashback",
        "amount": 6,
        "account_type": "cash_benefit",
        "currency": 154.64
      },
      {
        "type": "cashback",
        "amount": 6,
        "account_type": "cash_benefit",
        "currency": 154.64
      }
    ],
    "billing_address": {
      "city": "city2",
      "state": "state6",
      "postal_code": "postal_code0",
      "street": "street8",
      "phone": "phone2"
    },
    "checkin_date": "checkin_date2",
    "checkout_date": "checkout_date4",
    "clerk_number": "clerk_number4"
  }
}
```

