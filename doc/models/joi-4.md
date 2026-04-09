
# Joi 4

## Structure

`Joi4`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Conditions` | [`Joi4Conditions`](../../doc/models/containers/joi-4-conditions.md) | Optional | This is a container for any-of cases. | Joi4Conditions getConditions() | setConditions(Joi4Conditions conditions) |

## Example (as JSON)

```json
{
  "conditions": {
    "method": "oxor",
    "values": "token_api_id"
  }
}
```

