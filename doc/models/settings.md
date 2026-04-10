
# Settings

*This model accepts additional fields of type Object.*

## Structure

`Settings`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Enabled` | `Boolean` | Optional | Enabled | Boolean getEnabled() | setEnabled(Boolean enabled) |
| `Columns` | `Double` | Optional | Columns | Double getColumns() | setColumns(Double columns) |
| `Rows` | `Double` | Optional | Rows | Double getRows() | setRows(Double rows) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "enabled": true,
  "columns": 1.0,
  "rows": 1.0,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

