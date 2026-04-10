
# Data 18

*This model accepts additional fields of type Object.*

## Structure

`Data18`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `LocationId` | `String` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `Title` | `String` | Optional | Title<br><br>**Constraints**: *Maximum Length*: `64` | String getTitle() | setTitle(String title) |
| `CcProductTransactionId` | `String` | Optional | Transaction ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCcProductTransactionId() | setCcProductTransactionId(String ccProductTransactionId) |
| `AchProductTransactionId` | `String` | Optional | ACH Product Transaction Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getAchProductTransactionId() | setAchProductTransactionId(String achProductTransactionId) |
| `DueDate` | `String` | Optional | Due Date, Format: Y-m-d<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getDueDate() | setDueDate(String dueDate) |
| `ItemList` | [`List<ItemList>`](../../doc/models/item-list.md) | Optional | Item List<br><br>**Constraints**: *Minimum Items*: `1`, *Maximum Items*: `300`, *Unique Items Required* | List<ItemList> getItemList() | setItemList(List<ItemList> itemList) |
| `AllowOverpayment` | `Boolean` | Optional | Allow Overpayment. | Boolean getAllowOverpayment() | setAllowOverpayment(Boolean allowOverpayment) |
| `BankFundedOnlyOverride` | `Boolean` | Optional | Bank Funded Only override | Boolean getBankFundedOnlyOverride() | setBankFundedOnlyOverride(Boolean bankFundedOnlyOverride) |
| `Email` | `String` | Optional | Email<br><br>**Constraints**: *Maximum Length*: `128` | String getEmail() | setEmail(String email) |
| `ContactId` | `String` | Optional | Contact ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getContactId() | setContactId(String contactId) |
| `ContactApiId` | `String` | Optional | Contact API Id<br><br>**Constraints**: *Maximum Length*: `64` | String getContactApiId() | setContactApiId(String contactApiId) |
| `QuickInvoiceApiId` | `String` | Optional | Quick Invoice API Id<br><br>**Constraints**: *Maximum Length*: `64` | String getQuickInvoiceApiId() | setQuickInvoiceApiId(String quickInvoiceApiId) |
| `CustomerId` | `String` | Optional | Customer Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCustomerId() | setCustomerId(String customerId) |
| `ExpireDate` | `String` | Optional | Expire Date.<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getExpireDate() | setExpireDate(String expireDate) |
| `AllowPartialPay` | `Boolean` | Optional | Allow partial pay | Boolean getAllowPartialPay() | setAllowPartialPay(Boolean allowPartialPay) |
| `AttachFilesToEmail` | `Boolean` | Optional | Attach Files to Email | Boolean getAttachFilesToEmail() | setAttachFilesToEmail(Boolean attachFilesToEmail) |
| `SendEmail` | `Boolean` | Optional | Send Email | Boolean getSendEmail() | setSendEmail(Boolean sendEmail) |
| `InvoiceNumber` | `String` | Optional | Invoice number<br><br>**Constraints**: *Maximum Length*: `64` | String getInvoiceNumber() | setInvoiceNumber(String invoiceNumber) |
| `ItemHeader` | `String` | Optional | Item Header<br><br>**Constraints**: *Maximum Length*: `250` | String getItemHeader() | setItemHeader(String itemHeader) |
| `ItemFooter` | `String` | Optional | Item footer<br><br>**Constraints**: *Maximum Length*: `250` | String getItemFooter() | setItemFooter(String itemFooter) |
| `AmountDue` | `Double` | Optional | Amount Due | Double getAmountDue() | setAmountDue(Double amountDue) |
| `NotificationEmail` | `String` | Optional | Notification email<br><br>**Constraints**: *Maximum Length*: `640` | String getNotificationEmail() | setNotificationEmail(String notificationEmail) |
| `StatusId` | `Object` | Optional | - | Object getStatusId() | setStatusId(Object statusId) |
| `StatusCode` | `Object` | Optional | - | Object getStatusCode() | setStatusCode(Object statusCode) |
| `Note` | `String` | Optional | Note<br><br>**Constraints**: *Maximum Length*: `200` | String getNote() | setNote(String note) |
| `NotificationDaysBeforeDueDate` | `Integer` | Optional | Notification days before due date<br><br>**Constraints**: `>= 0`, `<= 99` | Integer getNotificationDaysBeforeDueDate() | setNotificationDaysBeforeDueDate(Integer notificationDaysBeforeDueDate) |
| `NotificationDaysAfterDueDate` | `Integer` | Optional | Notification days after due date<br><br>**Constraints**: `>= 0`, `<= 99` | Integer getNotificationDaysAfterDueDate() | setNotificationDaysAfterDueDate(Integer notificationDaysAfterDueDate) |
| `NotificationOnDueDate` | `Boolean` | Optional | Notification on due date | Boolean getNotificationOnDueDate() | setNotificationOnDueDate(Boolean notificationOnDueDate) |
| `SendTextToPay` | `Boolean` | Optional | Send Text To Pay | Boolean getSendTextToPay() | setSendTextToPay(Boolean sendTextToPay) |
| `Files` | [`List<File>`](../../doc/models/file.md) | Optional | File Information on `expand` | List<File> getFiles() | setFiles(List<File> files) |
| `RemainingBalance` | `Double` | Optional | Remaining Balance | Double getRemainingBalance() | setRemainingBalance(Double remainingBalance) |
| `SinglePaymentMinAmount` | `Integer` | Optional | Single Payment Min Amount | Integer getSinglePaymentMinAmount() | setSinglePaymentMinAmount(Integer singlePaymentMinAmount) |
| `SinglePaymentMaxAmount` | `Integer` | Optional | Single Payment Max Amount<br><br>**Default**: `999999999` | Integer getSinglePaymentMaxAmount() | setSinglePaymentMaxAmount(Integer singlePaymentMaxAmount) |
| `CellPhone` | `String` | Optional | Cell Phone<br><br>**Constraints**: *Minimum Length*: `10`, *Maximum Length*: `10`, *Pattern*: `^\d{10}$` | String getCellPhone() | setCellPhone(String cellPhone) |
| `Tags` | [`List<Tag>`](../../doc/models/tag.md) | Optional | Tag Information on `expand` | List<Tag> getTags() | setTags(List<Tag> tags) |
| `QuickInvoiceC1` | `String` | Optional | Custom field 1 for api users to store custom data<br><br>**Constraints**: *Maximum Length*: `128` | String getQuickInvoiceC1() | setQuickInvoiceC1(String quickInvoiceC1) |
| `QuickInvoiceC2` | `String` | Optional | Custom field 2 for api users to store custom data<br><br>**Constraints**: *Maximum Length*: `128` | String getQuickInvoiceC2() | setQuickInvoiceC2(String quickInvoiceC2) |
| `QuickInvoiceC3` | `String` | Optional | Custom field 1 for api users to store custom data<br><br>**Constraints**: *Maximum Length*: `128` | String getQuickInvoiceC3() | setQuickInvoiceC3(String quickInvoiceC3) |
| `AutoReopen` | `Boolean` | Optional | Auto Reopen. If set to true, a void, refund or detachment of a Transaction Payment will cause the QuickInvoice to be opened again | Boolean getAutoReopen() | setAutoReopen(Boolean autoReopen) |
| `Id` | `String` | Optional | Quick Invoice ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `CreatedUserId` | `String` | Optional | Created User Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `ModifiedUserId` | `String` | Optional | Modified User Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getModifiedUserId() | setModifiedUserId(String modifiedUserId) |
| `Active` | `Boolean` | Optional | Active status | Boolean getActive() | setActive(Boolean active) |
| `PaymentStatusId` | `Integer` | Optional | Payment Status Id<br><br>**Constraints**: `>= 1`, `<= 3` | Integer getPaymentStatusId() | setPaymentStatusId(Integer paymentStatusId) |
| `IsActive` | `Boolean` | Optional | Register is active | Boolean getIsActive() | setIsActive(Boolean isActive) |
| `QuickInvoiceSetting` | [`QuickInvoiceSetting1`](../../doc/models/quick-invoice-setting-1.md) | Optional | - | QuickInvoiceSetting1 getQuickInvoiceSetting() | setQuickInvoiceSetting(QuickInvoiceSetting1 quickInvoiceSetting) |
| `QuickInvoiceViews` | [`List<QuickInvoiceView>`](../../doc/models/quick-invoice-view.md) | Optional | Quick Invoice View Information on `expand` | List<QuickInvoiceView> getQuickInvoiceViews() | setQuickInvoiceViews(List<QuickInvoiceView> quickInvoiceViews) |
| `Location` | [`Location18`](../../doc/models/location-18.md) | Optional | - | Location18 getLocation() | setLocation(Location18 location) |
| `CreatedUser` | [`User9`](../../doc/models/user-9.md) | Optional | - | User9 getCreatedUser() | setCreatedUser(User9 createdUser) |
| `ModifiedUser` | [`User9`](../../doc/models/user-9.md) | Optional | - | User9 getModifiedUser() | setModifiedUser(User9 modifiedUser) |
| `Changelogs` | [`List<Changelog>`](../../doc/models/changelog.md) | Optional | Changelog Information on `expand` | List<Changelog> getChangelogs() | setChangelogs(List<Changelog> changelogs) |
| `Contact` | [`Contact3`](../../doc/models/contact-3.md) | Optional | - | Contact3 getContact() | setContact(Contact3 contact) |
| `LogEmails` | [`List<LogEmail>`](../../doc/models/log-email.md) | Optional | Log Email Information on `expand` | List<LogEmail> getLogEmails() | setLogEmails(List<LogEmail> logEmails) |
| `LogSms` | [`LogSms1`](../../doc/models/log-sms-1.md) | Optional | - | LogSms1 getLogSms() | setLogSms(LogSms1 logSms) |
| `Transactions` | [`List<Transaction>`](../../doc/models/transaction.md) | Optional | Transaction Information on `expand` | List<Transaction> getTransactions() | setTransactions(List<Transaction> transactions) |
| `CcProductTransaction` | [`ProductTransaction1`](../../doc/models/product-transaction-1.md) | Optional | - | ProductTransaction1 getCcProductTransaction() | setCcProductTransaction(ProductTransaction1 ccProductTransaction) |
| `AchProductTransaction` | [`ProductTransaction1`](../../doc/models/product-transaction-1.md) | Optional | - | ProductTransaction1 getAchProductTransaction() | setAchProductTransaction(ProductTransaction1 achProductTransaction) |
| `EmailBlacklist` | [`EmailBlacklist1`](../../doc/models/email-blacklist-1.md) | Optional | - | EmailBlacklist1 getEmailBlacklist() | setEmailBlacklist(EmailBlacklist1 emailBlacklist) |
| `SmsBlacklist` | [`SmsBlacklist1`](../../doc/models/sms-blacklist-1.md) | Optional | - | SmsBlacklist1 getSmsBlacklist() | setSmsBlacklist(SmsBlacklist1 smsBlacklist) |
| `PaymentUrl` | `String` | Optional | Payment Url Information on `expand` | String getPaymentUrl() | setPaymentUrl(String paymentUrl) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "title": "My terminal",
  "cc_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "ach_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "due_date": "2021-12-01",
  "allow_overpayment": true,
  "bank_funded_only_override": true,
  "email": "email@domain.com",
  "contact_id": "11e95f8ec39de8fbdb0a4f1a",
  "contact_api_id": "contact12345",
  "quick_invoice_api_id": "quickinvoice12345",
  "customer_id": "11e95f8ec39de8fbdb0a4f1a",
  "expire_date": "2021-12-01",
  "allow_partial_pay": true,
  "attach_files_to_email": true,
  "send_email": true,
  "invoice_number": "invoice12345",
  "item_header": "Quick invoice header sample",
  "item_footer": "Thank you",
  "amount_due": 245.36,
  "notification_email": "email@domain.com",
  "note": "some note",
  "notification_days_before_due_date": 3,
  "notification_days_after_due_date": 7,
  "notification_on_due_date": true,
  "send_text_to_pay": true,
  "remaining_balance": 245.36,
  "single_payment_min_amount": 500,
  "single_payment_max_amount": 500000,
  "cell_phone": "3339998822",
  "quick_invoice_c1": "custom-data-1",
  "quick_invoice_c2": "custom-data-2",
  "quick_invoice_c3": "custom-data-3",
  "auto_reopen": true,
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "modified_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "active": true,
  "payment_status_id": 1,
  "is_active": true,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

