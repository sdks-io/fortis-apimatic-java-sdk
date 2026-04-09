
# Joi 19

## Structure

`Joi19`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Conditions` | [`Joi19Conditions`](../../doc/models/containers/joi-19-conditions.md) | Optional | This is a container for any-of cases. | Joi19Conditions getConditions() | setConditions(Joi19Conditions conditions) |

## Example (as JSON)

```json
{
  "conditions": {
    "method": "xor",
    "values": "account_number"
  }
}
```

