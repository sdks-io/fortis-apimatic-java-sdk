
# Sort

Sort information used on the results

## Structure

`Sort`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type4Enum`](../../doc/models/type-4-enum.md) | Optional | Object type | Type4Enum getType() | setType(Type4Enum type) |
| `Fields` | [`List<Field>`](../../doc/models/field.md) | Optional | [object Object] | List<Field> getFields() | setFields(List<Field> fields) |

## Example (as JSON)

```json
{
  "type": "Sorting",
  "fields": [
    {
      "field": "field2",
      "order": "asc"
    },
    {
      "field": "field2",
      "order": "asc"
    }
  ]
}
```

