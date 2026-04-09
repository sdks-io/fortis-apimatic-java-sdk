
# Hosted Payment Page

Hosted Payment Page Information on `expand`

## Structure

`HostedPaymentPage`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `UserId` | `String` | Optional | User ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getUserId() | setUserId(String userId) |
| `LocationId` | `String` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `LocationApiId` | `String` | Optional | Location Api Id | String getLocationApiId() | setLocationApiId(String locationApiId) |
| `ProductTransactionId` | `String` | Optional | Product Transaction ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getProductTransactionId() | setProductTransactionId(String productTransactionId) |
| `Title` | `String` | Optional | Title<br><br>**Constraints**: *Maximum Length*: `64` | String getTitle() | setTitle(String title) |
| `RedirectUrlDelay` | `Double` | Optional | Redirect Url Delay<br><br>**Default**: `15d`<br><br>**Constraints**: `<= 15` | Double getRedirectUrlDelay() | setRedirectUrlDelay(Double redirectUrlDelay) |
| `MinPaymentAmount` | `Integer` | Optional | Min Payment Amount<br><br>**Constraints**: `>= 0` | Integer getMinPaymentAmount() | setMinPaymentAmount(Integer minPaymentAmount) |
| `MaxPaymentAmount` | `Long` | Optional | Max Payment Amount<br><br>**Default**: `9999999999L`<br><br>**Constraints**: `<= 9999999999` | Long getMaxPaymentAmount() | setMaxPaymentAmount(Long maxPaymentAmount) |
| `RedirectUrlOnApprove` | `String` | Optional | Redirect Url On Approval | String getRedirectUrlOnApprove() | setRedirectUrlOnApprove(String redirectUrlOnApprove) |
| `RedirectUrlOnDecline` | `String` | Optional | Redirect Url On Decline | String getRedirectUrlOnDecline() | setRedirectUrlOnDecline(String redirectUrlOnDecline) |
| `FieldConfiguration` | [`FieldConfiguration`](../../doc/models/field-configuration.md) | Optional | field_configuration | FieldConfiguration getFieldConfiguration() | setFieldConfiguration(FieldConfiguration fieldConfiguration) |
| `EncryptionKey` | `String` | Optional | Encryption Key<br><br>**Constraints**: *Minimum Length*: `32`, *Maximum Length*: `32` | String getEncryptionKey() | setEncryptionKey(String encryptionKey) |
| `StylesheetUrl` | `String` | Optional | Stylesheet Url | String getStylesheetUrl() | setStylesheetUrl(String stylesheetUrl) |
| `ParentSendMessage` | `Boolean` | Optional | Parent Send Message | Boolean getParentSendMessage() | setParentSendMessage(Boolean parentSendMessage) |
| `HideOptionalFields` | `Boolean` | Optional | Hide Optional Fields | Boolean getHideOptionalFields() | setHideOptionalFields(Boolean hideOptionalFields) |
| `Id` | `String` | Optional | Hosted Payment Page Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `CreatedUserId` | `String` | Optional | System generated id for user who created record<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `ModifiedUserId` | `String` | Optional | System generated id for user who created record<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getModifiedUserId() | setModifiedUserId(String modifiedUserId) |

## Example (as JSON)

```json
{
  "user_id": "11e95f8ec39de8fbdb0a4f1a",
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "title": "Sample title",
  "redirect_url_delay": 15,
  "min_payment_amount": 0,
  "max_payment_amount": 9999999999,
  "parent_send_message": true,
  "hide_optional_fields": true,
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "modified_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "location_api_id": "location_api_id2"
}
```

