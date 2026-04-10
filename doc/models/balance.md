
# Balance

*This model accepts additional fields of type Object.*

## Structure

`Balance`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AmountType` | `String` | Optional | The type of amount balance | String getAmountType() | setAmountType(String amountType) |
| `AccountType` | `String` | Optional | The type of account balance | String getAccountType() | setAccountType(String accountType) |
| `Amount` | `Integer` | Optional | The amount of balance | Integer getAmount() | setAmount(Integer amount) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "amount": 1000,
  "amount_type": "amount_type4",
  "account_type": "account_type6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

