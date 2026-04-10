
# Order 21

*This model accepts additional fields of type Object.*

## Structure

`Order21`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Key` | `String` | Required | Resource key to order by. | String getKey() | setKey(String key) |
| `Operator` | [`Operator`](../../doc/models/operator.md) | Required | - | Operator getOperator() | setOperator(Operator operator) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "key": "first_name",
  "operator": "asc",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

