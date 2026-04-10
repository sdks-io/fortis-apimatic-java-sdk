
# Tip Percents 1

*This model accepts additional fields of type Object.*

## Structure

`TipPercents1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Percent1` | `Integer` | Optional | field can only contain a value from 0 to 99, if 1 field is NULL, all fields must be null.<br><br>**Constraints**: `>= 0`, `<= 99` | Integer getPercent1() | setPercent1(Integer percent1) |
| `Percent2` | `Integer` | Optional | field can only contain a value from 0 to 99, if 1 field is NULL, all fields must be null.<br><br>**Constraints**: `>= 0`, `<= 99` | Integer getPercent2() | setPercent2(Integer percent2) |
| `Percent3` | `Integer` | Optional | field can only contain a value from 0 to 99, if 1 field is NULL, all fields must be null.<br><br>**Constraints**: `>= 0`, `<= 99` | Integer getPercent3() | setPercent3(Integer percent3) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "percent_1": 0,
  "percent_2": 2,
  "percent_3": 99,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

