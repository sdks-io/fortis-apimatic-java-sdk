
# Account Vault Cau Product Transaction

*This model accepts additional fields of type Object.*

## Structure

`AccountVaultCauProductTransaction`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `String` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `AccountNumber` | `String` | Optional | Account number<br><br>**Constraints**: *Maximum Length*: `32`, *Pattern*: `^[a-zA-Z0-9\-_]+$` | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `Address` | [`Address6`](../../doc/models/address-6.md) | Optional | - | Address6 getAddress() | setAddress(Address6 address) |
| `BrandingDomainId` | `String` | Optional | GUID for Branding Domain<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getBrandingDomainId() | setBrandingDomainId(String brandingDomainId) |
| `ContactEmailTrxReceiptDefault` | `Boolean` | Optional | If true, will email contact receipt for any transaction | Boolean getContactEmailTrxReceiptDefault() | setContactEmailTrxReceiptDefault(Boolean contactEmailTrxReceiptDefault) |
| `DefaultAch` | `String` | Optional | GUID for Location's default ACH Product Transaction<br><br>**Constraints**: *Minimum Length*: `24`, *Maximum Length*: `36` | String getDefaultAch() | setDefaultAch(String defaultAch) |
| `DefaultCc` | `String` | Optional | GUID for Location's default CC Product Transaction<br><br>**Constraints**: *Minimum Length*: `24`, *Maximum Length*: `36` | String getDefaultCc() | setDefaultCc(String defaultCc) |
| `EmailReplyTo` | `String` | Optional | Used as from email address when sending various notifications<br><br>**Constraints**: *Maximum Length*: `64` | String getEmailReplyTo() | setEmailReplyTo(String emailReplyTo) |
| `Fax` | `String` | Optional | Fax number<br><br>**Constraints**: *Minimum Length*: `10`, *Maximum Length*: `10`, *Pattern*: `^\d{10}$` | String getFax() | setFax(String fax) |
| `LocationApiId` | `String` | Optional | Location api ID<br><br>**Constraints**: *Maximum Length*: `36` | String getLocationApiId() | setLocationApiId(String locationApiId) |
| `LocationApiKey` | `String` | Optional | Location api key<br><br>**Constraints**: *Maximum Length*: `36` | String getLocationApiKey() | setLocationApiKey(String locationApiKey) |
| `LocationC1` | `String` | Optional | Can be used to store custom information for location.<br><br>**Constraints**: *Maximum Length*: `128` | String getLocationC1() | setLocationC1(String locationC1) |
| `LocationC2` | `String` | Optional | Can be used to store custom information for location.<br><br>**Constraints**: *Maximum Length*: `128` | String getLocationC2() | setLocationC2(String locationC2) |
| `LocationC3` | `String` | Optional | Can be used to store custom information for location.<br><br>**Constraints**: *Maximum Length*: `128` | String getLocationC3() | setLocationC3(String locationC3) |
| `Name` | `String` | Optional | Name of the company<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `64` | String getName() | setName(String name) |
| `OfficePhone` | `String` | Optional | Office phone number<br><br>**Constraints**: *Minimum Length*: `10`, *Maximum Length*: `10` | String getOfficePhone() | setOfficePhone(String officePhone) |
| `OfficeExtPhone` | `String` | Optional | Office phone extension number<br><br>**Constraints**: *Maximum Length*: `10` | String getOfficeExtPhone() | setOfficeExtPhone(String officeExtPhone) |
| `Tz` | `String` | Optional | Time zone<br><br>**Constraints**: *Maximum Length*: `30` | String getTz() | setTz(String tz) |
| `ParentId` | `String` | Optional | Location GUID of the parent location<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getParentId() | setParentId(String parentId) |
| `ShowContactNotes` | `Boolean` | Optional | If set to true will show 'Notes' tab on Contact | Boolean getShowContactNotes() | setShowContactNotes(Boolean showContactNotes) |
| `ShowContactFiles` | `Boolean` | Optional | If set to true will show 'Files' tab on Contact | Boolean getShowContactFiles() | setShowContactFiles(Boolean showContactFiles) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `LocationType` | `Object` | Optional | - | Object getLocationType() | setLocationType(Object locationType) |
| `ParentName` | `String` | Optional | Name of the parent location | String getParentName() | setParentName(String parentName) |
| `TicketHashKey` | `String` | Optional | Ticket Hash Key<br><br>**Constraints**: *Maximum Length*: `36` | String getTicketHashKey() | setTicketHashKey(String ticketHashKey) |
| `AdditionalAccess` | [`AdditionalAccess`](../../doc/models/additional-access.md) | Optional | - | AdditionalAccess getAdditionalAccess() | setAdditionalAccess(AdditionalAccess additionalAccess) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "account_number": "5454545454545454",
  "branding_domain_id": "11e95f8ec39de8fbdb0a4f1a",
  "contact_email_trx_receipt_default": true,
  "default_ach": "11e608a7d515f1e093242bb2",
  "default_cc": "11e608a442a5f1e092242dda",
  "email_reply_to": "email@domain.com",
  "fax": "3339998822",
  "location_api_id": "location-111111",
  "location_api_key": "AE34BBCAADF4AE34BBCAADF4",
  "location_c1": "custom 1",
  "location_c2": "custom 2",
  "location_c3": "custom data 3",
  "name": "Sample Company Headquarters",
  "office_phone": "2481234567",
  "office_ext_phone": "1021021209",
  "tz": "America/New_York",
  "parent_id": "11e95f8ec39de8fbdb0a4f1a",
  "show_contact_notes": true,
  "show_contact_files": true,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "ticket_hash_key": "A5F443CADF4AE34BBCAADF4",
  "address": {
    "city": "city6",
    "state": "state2",
    "postal_code": "postal_code8",
    "country": {
      "key1": "val1",
      "key2": "val2"
    },
    "street": "street6",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

