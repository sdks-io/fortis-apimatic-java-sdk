
# Conditions 181

*This model accepts additional fields of type Object.*

## Structure

`Conditions181`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Method` | [`Method53`](../../doc/models/method-53.md) | Optional | - | Method53 getMethod() | setMethod(Method53 method) |
| `Values` | [`Values51`](../../doc/models/values-51.md) | Optional | - | Values51 getValues() | setValues(Values51 values) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "method": "and",
  "values": "routing_number",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

