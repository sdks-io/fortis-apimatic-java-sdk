
# Joi

*This model accepts additional fields of type Object.*

## Structure

`Joi`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Conditions` | [`Conditions`](../../doc/models/conditions.md) | Optional | - | Conditions getConditions() | setConditions(Conditions conditions) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "conditions": {
    "method": "xor",
    "values": "account_vault_api_id",
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

