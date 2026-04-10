
# Conditions

*This model accepts additional fields of type Object.*

## Structure

`Conditions`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Method` | [`Method`](../../doc/models/method.md) | Optional | - | Method getMethod() | setMethod(Method method) |
| `Values` | [`Values`](../../doc/models/values.md) | Optional | - | Values getValues() | setValues(Values values) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "method": "xor",
  "values": "account_vault_id",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

