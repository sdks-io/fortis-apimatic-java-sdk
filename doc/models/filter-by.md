
# Filter By

## Structure

`FilterBy`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Key` | `String` | Required | Resource key to filter by | String getKey() | setKey(String key) |
| `Operator` | [`FilterByOperator`](../../doc/models/containers/filter-by-operator.md) | Required | This is a container for one-of cases. | FilterByOperator getOperator() | setOperator(FilterByOperator operator) |
| `Value` | [`FilterByValue`](../../doc/models/containers/filter-by-value.md) | Required | This is a container for one-of cases. | FilterByValue getValue() | setValue(FilterByValue value) |

## Example (as JSON)

```json
{
  "key": "first_name",
  "operator": "<=",
  "value": "Fred"
}
```

