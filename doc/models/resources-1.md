
# Resources 1

*This model accepts additional fields of type Object.*

## Structure

`Resources1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Title` | `String` | Optional | Resource Title<br><br>**Constraints**: *Maximum Length*: `64` | String getTitle() | setTitle(String title) |
| `Priv` | `String` | Optional | Priv<br><br>**Constraints**: *Maximum Length*: `64` | String getPriv() | setPriv(String priv) |
| `ResourceName` | `String` | Optional | Resource Name<br><br>**Constraints**: *Maximum Length*: `64` | String getResourceName() | setResourceName(String resourceName) |
| `Id` | `Integer` | Optional | Resource ID | Integer getId() | setId(Integer id) |
| `LastUsedDate` | `Integer` | Optional | Last Used Date | Integer getLastUsedDate() | setLastUsedDate(Integer lastUsedDate) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "title": "My terminal",
  "resource_name": "v2.addons.iframe.get",
  "id": 5693,
  "last_used_date": 1422040992,
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "priv": "priv0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

