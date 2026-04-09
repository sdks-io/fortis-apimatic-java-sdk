
# Field

## Structure

`Field`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Field` | `String` | Optional | Field name used on the sort | String getField() | setField(String field) |
| `Order` | [`OrderEnum`](../../doc/models/order-enum.md) | Optional | Sort direction ASC/DESC | OrderEnum getOrder() | setOrder(OrderEnum order) |

## Example (as JSON)

```json
{
  "field": "last_name",
  "order": "asc"
}
```

