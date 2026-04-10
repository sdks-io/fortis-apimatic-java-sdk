
# Postback Log

*This model accepts additional fields of type Object.*

## Structure

`PostbackLog`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PostbackStatusId` | `Object` | Optional | - | Object getPostbackStatusId() | setPostbackStatusId(Object postbackStatusId) |
| `Id` | `String` | Optional | Postback Log Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `PostbackConfigId` | `String` | Optional | Postback Config Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getPostbackConfigId() | setPostbackConfigId(String postbackConfigId) |
| `ChangelogId` | `String` | Optional | Changelog Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getChangelogId() | setChangelogId(String changelogId) |
| `HttpVerb` | `String` | Optional | Http Verb | String getHttpVerb() | setHttpVerb(String httpVerb) |
| `NextRunTs` | `Integer` | Optional | Next Run | Integer getNextRunTs() | setNextRunTs(Integer nextRunTs) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `Model` | `String` | Optional | MOdel | String getModel() | setModel(String model) |
| `ModelId` | `String` | Optional | Model Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getModelId() | setModelId(String modelId) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "postback_config_id": "11e95f8ec39de8fbdb0a4f1a",
  "changelog_id": "11e95f8ec39de8fbdb0a4f1a",
  "next_run_ts": 1422040992,
  "created_ts": 1422040992,
  "model_id": "11e95f8ec39de8fbdb0a4f1a",
  "postback_status_id": {
    "key1": "val1",
    "key2": "val2"
  },
  "http_verb": "http_verb8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

