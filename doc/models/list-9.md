
# List 9

*This model accepts additional fields of type Object.*

## Structure

`List9`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `LocationId` | `String` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `CcProductTransactionId` | `String` | Optional | cc_product_transaction_id that has paylinks enabled in the service settings.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCcProductTransactionId() | setCcProductTransactionId(String ccProductTransactionId) |
| `Email` | `String` | Optional | Optional. An email address that should be used as the "To" address when sending a Paylink Notification email.<br><br>**Constraints**: *Maximum Length*: `128` | String getEmail() | setEmail(String email) |
| `AmountDue` | `Integer` | Optional | This is the amount that need to be paid (automatically calculated by system). amount_due= sum of items in item_list<br><br>**Constraints**: `>= 1`, `<= 999999999` | Integer getAmountDue() | setAmountDue(Integer amountDue) |
| `LocationApiId` | `String` | Optional | Location Api Id. System id | String getLocationApiId() | setLocationApiId(String locationApiId) |
| `ContactId` | `String` | Optional | Include the Contact_id that the Paylink will belong to. This will allow you to query the List All Paylinks and filter_by Contact_id to see the status of all the contacts Paylinks.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getContactId() | setContactId(String contactId) |
| `ContactApiId` | `String` | Optional | Integrator provided unique id that was provided during the contact creation for the Fortis Contact. Include the Contact_id that the Paylink will belong to. This will allow you to query the List All Paylinks and filter_by Contact_id to see the status of all the contacts Paylinks. | String getContactApiId() | setContactApiId(String contactApiId) |
| `PaylinkApiId` | `String` | Optional | Integrator provided id that prevents duplicate Paylinke Api Id's per location.<br><br>**Constraints**: *Maximum Length*: `64` | String getPaylinkApiId() | setPaylinkApiId(String paylinkApiId) |
| `AchProductTransactionId` | `String` | Optional | ACH product transaction on which Paylink is created. This field is optional and will default to default_ach product if not supplied at all. Either this or cc_product_transaction_id must be supplied. Changes are allowed on PUT if payments have not been made against Paylink.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getAchProductTransactionId() | setAchProductTransactionId(String achProductTransactionId) |
| `ExpireDate` | `String` | Optional | Expire Date of Paylink. Optional<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getExpireDate() | setExpireDate(String expireDate) |
| `DisplayProductTransactionReceiptDetails` | `Boolean` | Optional | Display Product Transaction Receipt Details. Show the receipt details after the successful payment | Boolean getDisplayProductTransactionReceiptDetails() | setDisplayProductTransactionReceiptDetails(Boolean displayProductTransactionReceiptDetails) |
| `DisplayBillingFields` | `Boolean` | Optional | Display Billing Fields to show the billing field inputs in the paylink form | Boolean getDisplayBillingFields() | setDisplayBillingFields(Boolean displayBillingFields) |
| `DeliveryMethod` | `Object` | Optional | - | Object getDeliveryMethod() | setDeliveryMethod(Object deliveryMethod) |
| `CellPhone` | `String` | Optional | Required if delivery_method is set to 2[SMS], 3[Both email and sms], this will be the recipient of the SMS<br><br>**Constraints**: *Minimum Length*: `10`, *Maximum Length*: `10`, *Pattern*: `^\d{1,10}$` | String getCellPhone() | setCellPhone(String cellPhone) |
| `Description` | `String` | Optional | Add a Description for reporting purposes<br><br>**Constraints**: *Maximum Length*: `64` | String getDescription() | setDescription(String description) |
| `StoreToken` | `Boolean` | Optional | Store Token to create a token_id(account_vault_id) to be used for future payment types(CC Sale Tokenized, ACH Debit Tokenized) | Boolean getStoreToken() | setStoreToken(Boolean storeToken) |
| `StoreTokenTitle` | `String` | Optional | Store Token Title can be used to set the name of the token, sucha John Smith<br><br>**Constraints**: *Maximum Length*: `16` | String getStoreTokenTitle() | setStoreTokenTitle(String storeTokenTitle) |
| `PaylinkAction` | `Object` | Optional | - | Object getPaylinkAction() | setPaylinkAction(Object paylinkAction) |
| `BankFundedOnlyOverride` | `Boolean` | Optional | Bank Funded Only Override | Boolean getBankFundedOnlyOverride() | setBankFundedOnlyOverride(Boolean bankFundedOnlyOverride) |
| `Tags` | `List<String>` | Optional | Used to apply tags to a paylink. | List<String> getTags() | setTags(List<String> tags) |
| `RedirectUrlDelay` | `Double` | Optional | Redirect URL Delay in seconds<br><br>**Default**: `15d`<br><br>**Constraints**: `<= 15` | Double getRedirectUrlDelay() | setRedirectUrlDelay(Double redirectUrlDelay) |
| `RedirectUrlOnApprove` | `String` | Optional | Redirect URL On Approved transactions | String getRedirectUrlOnApprove() | setRedirectUrlOnApprove(String redirectUrlOnApprove) |
| `RedirectUrlOnDecline` | `String` | Optional | Redirect URL On Declined transactions | String getRedirectUrlOnDecline() | setRedirectUrlOnDecline(String redirectUrlOnDecline) |
| `Id` | `String` | Optional | System generatedPaylink Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `StatusId` | `Boolean` | Optional | (DEPRECATED) Status Id | Boolean getStatusId() | setStatusId(Boolean statusId) |
| `StatusCode` | `Object` | Optional | - | Object getStatusCode() | setStatusCode(Object statusCode) |
| `Active` | `Boolean` | Optional | Paylink is still Active | Boolean getActive() | setActive(Boolean active) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `ModifiedUserId` | `String` | Optional | Last User ID that updated the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getModifiedUserId() | setModifiedUserId(String modifiedUserId) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "cc_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "email": "email@domain.com",
  "amount_due": 1,
  "contact_id": "11e95f8ec39de8fbdb0a4f1a",
  "ach_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "expire_date": "2021-12-01",
  "display_product_transaction_receipt_details": true,
  "display_billing_fields": true,
  "cell_phone": "3339998822",
  "description": "Description",
  "store_token": false,
  "store_token_title": "John Account",
  "bank_funded_only_override": false,
  "redirect_url_delay": 15,
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "status_id": true,
  "active": true,
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "modified_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "location_api_id": "location_api_id8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

