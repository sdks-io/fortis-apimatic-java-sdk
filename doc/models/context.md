
# Context

*This model accepts additional fields of type Object.*

## Structure

`Context`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Key` | `String` | Optional | - | String getKey() | setKey(String key) |
| `Label` | `String` | Optional | - | String getLabel() | setLabel(String label) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "key": "fieldName",
  "label": "fieldName",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

