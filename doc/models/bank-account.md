
# Bank Account

The Bank Account.

*This model accepts additional fields of type Object.*

## Structure

`BankAccount`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RoutingNumber` | `String` | Optional | Nine-digit Bank routing number.<br><br>**Constraints**: *Maximum Length*: `9` | String getRoutingNumber() | setRoutingNumber(String routingNumber) |
| `AccountNumber` | `String` | Optional | Bank account number.<br><br>**Constraints**: *Maximum Length*: `17` | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `AccountHolderName` | `String` | Optional | Name on bank account.<br><br>**Constraints**: *Maximum Length*: `40` | String getAccountHolderName() | setAccountHolderName(String accountHolderName) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "routing_number": "011103093",
  "account_number": "01234567890123",
  "account_holder_name": "Bob Fairview",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

