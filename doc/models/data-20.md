
# Data 20

## Structure

`Data20`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AccountVaultId` | `String` | Optional | Token ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getAccountVaultId() | setAccountVaultId(String accountVaultId) |
| `TokenId` | `String` | Optional | Token ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getTokenId() | setTokenId(String tokenId) |
| `ContactId` | `String` | Optional | Contact ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getContactId() | setContactId(String contactId) |
| `AccountVaultApiId` | `String` | Optional | Token API ID<br><br>**Constraints**: *Maximum Length*: `64` | String getAccountVaultApiId() | setAccountVaultApiId(String accountVaultApiId) |
| `TokenApiId` | `String` | Optional | Token API ID<br><br>**Constraints**: *Maximum Length*: `64` | String getTokenApiId() | setTokenApiId(String tokenApiId) |
| `Joi` | [`Joi`](../../doc/models/joi.md) | Optional | - | Joi getJoi() | setJoi(Joi joi) |
| `Active` | `Boolean` | Optional | Active | Boolean getActive() | setActive(Boolean active) |
| `Description` | `String` | Optional | Description<br><br>**Constraints**: *Maximum Length*: `36` | String getDescription() | setDescription(String description) |
| `EndDate` | `String` | Optional | End date<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getEndDate() | setEndDate(String endDate) |
| `InstallmentTotalCount` | `Integer` | Optional | Installment Total Count<br><br>**Constraints**: `>= 1`, `<= 999` | Integer getInstallmentTotalCount() | setInstallmentTotalCount(Integer installmentTotalCount) |
| `Interval` | `Integer` | Optional | Interval<br><br>**Constraints**: `>= 0`, `<= 365` | Integer getInterval() | setInterval(Integer interval) |
| `IntervalType` | [`IntervalTypeEnum`](../../doc/models/interval-type-enum.md) | Optional | Interval Type | IntervalTypeEnum getIntervalType() | setIntervalType(IntervalTypeEnum intervalType) |
| `LocationId` | `String` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `NotificationDays` | `Integer` | Optional | Notification Days<br><br>**Constraints**: `>= 0`, `<= 365` | Integer getNotificationDays() | setNotificationDays(Integer notificationDays) |
| `PaymentMethod` | [`PaymentMethod1Enum`](../../doc/models/payment-method-1-enum.md) | Optional | Payment Method | PaymentMethod1Enum getPaymentMethod() | setPaymentMethod(PaymentMethod1Enum paymentMethod) |
| `ProductTransactionId` | `String` | Optional | Product Transaction ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getProductTransactionId() | setProductTransactionId(String productTransactionId) |
| `RecurringId` | `String` | Optional | Recurring ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getRecurringId() | setRecurringId(String recurringId) |
| `RecurringApiId` | `String` | Optional | Recurring Api ID<br><br>**Constraints**: *Maximum Length*: `64` | String getRecurringApiId() | setRecurringApiId(String recurringApiId) |
| `StartDate` | `String` | Optional | Start date<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getStartDate() | setStartDate(String startDate) |
| `Status` | [`StatusEnum`](../../doc/models/status-enum.md) | Optional | Status | StatusEnum getStatus() | setStatus(StatusEnum status) |
| `TransactionAmount` | `Integer` | Optional | Transaction amount | Integer getTransactionAmount() | setTransactionAmount(Integer transactionAmount) |
| `TermsAgree` | `Boolean` | Optional | Terms Agree | Boolean getTermsAgree() | setTermsAgree(Boolean termsAgree) |
| `TermsAgreeIp` | `String` | Optional | Terms Agree Ip | String getTermsAgreeIp() | setTermsAgreeIp(String termsAgreeIp) |
| `RecurringC1` | `String` | Optional | Custom field used for integrations<br><br>**Constraints**: *Maximum Length*: `128` | String getRecurringC1() | setRecurringC1(String recurringC1) |
| `RecurringC2` | `String` | Optional | Custom field used for integrations<br><br>**Constraints**: *Maximum Length*: `128` | String getRecurringC2() | setRecurringC2(String recurringC2) |
| `RecurringC3` | `String` | Optional | Custom field used for integrations<br><br>**Constraints**: *Maximum Length*: `128` | String getRecurringC3() | setRecurringC3(String recurringC3) |
| `SendToProcAsRecur` | `Boolean` | Optional | Send To Proc As Recur | Boolean getSendToProcAsRecur() | setSendToProcAsRecur(Boolean sendToProcAsRecur) |
| `Tags` | [`List<Tag>`](../../doc/models/tag.md) | Optional | Tag Information on `expand` | List<Tag> getTags() | setTags(List<Tag> tags) |
| `SecondaryAmount` | `Integer` | Optional | Retained Amount | Integer getSecondaryAmount() | setSecondaryAmount(Integer secondaryAmount) |
| `Currency` | `String` | Optional | - | String getCurrency() | setCurrency(String currency) |
| `Id` | `String` | Optional | Recurring ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `NextRunDate` | `String` | Optional | Next Run Date<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getNextRunDate() | setNextRunDate(String nextRunDate) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `RecurringTypeId` | [`RecurringTypeIdEnum`](../../doc/models/recurring-type-id-enum.md) | Optional | Recurring Type | RecurringTypeIdEnum getRecurringTypeId() | setRecurringTypeId(RecurringTypeIdEnum recurringTypeId) |
| `InstallmentAmountTotal` | `Integer` | Optional | Installment Amount Total | Integer getInstallmentAmountTotal() | setInstallmentAmountTotal(Integer installmentAmountTotal) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `LogEmails` | [`List<LogEmail>`](../../doc/models/log-email.md) | Optional | Log Email Information on `expand` | List<LogEmail> getLogEmails() | setLogEmails(List<LogEmail> logEmails) |
| `Contact` | [`Contact1`](../../doc/models/contact-1.md) | Optional | Contact Information on `expand` | Contact1 getContact() | setContact(Contact1 contact) |
| `AccountVault` | [`AccountVault`](../../doc/models/account-vault.md) | Optional | Token Information on `expand` | AccountVault getAccountVault() | setAccountVault(AccountVault accountVault) |
| `CreatedUser` | [`CreatedUser`](../../doc/models/created-user.md) | Optional | User Information on `expand` | CreatedUser getCreatedUser() | setCreatedUser(CreatedUser createdUser) |
| `Signature` | [`Signature`](../../doc/models/signature.md) | Optional | Signature Information on `expand` | Signature getSignature() | setSignature(Signature signature) |
| `PaymentSchedule` | `List<String>` | Optional | Payment Schedule Information on `expand`<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | List<String> getPaymentSchedule() | setPaymentSchedule(List<String> paymentSchedule) |
| `Location` | [`Location`](../../doc/models/location.md) | Optional | Location Information on `expand` | Location getLocation() | setLocation(Location location) |
| `ProductTransaction` | [`ProductTransaction`](../../doc/models/product-transaction.md) | Optional | Product Transaction Information on `expand` | ProductTransaction getProductTransaction() | setProductTransaction(ProductTransaction productTransaction) |
| `NextRunDateMin` | `String` | Optional | Next Run Date Min Information on `expand`<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getNextRunDateMin() | setNextRunDateMin(String nextRunDateMin) |
| `NextRunDateMax` | `String` | Optional | Next Run Date Max Information on `expand`<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getNextRunDateMax() | setNextRunDateMax(String nextRunDateMax) |
| `AllTags` | [`List<AllTag>`](../../doc/models/all-tag.md) | Optional | All Tag Information on `expand` | List<AllTag> getAllTags() | setAllTags(List<AllTag> allTags) |
| `Changelogs` | [`List<Changelog>`](../../doc/models/changelog.md) | Optional | Changelog Information on `expand` | List<Changelog> getChangelogs() | setChangelogs(List<Changelog> changelogs) |
| `Forecast` | [`Forecast`](../../doc/models/forecast.md) | Optional | Forecast Information on `expand` | Forecast getForecast() | setForecast(Forecast forecast) |
| `RecurringSplits` | [`List<RecurringSplit>`](../../doc/models/recurring-split.md) | Optional | Recurring Split Information on `expand` | List<RecurringSplit> getRecurringSplits() | setRecurringSplits(List<RecurringSplit> recurringSplits) |

## Example (as JSON)

```json
{
  "account_vault_id": "11e95f8ec39de8fbdb0a4f1a",
  "token_id": "11e95f8ec39de8fbdb0a4f1a",
  "contact_id": "11e95f8ec39de8fbdb0a4f1a",
  "account_vault_api_id": "token1234abcd",
  "token_api_id": "token1234abcd",
  "active": true,
  "description": "Description",
  "end_date": "2021-12-01",
  "installment_total_count": 20,
  "interval": 1,
  "interval_type": "d",
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "notification_days": 2,
  "payment_method": "cc",
  "product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "recurring_id": "11e95f8ec39de8fbdb0a4f1a",
  "recurring_api_id": "recurring1234abcd",
  "start_date": "2021-12-01",
  "status": "active",
  "transaction_amount": 300,
  "terms_agree": true,
  "terms_agree_ip": "192.168.0.10",
  "recurring_c1": "recurring custom data 1",
  "recurring_c2": "recurring custom data 2",
  "recurring_c3": "recurring custom data 3",
  "send_to_proc_as_recur": true,
  "secondary_amount": 100,
  "currency": "USD",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "next_run_date": "2021-12-01",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "recurring_type_id": "i",
  "installment_amount_total": 99999999,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "next_run_date_min": "2021-12-01",
  "next_run_date_max": "2021-12-01"
}
```

