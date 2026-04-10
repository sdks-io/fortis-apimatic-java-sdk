
# Active Recurring

*This model accepts additional fields of type Object.*

## Structure

`ActiveRecurring`

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
| `IntervalType` | [`IntervalType`](../../doc/models/interval-type.md) | Optional | - | IntervalType getIntervalType() | setIntervalType(IntervalType intervalType) |
| `LocationId` | `String` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `NotificationDays` | `Integer` | Optional | Notification Days<br><br>**Constraints**: `>= 0`, `<= 365` | Integer getNotificationDays() | setNotificationDays(Integer notificationDays) |
| `PaymentMethod` | [`PaymentMethod1`](../../doc/models/payment-method-1.md) | Optional | - | PaymentMethod1 getPaymentMethod() | setPaymentMethod(PaymentMethod1 paymentMethod) |
| `ProductTransactionId` | `String` | Optional | Product Transaction ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getProductTransactionId() | setProductTransactionId(String productTransactionId) |
| `RecurringId` | `String` | Optional | Recurring ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getRecurringId() | setRecurringId(String recurringId) |
| `RecurringApiId` | `String` | Optional | Recurring Api ID<br><br>**Constraints**: *Maximum Length*: `64` | String getRecurringApiId() | setRecurringApiId(String recurringApiId) |
| `StartDate` | `String` | Optional | Start date<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getStartDate() | setStartDate(String startDate) |
| `Status` | [`Status`](../../doc/models/status.md) | Optional | - | Status getStatus() | setStatus(Status status) |
| `TransactionAmount` | `Integer` | Optional | Transaction amount | Integer getTransactionAmount() | setTransactionAmount(Integer transactionAmount) |
| `TermsAgree` | `Boolean` | Optional | Terms Agree | Boolean getTermsAgree() | setTermsAgree(Boolean termsAgree) |
| `TermsAgreeIp` | `String` | Optional | Terms Agree Ip | String getTermsAgreeIp() | setTermsAgreeIp(String termsAgreeIp) |
| `RecurringC1` | `String` | Optional | Custom field used for integrations<br><br>**Constraints**: *Maximum Length*: `128` | String getRecurringC1() | setRecurringC1(String recurringC1) |
| `RecurringC2` | `String` | Optional | Custom field used for integrations<br><br>**Constraints**: *Maximum Length*: `128` | String getRecurringC2() | setRecurringC2(String recurringC2) |
| `RecurringC3` | `String` | Optional | Custom field used for integrations<br><br>**Constraints**: *Maximum Length*: `128` | String getRecurringC3() | setRecurringC3(String recurringC3) |
| `SendToProcAsRecur` | `Boolean` | Optional | Send To Proc As Recur | Boolean getSendToProcAsRecur() | setSendToProcAsRecur(Boolean sendToProcAsRecur) |
| `Tags` | `List<String>` | Optional | Tags | List<String> getTags() | setTags(List<String> tags) |
| `SecondaryAmount` | `Integer` | Optional | Retained Amount | Integer getSecondaryAmount() | setSecondaryAmount(Integer secondaryAmount) |
| `Currency` | `String` | Optional | - | String getCurrency() | setCurrency(String currency) |
| `Id` | `String` | Optional | Recurring ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `NextRunDate` | `String` | Optional | Next Run Date<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getNextRunDate() | setNextRunDate(String nextRunDate) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `RecurringTypeId` | [`RecurringTypeId`](../../doc/models/recurring-type-id.md) | Optional | - | RecurringTypeId getRecurringTypeId() | setRecurringTypeId(RecurringTypeId recurringTypeId) |
| `InstallmentAmountTotal` | `Integer` | Optional | Installment Amount Total | Integer getInstallmentAmountTotal() | setInstallmentAmountTotal(Integer installmentAmountTotal) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

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
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "notification_days": 2,
  "product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "recurring_id": "11e95f8ec39de8fbdb0a4f1a",
  "recurring_api_id": "recurring1234abcd",
  "start_date": "2021-12-01",
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
  "installment_amount_total": 99999999,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

