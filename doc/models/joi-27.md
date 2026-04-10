
# Joi 27

*This model accepts additional fields of type Object.*

## Structure

`Joi27`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Conditions` | [`Conditions27`](../../doc/models/conditions-27.md) | Optional | - | Conditions27 getConditions() | setConditions(Conditions27 conditions) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "conditions": {
    "method": "xor",
    "values": "previous_transaction_id",
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

