
# Conditions 27

*This model accepts additional fields of type Object.*

## Structure

`Conditions27`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Method` | [`Method`](../../doc/models/method.md) | Optional | - | Method getMethod() | setMethod(Method method) |
| `Values` | [`Values99`](../../doc/models/values-99.md) | Optional | - | Values99 getValues() | setValues(Values99 values) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "method": "xor",
  "values": "previous_transaction_id",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

