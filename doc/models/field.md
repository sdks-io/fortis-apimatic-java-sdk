
# Field

*This model accepts additional fields of type Object.*

## Structure

`Field`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Field` | `String` | Optional | Field name used on the sort | String getField() | setField(String field) |
| `Order` | [`Order`](../../doc/models/order.md) | Optional | - | Order getOrder() | setOrder(Order order) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "field": "last_name",
  "order": "asc",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

