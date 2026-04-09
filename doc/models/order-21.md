
# Order 21

## Structure

`Order21`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Key` | `String` | Required | Resource key to order by. | String getKey() | setKey(String key) |
| `Operator` | [`OperatorEnum`](../../doc/models/operator-enum.md) | Required | The order. Ascending or descending. | OperatorEnum getOperator() | setOperator(OperatorEnum operator) |

## Example (as JSON)

```json
{
  "key": "first_name",
  "operator": "asc"
}
```

