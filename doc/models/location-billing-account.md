
# Location Billing Account

## Structure

`LocationBillingAccount`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Title` | `String` | Optional | Title<br><br>**Constraints**: *Maximum Length*: `64` | String getTitle() | setTitle(String title) |
| `LocationId` | `String` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `LocationApiId` | `String` | Optional | Location Api Id | String getLocationApiId() | setLocationApiId(String locationApiId) |
| `AchSecCode` | `String` | Optional | Ach Sec Code | String getAchSecCode() | setAchSecCode(String achSecCode) |
| `AccountNumber` | `String` | Optional | Account number | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `Routing` | `String` | Optional | Routing | String getRouting() | setRouting(String routing) |
| `ExpDate` | `String` | Optional | Exp Date | String getExpDate() | setExpDate(String expDate) |
| `BillingZip` | `String` | Optional | Billing Zip<br><br>**Constraints**: *Minimum Length*: `3`, *Maximum Length*: `10`, *Pattern*: `^[a-zA-Z0-9\-\s]+$` | String getBillingZip() | setBillingZip(String billingZip) |
| `AccountType` | `String` | Optional | Account Type | String getAccountType() | setAccountType(String accountType) |
| `AccountHolderName` | `String` | Optional | Account Holder Name | String getAccountHolderName() | setAccountHolderName(String accountHolderName) |
| `Id` | `String` | Optional | Location Billing Account Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `CreatedUserId` | `String` | Optional | Created User Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `ModifiedUserId` | `String` | Optional | Modified User Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getModifiedUserId() | setModifiedUserId(String modifiedUserId) |
| `BillingDescriptor` | `String` | Optional | Billing Descriptor | String getBillingDescriptor() | setBillingDescriptor(String billingDescriptor) |
| `PaymentMethod` | `String` | Optional | Billing Descriptor | String getPaymentMethod() | setPaymentMethod(String paymentMethod) |
| `PortfolioId` | `String` | Optional | Portfolio Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getPortfolioId() | setPortfolioId(String portfolioId) |

## Example (as JSON)

```json
{
  "title": "Billing Acccount Title",
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "exp_date": "0722",
  "billing_zip": "48375",
  "account_holder_name": "John Smith",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "modified_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "portfolio_id": "11e95f8ec39de8fbdb0a4f1a",
  "location_api_id": "location_api_id4",
  "ach_sec_code": "ach_sec_code6",
  "account_number": "account_number4"
}
```

