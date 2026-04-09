
# Item List 5

## Structure

`ItemList5`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Name` | `String` | Optional | Item's Name, must be unique on the list<br><br>**Constraints**: *Maximum Length*: `100` | String getName() | setName(String name) |
| `Amount` | `Integer` | Optional | Item's Amount<br><br>**Constraints**: `>= -999999999`, `<= 999999999` | Integer getAmount() | setAmount(Integer amount) |

## Example (as JSON)

```json
{
  "name": "Bread",
  "amount": 2015
}
```

