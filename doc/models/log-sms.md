
# Log Sms

Log Sms Information on `expand`

## Structure

`LogSms`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `String` | Optional | Log Sms Id<br><br>**Constraints**: *Maximum Length*: `24`, *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `Body` | `String` | Optional | Body | String getBody() | setBody(String body) |
| `ReasonModel` | `String` | Optional | Reason Model<br><br>**Constraints**: *Maximum Length*: `24` | String getReasonModel() | setReasonModel(String reasonModel) |
| `ReasonModelId` | `String` | Optional | Reason Model ID<br><br>**Constraints**: *Maximum Length*: `36` | String getReasonModelId() | setReasonModelId(String reasonModelId) |
| `ProviderId` | `String` | Optional | Provider ID<br><br>**Constraints**: *Maximum Length*: `60` | String getProviderId() | setProviderId(String providerId) |
| `Status` | `String` | Optional | Status<br><br>**Constraints**: *Maximum Length*: `10` | String getStatus() | setStatus(String status) |
| `Sender` | `String` | Optional | Sender<br><br>**Constraints**: *Maximum Length*: `10` | String getSender() | setSender(String sender) |
| `Recipient` | `String` | Optional | Recipient<br><br>**Constraints**: *Maximum Length*: `10` | String getRecipient() | setRecipient(String recipient) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Maximum Length*: `36`, *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |

## Example (as JSON)

```json
{
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "body": "body2",
  "reason_model": "reason_model2",
  "reason_model_id": "reason_model_id8",
  "provider_id": "provider_id8"
}
```

