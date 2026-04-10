
# Conditions 191

*This model accepts additional fields of type Object.*

## Structure

`Conditions191`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Method` | [`Method53`](../../doc/models/method-53.md) | Optional | - | Method53 getMethod() | setMethod(Method53 method) |
| `Values` | [`Values58`](../../doc/models/values-58.md) | Optional | - | Values58 getValues() | setValues(Values58 values) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "method": "and",
  "values": "account_number",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

