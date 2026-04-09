
# Bank Account 1

Array of bank account objects.

> One account with “deposit_type” of primary is required. Maximum of two accounts are allowed.

## Structure

`BankAccount1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AccountHolderName` | `String` | Required | Account holder name.<br><br>**Constraints**: *Maximum Length*: `40` | String getAccountHolderName() | setAccountHolderName(String accountHolderName) |
| `RoutingNumber` | `String` | Required | Nine-digit Bank routing number.<br><br>**Constraints**: *Maximum Length*: `9` | String getRoutingNumber() | setRoutingNumber(String routingNumber) |
| `AccountNumber` | `String` | Required | Account number.<br><br>**Constraints**: *Maximum Length*: `17` | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `IsPrimary` | `Boolean` | Optional | Flag indicating whether or not the account is the primary account. Only one account can be marked as primary.<br><br>> Indicates that the account should be the primary account for the merchant. One and only one account may be set to true. | Boolean getIsPrimary() | setIsPrimary(Boolean isPrimary) |
| `AccountType` | [`AccountType12Enum`](../../doc/models/account-type-12-enum.md) | Required | Account type. Either "checking" or "savings"<br><br>**Constraints**: *Maximum Length*: `10` | AccountType12Enum getAccountType() | setAccountType(AccountType12Enum accountType) |
| `AltDepositTypes` | `List<String>` | Optional | Array of deposit types. ('fees', 'adjustments', 'returns') | List<String> getAltDepositTypes() | setAltDepositTypes(List<String> altDepositTypes) |

## Example (as JSON)

```json
{
  "account_holder_name": "James Bond",
  "routing_number": "111111111",
  "account_number": "1234567",
  "is_primary": true,
  "account_type": "checking",
  "alt_deposit_types": [
    "alt_deposit_types0",
    "alt_deposit_types9"
  ]
}
```

