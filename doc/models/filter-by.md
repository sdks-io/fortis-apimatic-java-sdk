
# Filter By

*This model accepts additional fields of type Object.*

## Structure

`FilterBy`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Key` | `String` | Required | Resource key to filter by | String getKey() | setKey(String key) |
| `Operator` | [`FilterByOperator`](../../doc/models/containers/filter-by-operator.md) | Required | This is a container for one-of cases. | FilterByOperator getOperator() | setOperator(FilterByOperator operator) |
| `Value` | [`FilterByValue`](../../doc/models/containers/filter-by-value.md) | Required | This is a container for one-of cases. | FilterByValue getValue() | setValue(FilterByValue value) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "key": "first_name",
  "operator": "<=",
  "value": "Fred",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

