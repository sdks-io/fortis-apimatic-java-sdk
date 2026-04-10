
# Terminal Cvm 1

*This model accepts additional fields of type Object.*

## Structure

`TerminalCvm1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TerminalManufacturerCode` | `Double` | Optional | Terminal Manufacturer Code | Double getTerminalManufacturerCode() | setTerminalManufacturerCode(Double terminalManufacturerCode) |
| `Title` | `String` | Optional | Title<br><br>**Constraints**: *Maximum Length*: `32` | String getTitle() | setTitle(String title) |
| `ContactData` | `String` | Optional | Contact Data<br><br>**Constraints**: *Maximum Length*: `100000` | String getContactData() | setContactData(String contactData) |
| `ContactlessData` | `String` | Optional | Contactless Data<br><br>**Constraints**: *Maximum Length*: `100000` | String getContactlessData() | setContactlessData(String contactlessData) |
| `Id` | `String` | Optional | Terminal Manufacturer Cvms Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `ModifiedUserId` | `String` | Optional | Last User ID that updated the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getModifiedUserId() | setModifiedUserId(String modifiedUserId) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "terminal_manufacturer_code": 4.0,
  "title": "CVM One",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "modified_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "contact_data": "contact_data6",
  "contactless_data": "contactless_data8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

