
# Additional Amount

## Structure

`AdditionalAmount`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type60Enum`](../../doc/models/type-60-enum.md) | Optional | type of the amount [4S-Healthcare(Visa and MC Only), 4U-Prescription/Rx(Visa and MC Only), 4V-Vision/Optical(Visa Only), 4W-clinic/other qualified medical(Visa Only) ,4X-Dental(Visa Only)]. | Type60Enum getType() | setType(Type60Enum type) |
| `Amount` | `Integer` | Optional | The amount of additional amount. | Integer getAmount() | setAmount(Integer amount) |
| `AccountType` | [`AccountTypeEnum`](../../doc/models/account-type-enum.md) | Optional | Account Type | AccountTypeEnum getAccountType() | setAccountType(AccountTypeEnum accountType) |
| `Currency` | `Double` | Optional | Currency Code | Double getCurrency() | setCurrency(Double currency) |

## Example (as JSON)

```json
{
  "type": "cashback",
  "amount": 10,
  "account_type": "credit",
  "currency": 840.0
}
```

