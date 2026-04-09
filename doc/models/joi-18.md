
# Joi 18

## Structure

`Joi18`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Conditions` | [`Joi18Conditions`](../../doc/models/containers/joi-18-conditions.md) | Optional | This is a container for any-of cases. | Joi18Conditions getConditions() | setConditions(Joi18Conditions conditions) |

## Example (as JSON)

```json
{
  "conditions": {
    "method": "xor",
    "values": "account_number"
  }
}
```

