
# Conditions 42

*This model accepts additional fields of type Object.*

## Structure

`Conditions42`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Method` | [`Method5`](../../doc/models/method-5.md) | Optional | - | Method5 getMethod() | setMethod(Method5 method) |
| `Values` | [`Values6`](../../doc/models/values-6.md) | Optional | - | Values6 getValues() | setValues(Values6 values) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "method": "oxor",
  "values": "accountvault_c2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

