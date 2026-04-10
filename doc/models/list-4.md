
# List 4

*This model accepts additional fields of type Object.*

## Structure

`List4`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `LocationId` | `String` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `TerminalId` | `String` | Optional | Terminal ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getTerminalId() | setTerminalId(String terminalId) |
| `RequireSignature` | `Boolean` | Optional | Set to true or 1 to require a signature from the customer | Boolean getRequireSignature() | setRequireSignature(Boolean requireSignature) |
| `DeviceTermApiId` | `String` | Optional | Can be used for associating record to external systems. Must be unique per location.<br><br>**Constraints**: *Maximum Length*: `64` | String getDeviceTermApiId() | setDeviceTermApiId(String deviceTermApiId) |
| `TermsConditions` | `String` | Optional | This is the message that is displayed on the screen when prompting for a signature.<br><br>**Constraints**: *Maximum Length*: `4096` | String getTermsConditions() | setTermsConditions(String termsConditions) |
| `Id` | `String` | Optional | Device term ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `ReasonCodeId` | `Integer` | Optional | Reason code ID | Integer getReasonCodeId() | setReasonCodeId(Integer reasonCodeId) |
| `Signature` | [`Signature1`](../../doc/models/signature-1.md) | Optional | - | Signature1 getSignature() | setSignature(Signature1 signature) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `CreatedUserId` | `String` | Optional | System generated id for user who created record<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `CreatedUser` | [`User9`](../../doc/models/user-9.md) | Optional | - | User9 getCreatedUser() | setCreatedUser(User9 createdUser) |
| `Location` | [`Location18`](../../doc/models/location-18.md) | Optional | - | Location18 getLocation() | setLocation(Location18 location) |
| `Terminal` | [`Terminal2`](../../doc/models/terminal-2.md) | Optional | - | Terminal2 getTerminal() | setTerminal(Terminal2 terminal) |
| `Changelogs` | [`List<Changelog>`](../../doc/models/changelog.md) | Optional | Changelog Information on `expand` | List<Changelog> getChangelogs() | setChangelogs(List<Changelog> changelogs) |
| `ReasonCode` | [`ReasonCode1`](../../doc/models/reason-code-1.md) | Optional | - | ReasonCode1 getReasonCode() | setReasonCode(ReasonCode1 reasonCode) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "terminal_id": "11e95f8ec39de8fbdb0a4f1a",
  "require_signature": true,
  "device_term_api_id": "device_term134",
  "terms_conditions": "FUNgib0Vh0B9c0Wbttvr50vNtGLOkTdFL0eFmhN1RJpKhK14IENeDa8irp2dEk9thEcVHvVEyriQeZLs5NjNsCzqNj9JDA4RSJwK647IFtYjrNPN1nBb9bw6hoQ71oT5kpsiXGt8HcqBFVBVeDA7psIzKAyDveAw2o1hfjipkOtXrPgWun0rYwyyFuvqkT1egQYKfYDj",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "reason_code_id": 1000,
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

