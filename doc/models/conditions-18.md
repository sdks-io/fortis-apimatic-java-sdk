
# Conditions 18

*This model accepts additional fields of type Object.*

## Structure

`Conditions18`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Method` | [`Method`](../../doc/models/method.md) | Optional | - | Method getMethod() | setMethod(Method method) |
| `Values` | [`Values50`](../../doc/models/values-50.md) | Optional | - | Values50 getValues() | setValues(Values50 values) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "method": "xor",
  "values": "account_number",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

