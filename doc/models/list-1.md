
# List 1

*This model accepts additional fields of type Object.*

## Structure

`List1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `LocationId` | `String` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `AccountNumber` | `String` | Optional | Contact Account Number<br><br>**Constraints**: *Maximum Length*: `32` | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `ContactApiId` | `String` | Optional | Contact API Id<br><br>**Constraints**: *Maximum Length*: `64`, *Pattern*: `^[a-zA-Z0-9]*$` | String getContactApiId() | setContactApiId(String contactApiId) |
| `FirstName` | `String` | Optional | First Name<br><br>**Constraints**: *Maximum Length*: `64` | String getFirstName() | setFirstName(String firstName) |
| `LastName` | `String` | Optional | Last Name<br><br>**Constraints**: *Maximum Length*: `64` | String getLastName() | setLastName(String lastName) |
| `CellPhone` | `String` | Optional | Cell phone of contact<br><br>**Constraints**: *Minimum Length*: `10`, *Maximum Length*: `10`, *Pattern*: `^\d{10}$` | String getCellPhone() | setCellPhone(String cellPhone) |
| `Balance` | `Double` | Optional | Balance<br><br>**Constraints**: `>= -99999999.99`, `<= 99999999.99` | Double getBalance() | setBalance(Double balance) |
| `Address` | [`Address4`](../../doc/models/address-4.md) | Optional | - | Address4 getAddress() | setAddress(Address4 address) |
| `CompanyName` | `String` | Optional | Company Name<br><br>**Constraints**: *Maximum Length*: `64` | String getCompanyName() | setCompanyName(String companyName) |
| `HeaderMessage` | `String` | Optional | Header Message<br><br>**Constraints**: *Maximum Length*: `250` | String getHeaderMessage() | setHeaderMessage(String headerMessage) |
| `DateOfBirth` | `String` | Optional | Contacts DOB, Format: yyyy-MM-dd<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getDateOfBirth() | setDateOfBirth(String dateOfBirth) |
| `EmailTrxReceipt` | `Boolean` | Optional | Whether or not to email all transactions receipts to contact (1 or 0) | Boolean getEmailTrxReceipt() | setEmailTrxReceipt(Boolean emailTrxReceipt) |
| `HomePhone` | `String` | Optional | Contacts home phone<br><br>**Constraints**: *Minimum Length*: `10`, *Maximum Length*: `10`, *Pattern*: `^\d{10}$` | String getHomePhone() | setHomePhone(String homePhone) |
| `OfficePhone` | `String` | Optional | Contacts office phone<br><br>**Constraints**: *Minimum Length*: `10`, *Maximum Length*: `10`, *Pattern*: `^\d{10}$` | String getOfficePhone() | setOfficePhone(String officePhone) |
| `OfficePhoneExt` | `String` | Optional | Contacts office phone extension for office phone<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^\d{1,10}$` | String getOfficePhoneExt() | setOfficePhoneExt(String officePhoneExt) |
| `HomePhoneCountryCode` | `String` | Optional | Home phone country code<br><br>**Constraints**: *Maximum Length*: `6`, *Pattern*: `^\+([\d]+)$` | String getHomePhoneCountryCode() | setHomePhoneCountryCode(String homePhoneCountryCode) |
| `OfficePhoneCountryCode` | `String` | Optional | Office phone country code<br><br>**Constraints**: *Maximum Length*: `6`, *Pattern*: `^\+([\d]+)$` | String getOfficePhoneCountryCode() | setOfficePhoneCountryCode(String officePhoneCountryCode) |
| `CellPhoneCountryCode` | `String` | Optional | Cell phone country code<br><br>**Constraints**: *Maximum Length*: `6`, *Pattern*: `^\+([\d]+)$` | String getCellPhoneCountryCode() | setCellPhoneCountryCode(String cellPhoneCountryCode) |
| `HeaderMessageType` | `Integer` | Optional | Header Message Type<br><br>**Constraints**: `>= 0`, `<= 4` | Integer getHeaderMessageType() | setHeaderMessageType(Integer headerMessageType) |
| `UpdateIfExists` | `Object` | Optional | - | Object getUpdateIfExists() | setUpdateIfExists(Object updateIfExists) |
| `ContactC1` | `String` | Optional | Custom field 1 for api users to store custom data<br><br>**Constraints**: *Maximum Length*: `128` | String getContactC1() | setContactC1(String contactC1) |
| `ContactC2` | `String` | Optional | Custom field 2 for api users to store custom data<br><br>**Constraints**: *Maximum Length*: `128` | String getContactC2() | setContactC2(String contactC2) |
| `ContactC3` | `String` | Optional | Custom field 3 for api users to store custom data<br><br>**Constraints**: *Maximum Length*: `128` | String getContactC3() | setContactC3(String contactC3) |
| `ParentId` | `String` | Optional | Parent Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getParentId() | setParentId(String parentId) |
| `Email` | `String` | Optional | Email of contact<br><br>**Constraints**: *Maximum Length*: `64` | String getEmail() | setEmail(String email) |
| `TokenImportId` | `String` | Optional | Token Import Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getTokenImportId() | setTokenImportId(String tokenImportId) |
| `Id` | `String` | Optional | Contact ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `Active` | `Boolean` | Optional | Active | Boolean getActive() | setActive(Boolean active) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `ReceivedEmails` | [`List<ReceivedEmail>`](../../doc/models/received-email.md) | Optional | Received Email Information on `expand` | List<ReceivedEmail> getReceivedEmails() | setReceivedEmails(List<ReceivedEmail> receivedEmails) |
| `IsDeletable` | `Boolean` | Optional | Is Deletable Information on `expand` | Boolean getIsDeletable() | setIsDeletable(Boolean isDeletable) |
| `Location` | [`Location18`](../../doc/models/location-18.md) | Optional | - | Location18 getLocation() | setLocation(Location18 location) |
| `User` | [`User9`](../../doc/models/user-9.md) | Optional | - | User9 getUser() | setUser(User9 user) |
| `Recurrings` | [`List<Recurring>`](../../doc/models/recurring.md) | Optional | Recurring Information on `expand` | List<Recurring> getRecurrings() | setRecurrings(List<Recurring> recurrings) |
| `EmailBlacklist` | [`EmailBlacklist1`](../../doc/models/email-blacklist-1.md) | Optional | - | EmailBlacklist1 getEmailBlacklist() | setEmailBlacklist(EmailBlacklist1 emailBlacklist) |
| `SmsBlacklist` | [`SmsBlacklist1`](../../doc/models/sms-blacklist-1.md) | Optional | - | SmsBlacklist1 getSmsBlacklist() | setSmsBlacklist(SmsBlacklist1 smsBlacklist) |
| `Changelogs` | [`List<Changelog>`](../../doc/models/changelog.md) | Optional | Changelog Information on `expand` | List<Changelog> getChangelogs() | setChangelogs(List<Changelog> changelogs) |
| `PostbackLogs` | [`List<PostbackLog>`](../../doc/models/postback-log.md) | Optional | Postback Log Information on `expand` | List<PostbackLog> getPostbackLogs() | setPostbackLogs(List<PostbackLog> postbackLogs) |
| `CreatedUser` | [`User9`](../../doc/models/user-9.md) | Optional | - | User9 getCreatedUser() | setCreatedUser(User9 createdUser) |
| `Parent` | [`Parent5`](../../doc/models/parent-5.md) | Optional | - | Parent5 getParent() | setParent(Parent5 parent) |
| `Children` | [`Children1`](../../doc/models/children-1.md) | Optional | - | Children1 getChildren() | setChildren(Children1 children) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "account_number": "54545433332",
  "contact_api_id": "137",
  "first_name": "John",
  "last_name": "Smith",
  "cell_phone": "3339998822",
  "balance": 245.36,
  "company_name": "Fortis Payment Systems, LLC",
  "header_message": "This is a sample message for you",
  "date_of_birth": "2021-12-01",
  "email_trx_receipt": true,
  "home_phone": "3339998822",
  "office_phone": "3339998822",
  "office_phone_ext": "5",
  "home_phone_country_code": "+1",
  "office_phone_country_code": "+1",
  "cell_phone_country_code": "+1",
  "header_message_type": 0,
  "contact_c1": "any",
  "contact_c2": "anything",
  "contact_c3": "something",
  "parent_id": "11e95f8ec39de8fbdb0a4f1a",
  "email": "email@domain.com",
  "token_import_id": "11e95f8ec39de8fbdb0a4f1a",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "active": true,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "is_deletable": true,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

