
# Product Recurring

Product recurring array

## Structure

`ProductRecurring`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Title` | `String` | Optional | Title<br><br>**Constraints**: *Maximum Length*: `64` | String getTitle() | setTitle(String title) |
| `LocationId` | `String` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `LocationApiId` | `String` | Optional | Location Api ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationApiId() | setLocationApiId(String locationApiId) |
| `SendDeclinedNotifications` | `Boolean` | Optional | Send Declined Notifications | Boolean getSendDeclinedNotifications() | setSendDeclinedNotifications(Boolean sendDeclinedNotifications) |
| `RequireFullPayment` | `Boolean` | Optional | Require Full Payment | Boolean getRequireFullPayment() | setRequireFullPayment(Boolean requireFullPayment) |
| `ExpireNotificationEmailEnable` | `Boolean` | Optional | Expire Notification Email Enable | Boolean getExpireNotificationEmailEnable() | setExpireNotificationEmailEnable(Boolean expireNotificationEmailEnable) |
| `ExpireNotificationSmsEnable` | `Boolean` | Optional | Expire Notification SMS Enable | Boolean getExpireNotificationSmsEnable() | setExpireNotificationSmsEnable(Boolean expireNotificationSmsEnable) |
| `NotificationDaysDefault` | `Integer` | Optional | Notification Days Default<br><br>**Constraints**: `>= 0`, `<= 365` | Integer getNotificationDaysDefault() | setNotificationDaysDefault(Integer notificationDaysDefault) |
| `Id` | `String` | Optional | Product Recurring Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `CreatedUserId` | `String` | Optional | Created User Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `ModifiedUserId` | `String` | Optional | Modified User Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getModifiedUserId() | setModifiedUserId(String modifiedUserId) |

## Example (as JSON)

```json
{
  "title": "Fortispay RbYN6y",
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "location_api_id": "11e95f8ec39de8fbdb0a4f1a",
  "send_declined_notifications": true,
  "require_full_payment": true,
  "expire_notification_email_enable": true,
  "expire_notification_sms_enable": true,
  "notification_days_default": 1,
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "modified_user_id": "11e95f8ec39de8fbdb0a4f1a"
}
```

