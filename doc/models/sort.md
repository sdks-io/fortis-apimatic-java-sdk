
# Sort

Sort information used on the results

*This model accepts additional fields of type Object.*

## Structure

`Sort`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type4`](../../doc/models/type-4.md) | Optional | - | Type4 getType() | setType(Type4 type) |
| `Fields` | [`List<Field>`](../../doc/models/field.md) | Optional | [object Object] | List<Field> getFields() | setFields(List<Field> fields) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "Sorting",
  "fields": [
    {
      "field": "field2",
      "order": "asc",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "field": "field2",
      "order": "asc",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

