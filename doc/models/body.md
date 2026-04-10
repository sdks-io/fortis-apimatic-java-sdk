
# Body

Body

*This model accepts additional fields of type Object.*

## Structure

`Body`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Settings` | [`Settings`](../../doc/models/settings.md) | Optional | - | Settings getSettings() | setSettings(Settings settings) |
| `Fields` | [`List<Field18>`](../../doc/models/field-18.md) | Optional | - | List<Field18> getFields() | setFields(List<Field18> fields) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "settings": {
    "enabled": false,
    "columns": 202.28,
    "rows": 235.78,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "fields": [
    {
      "id": "id8",
      "label": "label8",
      "field_type": "field_type4",
      "position": [
        "position7",
        "position8",
        "position9"
      ],
      "required": false,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "id": "id8",
      "label": "label8",
      "field_type": "field_type4",
      "position": [
        "position7",
        "position8",
        "position9"
      ],
      "required": false,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "id": "id8",
      "label": "label8",
      "field_type": "field_type4",
      "position": [
        "position7",
        "position8",
        "position9"
      ],
      "required": false,
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

