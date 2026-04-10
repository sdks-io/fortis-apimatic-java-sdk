
# Item List

*This model accepts additional fields of type Object.*

## Structure

`ItemList`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Name` | `String` | Optional | Item's Name, must be unique on the list<br><br>**Constraints**: *Maximum Length*: `100` | String getName() | setName(String name) |
| `Amount` | `Integer` | Optional | Item's Amount<br><br>**Constraints**: `>= -999999999`, `<= 999999999` | Integer getAmount() | setAmount(Integer amount) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "name": "Bread",
  "amount": 2015,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

