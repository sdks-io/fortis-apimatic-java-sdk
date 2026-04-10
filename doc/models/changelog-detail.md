
# Changelog Detail

*This model accepts additional fields of type Object.*

## Structure

`ChangelogDetail`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `String` | Optional | ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `ChangelogId` | `String` | Optional | Changelog ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getChangelogId() | setChangelogId(String changelogId) |
| `Field` | `String` | Optional | Field | String getField() | setField(String field) |
| `OldValue` | `String` | Optional | Old Value | String getOldValue() | setOldValue(String oldValue) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "changelog_id": "11e95f8ec39de8fbdb0a4f1a",
  "field": "next_run_ts",
  "old_value": "1643616000",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

