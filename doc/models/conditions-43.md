
# Conditions 43

*This model accepts additional fields of type Object.*

## Structure

`Conditions43`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Method` | [`Method5`](../../doc/models/method-5.md) | Optional | - | Method5 getMethod() | setMethod(Method5 method) |
| `Values` | [`Values7`](../../doc/models/values-7.md) | Optional | - | Values7 getValues() | setValues(Values7 values) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "method": "oxor",
  "values": "accountvault_c3",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

