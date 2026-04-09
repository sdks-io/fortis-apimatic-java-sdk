
# Modified User

Modified User Information on `expand`

## Structure

`ModifiedUser`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AccountNumber` | `String` | Optional | Account Number | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `BrandingDomainUrl` | `String` | Optional | Branding Domain Url<br><br>**Constraints**: *Maximum Length*: `64` | String getBrandingDomainUrl() | setBrandingDomainUrl(String brandingDomainUrl) |
| `CellPhone` | `String` | Optional | Cell Phone<br><br>**Constraints**: *Minimum Length*: `10`, *Maximum Length*: `10`, *Pattern*: `^\d{10}$` | String getCellPhone() | setCellPhone(String cellPhone) |
| `CompanyName` | `String` | Optional | Company Name<br><br>**Constraints**: *Maximum Length*: `64` | String getCompanyName() | setCompanyName(String companyName) |
| `ContactId` | `String` | Optional | Contact<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getContactId() | setContactId(String contactId) |
| `DateOfBirth` | `String` | Optional | Date Of Birth<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getDateOfBirth() | setDateOfBirth(String dateOfBirth) |
| `DomainId` | `String` | Optional | Domain<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getDomainId() | setDomainId(String domainId) |
| `Email` | `String` | Optional | Email<br><br>**Constraints**: *Maximum Length*: `128` | String getEmail() | setEmail(String email) |
| `EmailTrxReceipt` | `Boolean` | Optional | Email Trx Receipt | Boolean getEmailTrxReceipt() | setEmailTrxReceipt(Boolean emailTrxReceipt) |
| `HomePhone` | `String` | Optional | Home Phone<br><br>**Constraints**: *Minimum Length*: `10`, *Maximum Length*: `10`, *Pattern*: `^\d{10}$` | String getHomePhone() | setHomePhone(String homePhone) |
| `FirstName` | `String` | Optional | First Name<br><br>**Constraints**: *Maximum Length*: `64` | String getFirstName() | setFirstName(String firstName) |
| `LastName` | `String` | Optional | Last Name<br><br>**Constraints**: *Maximum Length*: `64` | String getLastName() | setLastName(String lastName) |
| `Locale` | `String` | Optional | Locale<br><br>**Constraints**: *Maximum Length*: `8` | String getLocale() | setLocale(String locale) |
| `OfficePhone` | `String` | Optional | Office Phone<br><br>**Constraints**: *Minimum Length*: `10`, *Maximum Length*: `10`, *Pattern*: `^\d{10}$` | String getOfficePhone() | setOfficePhone(String officePhone) |
| `OfficeExtPhone` | `String` | Optional | Office Ext Phone<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^\d{1,10}$` | String getOfficeExtPhone() | setOfficeExtPhone(String officeExtPhone) |
| `PrimaryLocationId` | `String` | Optional | Primary Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getPrimaryLocationId() | setPrimaryLocationId(String primaryLocationId) |
| `RequiresNewPassword` | `String` | Optional | Requires New Password<br><br>**Constraints**: *Maximum Length*: `1` | String getRequiresNewPassword() | setRequiresNewPassword(String requiresNewPassword) |
| `TermsConditionCode` | `String` | Optional | Terms Condition (This field is required when updating your own password). | String getTermsConditionCode() | setTermsConditionCode(String termsConditionCode) |
| `Tz` | `String` | Optional | Time zone<br><br>**Constraints**: *Maximum Length*: `30` | String getTz() | setTz(String tz) |
| `UiPrefs` | [`UiPrefs`](../../doc/models/ui-prefs.md) | Optional | Ui Prefs | UiPrefs getUiPrefs() | setUiPrefs(UiPrefs uiPrefs) |
| `Username` | `String` | Optional | Username<br><br>**Constraints**: *Minimum Length*: `2`, *Maximum Length*: `64` | String getUsername() | setUsername(String username) |
| `UserApiKey` | `String` | Optional | User Api Key<br><br>**Constraints**: *Minimum Length*: `16`, *Maximum Length*: `64` | String getUserApiKey() | setUserApiKey(String userApiKey) |
| `UserHashKey` | `String` | Optional | User Hash Key<br><br>**Constraints**: *Minimum Length*: `24`, *Maximum Length*: `36` | String getUserHashKey() | setUserHashKey(String userHashKey) |
| `UserTypeCode` | [`UserTypeCodeEnum`](../../doc/models/user-type-code-enum.md) | Optional | User Type | UserTypeCodeEnum getUserTypeCode() | setUserTypeCode(UserTypeCodeEnum userTypeCode) |
| `Password` | `String` | Optional | Password<br><br>**Constraints**: *Minimum Length*: `8`, *Maximum Length*: `128`, *Pattern*: ``^(?=.*[`!@#$%^&*()_+\-=\[\]{};':"\\\|,.<>\/?~])(?=.*[0-9])(?=.*[a-zA-Z]).*$`` | String getPassword() | setPassword(String password) |
| `Zip` | `String` | Optional | Zip<br><br>**Constraints**: *Minimum Length*: `3`, *Maximum Length*: `10`, *Pattern*: `^[a-zA-Z0-9\-\s]+$` | String getZip() | setZip(String zip) |
| `LocationId` | `String` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `ContactApiId` | `String` | Optional | ContactApi Id | String getContactApiId() | setContactApiId(String contactApiId) |
| `PrimaryLocationApiId` | `String` | Optional | Primary LocationApi ID | String getPrimaryLocationApiId() | setPrimaryLocationApiId(String primaryLocationApiId) |
| `StatusCode` | [`StatusCodeEnum`](../../doc/models/status-code-enum.md) | Optional | Status Code | StatusCodeEnum getStatusCode() | setStatusCode(StatusCodeEnum statusCode) |
| `ApiOnly` | `Boolean` | Optional | API Only | Boolean getApiOnly() | setApiOnly(Boolean apiOnly) |
| `IsInvitation` | `Boolean` | Optional | Is Invitation | Boolean getIsInvitation() | setIsInvitation(Boolean isInvitation) |
| `Address` | [`Address2`](../../doc/models/address-2.md) | Optional | Address | Address2 getAddress() | setAddress(Address2 address) |
| `Id` | `String` | Optional | User ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `Status` | `Boolean` | Optional | Status | Boolean getStatus() | setStatus(Boolean status) |
| `LoginAttempts` | `Integer` | Optional | Login Attempts | Integer getLoginAttempts() | setLoginAttempts(Integer loginAttempts) |
| `LastLoginTs` | `Integer` | Optional | Last Login | Integer getLastLoginTs() | setLastLoginTs(Integer lastLoginTs) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `CreatedUserId` | `String` | Optional | Created User<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `TermsAcceptedTs` | `Integer` | Optional | Terms Accepted | Integer getTermsAcceptedTs() | setTermsAcceptedTs(Integer termsAcceptedTs) |
| `TermsAgreeIp` | `String` | Optional | Terms Agree Ip<br><br>**Constraints**: *Maximum Length*: `16` | String getTermsAgreeIp() | setTermsAgreeIp(String termsAgreeIp) |
| `CurrentDateTime` | `String` | Optional | Current Date Time<br><br>**Constraints**: *Maximum Length*: `24` | String getCurrentDateTime() | setCurrentDateTime(String currentDateTime) |
| `CurrentLoginIp` | `String` | Optional | Current Login Ip | String getCurrentLoginIp() | setCurrentLoginIp(String currentLoginIp) |
| `CurrentLogin` | `Integer` | Optional | Current Login Timestamp | Integer getCurrentLogin() | setCurrentLogin(Integer currentLogin) |
| `SftpAccess` | `Boolean` | Optional | SFTP Access | Boolean getSftpAccess() | setSftpAccess(Boolean sftpAccess) |
| `LogApiResponseBodyTs` | `Integer` | Optional | Log Api Response Body | Integer getLogApiResponseBodyTs() | setLogApiResponseBodyTs(Integer logApiResponseBodyTs) |

## Example (as JSON)

```json
{
  "account_number": "5454545454545454",
  "branding_domain_url": "{branding_domain_url}",
  "cell_phone": "3339998822",
  "company_name": "Fortis Payment Systems, LLC",
  "contact_id": "11e95f8ec39de8fbdb0a4f1a",
  "date_of_birth": "2021-12-01",
  "domain_id": "11e95f8ec39de8fbdb0a4f1a",
  "email": "email@domain.com",
  "email_trx_receipt": true,
  "home_phone": "3339998822",
  "first_name": "John",
  "last_name": "Smith",
  "locale": "en-US",
  "office_phone": "3339998822",
  "office_ext_phone": "5",
  "primary_location_id": "11e95f8ec39de8fbdb0a4f1a",
  "terms_condition_code": "20220308",
  "tz": "America/New_York",
  "username": "{user_name}",
  "user_api_key": "234bas8dfn8238f923w2",
  "user_type_code": 100,
  "zip": "48375",
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "status_code": 1,
  "api_only": false,
  "is_invitation": false,
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "status": true,
  "login_attempts": 0,
  "last_login_ts": 1422040992,
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "terms_accepted_ts": 1422040992,
  "terms_agree_ip": "192.168.0.10",
  "current_login": 1422040992,
  "log_api_response_body_ts": 1422040992
}
```

