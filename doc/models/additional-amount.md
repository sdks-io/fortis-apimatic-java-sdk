
# Additional Amount

*This model accepts additional fields of type Object.*

## Structure

`AdditionalAmount`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | `Object` | Optional | - | Object getType() | setType(Object type) |
| `Amount` | `Integer` | Optional | The amount of additional amount. | Integer getAmount() | setAmount(Integer amount) |
| `AccountType` | `Object` | Optional | - | Object getAccountType() | setAccountType(Object accountType) |
| `Currency` | `Double` | Optional | Currency Code | Double getCurrency() | setCurrency(Double currency) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "amount": 10,
  "currency": 840.0,
  "type": {
    "key1": "val1",
    "key2": "val2"
  },
  "account_type": {
    "key1": "val1",
    "key2": "val2"
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

