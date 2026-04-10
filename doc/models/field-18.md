
# Field 18

*This model accepts additional fields of type Object.*

## Structure

`Field18`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `String` | Optional | id | String getId() | setId(String id) |
| `Label` | `String` | Optional | Label | String getLabel() | setLabel(String label) |
| `FieldType` | `String` | Optional | Field Type | String getFieldType() | setFieldType(String fieldType) |
| `Position` | `List<String>` | Optional | Position<br><br>**Constraints**: *Minimum Items*: `1` | List<String> getPosition() | setPosition(List<String> position) |
| `Required` | `Boolean` | Optional | Required | Boolean getRequired() | setRequired(Boolean required) |
| `Readonly` | `Boolean` | Optional | Read Only | Boolean getReadonly() | setReadonly(Boolean readonly) |
| `Visible` | `Boolean` | Optional | Visible | Boolean getVisible() | setVisible(Boolean visible) |
| `Value` | `String` | Optional | Value | String getValue() | setValue(String value) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "id": "transaction_amount",
  "label": "Header",
  "field_type": "heading",
  "position": [
    "1",
    "0",
    "1",
    "1"
  ],
  "required": true,
  "readonly": true,
  "visible": true,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

