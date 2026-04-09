
# Active Notification Alert

## Structure

`ActiveNotificationAlert`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `LocationId` | `String` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `LocationApiId` | `String` | Optional | Location Api ID | String getLocationApiId() | setLocationApiId(String locationApiId) |
| `DateStart` | `String` | Optional | Date Start<br><br>**Constraints**: *Maximum Length*: `19`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}\s[\d]{2}:[\d]{2}:[\d]{2}$` | String getDateStart() | setDateStart(String dateStart) |
| `DateEnd` | `String` | Optional | Date End<br><br>**Constraints**: *Maximum Length*: `19`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}\s[\d]{2}:[\d]{2}:[\d]{2}$` | String getDateEnd() | setDateEnd(String dateEnd) |
| `UserLocation` | `Boolean` | Optional | User Location | Boolean getUserLocation() | setUserLocation(Boolean userLocation) |
| `UserContact` | `Boolean` | Optional | User Contact | Boolean getUserContact() | setUserContact(Boolean userContact) |
| `IncludeChildren` | `Boolean` | Optional | Include Children | Boolean getIncludeChildren() | setIncludeChildren(Boolean includeChildren) |
| `AlertType` | [`AlertTypeEnum`](../../doc/models/alert-type-enum.md) | Optional | Alert Type | AlertTypeEnum getAlertType() | setAlertType(AlertTypeEnum alertType) |
| `AlertTypeId` | [`AlertTypeIdEnum`](../../doc/models/alert-type-id-enum.md) | Optional | Alert Type ID | AlertTypeIdEnum getAlertTypeId() | setAlertTypeId(AlertTypeIdEnum alertTypeId) |
| `Description` | `String` | Optional | Description<br><br>**Constraints**: *Maximum Length*: `32` | String getDescription() | setDescription(String description) |
| `AlertMessage` | `String` | Optional | Alert Message | String getAlertMessage() | setAlertMessage(String alertMessage) |
| `Id` | `String` | Optional | Notification Alert ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `ModifiedUserId` | `String` | Optional | Last User ID that updated the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getModifiedUserId() | setModifiedUserId(String modifiedUserId) |

## Example (as JSON)

```json
{
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "date_start": "2021-12-01 10:10:00",
  "date_end": "2021-12-01 10:10:00",
  "user_location": true,
  "user_contact": true,
  "include_children": true,
  "alert_type": 1,
  "alert_type_id": 1,
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "modified_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "location_api_id": "location_api_id4"
}
```

