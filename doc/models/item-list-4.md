
# Item List 4

## Structure

`ItemList4`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Name` | `String` | Required | Item's Name, must be unique on the list<br><br>**Constraints**: *Maximum Length*: `100` | String getName() | setName(String name) |
| `Amount` | `int` | Required | Item's Amount<br><br>**Constraints**: `>= -999999999`, `<= 999999999` | int getAmount() | setAmount(int amount) |

## Example (as JSON)

```json
{
  "name": "Bread",
  "amount": 2015
}
```

