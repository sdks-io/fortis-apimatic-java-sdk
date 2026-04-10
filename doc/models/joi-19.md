
# Joi 19

*This model accepts additional fields of type Object.*

## Structure

`Joi19`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Conditions` | [`Joi19Conditions`](../../doc/models/containers/joi-19-conditions.md) | Optional | This is a container for any-of cases. | Joi19Conditions getConditions() | setConditions(Joi19Conditions conditions) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "conditions": {
    "method": "xor",
    "values": "account_number",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

