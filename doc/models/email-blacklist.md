
# Email Blacklist

Email Blacklist Information on `expand`

## Structure

`EmailBlacklist`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `String` | Optional | Blacklist ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `IsBlacklisted` | `Boolean` | Optional | isBlacklisted | Boolean getIsBlacklisted() | setIsBlacklisted(Boolean isBlacklisted) |
| `Detail` | `Boolean` | Optional | Contact Id | Boolean getDetail() | setDetail(Boolean detail) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |

## Example (as JSON)

```json
{
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "isBlacklisted": true,
  "detail": true,
  "created_ts": 1422040992
}
```

