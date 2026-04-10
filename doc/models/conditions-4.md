
# Conditions 4

*This model accepts additional fields of type Object.*

## Structure

`Conditions4`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Method` | [`Method5`](../../doc/models/method-5.md) | Optional | - | Method5 getMethod() | setMethod(Method5 method) |
| `Values` | [`Values4`](../../doc/models/values-4.md) | Optional | - | Values4 getValues() | setValues(Values4 values) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "method": "oxor",
  "values": "token_api_id",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

