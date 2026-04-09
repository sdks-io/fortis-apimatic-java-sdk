
# Changelog

## Structure

`Changelog`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `String` | Optional | Change Log ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `Action` | `String` | Optional | Action<br><br>**Constraints**: *Maximum Length*: `255` | String getAction() | setAction(String action) |
| `Model` | `String` | Optional | Model<br><br>**Constraints**: *Maximum Length*: `255` | String getModel() | setModel(String model) |
| `ModelId` | `String` | Optional | Model ID<br><br>**Constraints**: *Maximum Length*: `255` | String getModelId() | setModelId(String modelId) |
| `UserId` | `String` | Optional | User ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getUserId() | setUserId(String userId) |
| `ChangelogDetails` | [`List<ChangelogDetail>`](../../doc/models/changelog-detail.md) | Optional | Change Log Details | List<ChangelogDetail> getChangelogDetails() | setChangelogDetails(List<ChangelogDetail> changelogDetails) |
| `User` | [`User`](../../doc/models/user.md) | Optional | User | User getUser() | setUser(User user) |

## Example (as JSON)

```json
{
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "action": "CREATE",
  "model": "TransactionRequest",
  "model_id": "11ec829598f0d4008be9aba4",
  "user_id": "11e95f8ec39de8fbdb0a4f1a"
}
```

