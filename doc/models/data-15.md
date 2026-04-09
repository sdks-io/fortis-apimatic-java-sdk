
# Data 15

## Structure

`Data15`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ParentId` | `String` | Optional | Location ID | String getParentId() | setParentId(String parentId) |
| `PrimaryPrincipal` | [`PrimaryPrincipal`](../../doc/models/primary-principal.md) | Optional | The Primary Principal. | PrimaryPrincipal getPrimaryPrincipal() | setPrimaryPrincipal(PrimaryPrincipal primaryPrincipal) |
| `TemplateCode` | `String` | Optional | The ID of the template to be used - this value will be provided by Fortis.<br><br>**Constraints**: *Maximum Length*: `20`, *Pattern*: `^[a-zA-Z0-9]*$` | String getTemplateCode() | setTemplateCode(String templateCode) |
| `Email` | `String` | Optional | Merchant email address.<br><br>**Constraints**: *Maximum Length*: `100` | String getEmail() | setEmail(String email) |
| `DbaName` | `String` | Optional | Merchant 'Doing Business As' name.<br><br>**Constraints**: *Maximum Length*: `100` | String getDbaName() | setDbaName(String dbaName) |
| `Location` | [`Location5`](../../doc/models/location-5.md) | Optional | The Location. | Location5 getLocation() | setLocation(Location5 location) |
| `AppDelivery` | `String` | Optional | The delivery method of the app to the merchant.<br><br>**Constraints**: *Maximum Length*: `20` | String getAppDelivery() | setAppDelivery(String appDelivery) |
| `BusinessCategory` | [`BusinessCategoryEnum`](../../doc/models/business-category-enum.md) | Optional | The Category of the merchant's business<br><br>> (Required if "business_type" is provided). Note: "business_type" must belong to the appropriate "business_category" | BusinessCategoryEnum getBusinessCategory() | setBusinessCategory(BusinessCategoryEnum businessCategory) |
| `BusinessType` | [`BusinessTypeEnum`](../../doc/models/business-type-enum.md) | Optional | The Type of a merchant's business. | BusinessTypeEnum getBusinessType() | setBusinessType(BusinessTypeEnum businessType) |
| `BusinessDescription` | `String` | Optional | Description of Goods or Services.<br><br>**Constraints**: *Maximum Length*: `200` | String getBusinessDescription() | setBusinessDescription(String businessDescription) |
| `SwipedPercent` | `Integer` | Optional | Card present/swiped percentage<br><br>> The sum total of "swiped_percent", "keyed_percent" and "ecommerce_percent" must add up to 100.<br><br>**Constraints**: `>= 0`, `<= 100` | Integer getSwipedPercent() | setSwipedPercent(Integer swipedPercent) |
| `KeyedPercent` | `Integer` | Optional | Card not present/keyed percentage<br><br>> The sum total of "swiped_percent", "keyed_percent" and "ecommerce_percent" must add up to 100.<br><br>**Constraints**: `>= 0`, `<= 100` | Integer getKeyedPercent() | setKeyedPercent(Integer keyedPercent) |
| `EcommercePercent` | `Integer` | Optional | eCommerce percentage.<br><br>> The sum total of "swiped_percent", "keyed_percent" and "ecommerce_percent" must add up to 100.<br><br>**Constraints**: `>= 0`, `<= 100` | Integer getEcommercePercent() | setEcommercePercent(Integer ecommercePercent) |
| `OwnershipType` | [`OwnershipTypeEnum`](../../doc/models/ownership-type-enum.md) | Optional | The Ownership Type of the merchant's business.<br><br>**Constraints**: *Maximum Length*: `10` | OwnershipTypeEnum getOwnershipType() | setOwnershipType(OwnershipTypeEnum ownershipType) |
| `FedTaxId` | `String` | Optional | Federal Tax ID (EIN).<br><br>**Constraints**: *Maximum Length*: `10` | String getFedTaxId() | setFedTaxId(String fedTaxId) |
| `CcAverageTicketRange` | `Integer` | Optional | Average Transaction Amount Range<br><br>> (Applicable when Template Application Type is 'credit_card' or 'both').<br><br>**Constraints**: `>= 1`, `<= 7` | Integer getCcAverageTicketRange() | setCcAverageTicketRange(Integer ccAverageTicketRange) |
| `CcMonthlyVolumeRange` | `Integer` | Optional | Monthly Processing Volume Range<br><br>> (Applicable when Template Application Type is 'credit_card' or 'both').<br><br>**Constraints**: `>= 1`, `<= 7` | Integer getCcMonthlyVolumeRange() | setCcMonthlyVolumeRange(Integer ccMonthlyVolumeRange) |
| `CcHighTicket` | `Integer` | Optional | Highest transaction amount rounded to the next dollar<br><br>> (No decimal and applicable when Template Application Type is 'credit_card' or 'both').<br><br>**Constraints**: `>= 0`, `<= 30000` | Integer getCcHighTicket() | setCcHighTicket(Integer ccHighTicket) |
| `EcAverageTicketRange` | `Integer` | Optional | Average Transaction Amount Range<br><br>> (Applicable when Template Application Type is 'echeck' or 'both').<br><br>**Constraints**: `>= 1`, `<= 7` | Integer getEcAverageTicketRange() | setEcAverageTicketRange(Integer ecAverageTicketRange) |
| `EcMonthlyVolumeRange` | `Integer` | Optional | Monthly Processing Volume Range<br><br>> (Applicable when Template Application Type is 'echeck' or 'both').<br><br>**Constraints**: `>= 1`, `<= 7` | Integer getEcMonthlyVolumeRange() | setEcMonthlyVolumeRange(Integer ecMonthlyVolumeRange) |
| `EcHighTicket` | `Integer` | Optional | Highest transaction amount rounded to the next dollar<br><br>> (No decimal and applicable when Template Application Type is 'echeck' or 'both').<br><br>**Constraints**: `>= 0`, `<= 30000` | Integer getEcHighTicket() | setEcHighTicket(Integer ecHighTicket) |
| `Website` | `String` | Optional | Merchant's business website.<br><br>> (Required if "ecommerce_percent" is greater than 0).<br><br>**Constraints**: *Maximum Length*: `100` | String getWebsite() | setWebsite(String website) |
| `BankAccount` | [`BankAccount`](../../doc/models/bank-account.md) | Optional | The Bank Account. | BankAccount getBankAccount() | setBankAccount(BankAccount bankAccount) |
| `AltBankAccount` | [`AltBankAccount`](../../doc/models/alt-bank-account.md) | Optional | The Alternative Bank Account. | AltBankAccount getAltBankAccount() | setAltBankAccount(AltBankAccount altBankAccount) |
| `LegalName` | `String` | Optional | Merchant legal name.<br><br>> (leave blank if same as DBA name).<br><br>**Constraints**: *Maximum Length*: `100` | String getLegalName() | setLegalName(String legalName) |
| `Contact` | [`Contact`](../../doc/models/contact.md) | Optional | The Contact. | Contact getContact() | setContact(Contact contact) |
| `ClientAppId` | `String` | Optional | Client Issues Id to track that can be used to track each submitted merchant application. This id should be generated and sent in the request payload, and will be returned in the response payload. If no id is submitted in the payload request, this field will be null in the response.<br><br>**Constraints**: *Maximum Length*: `20` | String getClientAppId() | setClientAppId(String clientAppId) |
| `SecCodes` | [`List<SecCodeEnum>`](../../doc/models/sec-code-enum.md) | Optional | Array of SEC codes that will be allowed, Only applicable for ACH. Valid values are 'PPD', 'WEB', 'TEL', 'CCD'. | List<SecCodeEnum> getSecCodes() | setSecCodes(List<SecCodeEnum> secCodes) |
| `AppLink` | `String` | Optional | A full page or iframeable link, set in the request app_delivery field, that can be used to retrieve and resume the generated merchant application. No link will be returned if app_delivery is direct<br><br>**Constraints**: *Maximum Length*: `400` | String getAppLink() | setAppLink(String appLink) |

## Example (as JSON)

```json
{
  "template_code": "1234YourTemplateCode",
  "email": "jtodd@example.com",
  "dba_name": "Discount Home Goods",
  "app_delivery": "link_full_page",
  "business_category": "education",
  "swiped_percent": 0,
  "keyed_percent": 0,
  "ecommerce_percent": 100,
  "ownership_type": "llp",
  "fed_tax_id": "0000000000",
  "cc_average_ticket_range": 5,
  "cc_monthly_volume_range": 1,
  "cc_high_ticket": 1500,
  "ec_average_ticket_range": 5,
  "ec_monthly_volume_range": 2,
  "ec_high_ticket": 1500,
  "website": "http://www.example.com",
  "legal_name": "Total Home Goods, LLP",
  "client_app_id": "ABC123",
  "app_link": "https://mpa.example.com/signup/123456788",
  "parent_id": "parent_id0",
  "primary_principal": {
    "first_name": "first_name6",
    "last_name": "last_name4",
    "middle_name": "middle_name6",
    "title": "title2",
    "date_of_birth": "date_of_birth2"
  }
}
```

