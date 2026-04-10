
# Joi 4

*This model accepts additional fields of type Object.*

## Structure

`Joi4`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Conditions` | [`Joi4Conditions`](../../doc/models/containers/joi-4-conditions.md) | Optional | This is a container for any-of cases. | Joi4Conditions getConditions() | setConditions(Joi4Conditions conditions) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "conditions": {
    "method": "oxor",
    "values": "token_api_id",
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

