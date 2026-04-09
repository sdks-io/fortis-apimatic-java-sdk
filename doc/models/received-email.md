
# Received Email

## Structure

`ReceivedEmail`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Subject` | `String` | Optional | Subject<br><br>**Constraints**: *Maximum Length*: `256` | String getSubject() | setSubject(String subject) |
| `Body` | `String` | Optional | Body | String getBody() | setBody(String body) |
| `SourceAddress` | `String` | Optional | Source Address<br><br>**Constraints**: *Maximum Length*: `64` | String getSourceAddress() | setSourceAddress(String sourceAddress) |
| `ReturnPath` | `String` | Optional | Return Path<br><br>**Constraints**: *Maximum Length*: `64` | String getReturnPath() | setReturnPath(String returnPath) |
| `ProviderId` | `String` | Optional | Provider<br><br>**Constraints**: *Maximum Length*: `60` | String getProviderId() | setProviderId(String providerId) |
| `DomainId` | `String` | Optional | Domain<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getDomainId() | setDomainId(String domainId) |
| `ReasonSent` | `String` | Optional | Reason Sent<br><br>**Constraints**: *Maximum Length*: `36` | String getReasonSent() | setReasonSent(String reasonSent) |
| `ReasonModel` | [`ReasonModelEnum`](../../doc/models/reason-model-enum.md) | Optional | Reason Model<br><br>**Constraints**: *Maximum Length*: `64` | ReasonModelEnum getReasonModel() | setReasonModel(ReasonModelEnum reasonModel) |
| `ReasonModelId` | `String` | Optional | Reason Model<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getReasonModelId() | setReasonModelId(String reasonModelId) |
| `ReplyTo` | `String` | Optional | Reply To<br><br>**Constraints**: *Maximum Length*: `520` | String getReplyTo() | setReplyTo(String replyTo) |
| `Id` | `String` | Optional | Log Email Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |

## Example (as JSON)

```json
{
  "subject": "Payment Receipt - 12skiestech",
  "body": "This email is being sent from a server.",
  "source_address": "\"12skiestech A7t3qi\" <noreply@zeamster.email>",
  "return_path": "\"12skiestech A7t3qi\" <noreply@zeamster.email>",
  "provider_id": "0100017e67bcc530-e1dd23b4-8a39-4a5b-8d5d-68d51c4c942f-000000",
  "domain_id": "11e95f8ec39de8fbdb0a4f1a",
  "reason_sent": "Contact Email",
  "reason_model": "Transaction",
  "reason_model_id": "11e95f8ec39de8fbdb0a4f1a",
  "reply_to": "\"Zeamster\" <emma.p@zeamster.com>",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992
}
```

