
# Data 19

*This model accepts additional fields of type Object.*

## Structure

`Data19`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `String` | Optional | Quick Invoice ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `EmailLogId` | `String` | Optional | Email Log Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getEmailLogId() | setEmailLogId(String emailLogId) |
| `SmsLogId` | `String` | Optional | SMS Log Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getSmsLogId() | setSmsLogId(String smsLogId) |
| `Success` | `Boolean` | Optional | Success | Boolean getSuccess() | setSuccess(Boolean success) |
| `SmsSuccess` | `Boolean` | Optional | SMS Success | Boolean getSmsSuccess() | setSmsSuccess(Boolean smsSuccess) |
| `Email` | `String` | Optional | Email<br><br>**Constraints**: *Maximum Length*: `64` | String getEmail() | setEmail(String email) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "email_log_id": "11e95f8ec39de8fbdb0a4f1a",
  "sms_log_id": "11e95f8ec39de8fbdb0a4f1a",
  "success": true,
  "sms_success": true,
  "email": "email@domain.com",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

