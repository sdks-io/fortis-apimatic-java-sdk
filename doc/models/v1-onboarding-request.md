
# V1 Onboarding Request

## Structure

`V1OnboardingRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ParentId` | `String` | Optional | Location ID | String getParentId() | setParentId(String parentId) |
| `PrimaryPrincipal` | [`PrimaryPrincipal1`](../../doc/models/primary-principal-1.md) | Required | The Primary Principal. | PrimaryPrincipal1 getPrimaryPrincipal() | setPrimaryPrincipal(PrimaryPrincipal1 primaryPrincipal) |
| `TemplateCode` | `String` | Required | The ID of the template to be used - this value will be provided by Fortis.<br><br>**Constraints**: *Maximum Length*: `20`, *Pattern*: `^[a-zA-Z0-9]*$` | String getTemplateCode() | setTemplateCode(String templateCode) |
| `Email` | `String` | Required | Merchant email address.<br><br>**Constraints**: *Maximum Length*: `100` | String getEmail() | setEmail(String email) |
| `DbaName` | `String` | Required | Merchant 'Doing Business As' name.<br><br>**Constraints**: *Maximum Length*: `100` | String getDbaName() | setDbaName(String dbaName) |
| `Location` | [`Location20`](../../doc/models/location-20.md) | Required | The Location. | Location20 getLocation() | setLocation(Location20 location) |
| `AppDelivery` | [`AppDeliveryEnum`](../../doc/models/app-delivery-enum.md) | Required | The delivery method of the app to the merchant.<br><br>**Constraints**: *Maximum Length*: `12` | AppDeliveryEnum getAppDelivery() | setAppDelivery(AppDeliveryEnum appDelivery) |
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
| `Contact` | [`Contact11`](../../doc/models/contact-11.md) | Required | The Contact. | Contact11 getContact() | setContact(Contact11 contact) |
| `ClientAppId` | `String` | Optional | Client Issues Id to track that can be used to track each submitted merchant application. This id should be generated and sent in the request payload, and will be returned in the response payload. If no id is submitted in the payload request, this field will be null in the response.<br><br>**Constraints**: *Maximum Length*: `50` | String getClientAppId() | setClientAppId(String clientAppId) |
| `SecCodes` | [`List<SecCodeEnum>`](../../doc/models/sec-code-enum.md) | Optional | Array of SEC codes that will be allowed, Only applicable for ACH. Valid values are 'PPD', 'WEB', 'TEL', 'CCD'. | List<SecCodeEnum> getSecCodes() | setSecCodes(List<SecCodeEnum> secCodes) |

## Example (as JSON)

```json
{
  "primary_principal": {
    "first_name": "Bob",
    "last_name": "Fairview",
    "middle_name": "Nathaniel",
    "title": "Dr",
    "date_of_birth": "2021-12-01",
    "address_line_1": "1354 Oak St.",
    "address_line_2": "Unit 203",
    "city": "Dover",
    "state_province": "DE",
    "postal_code": "55022",
    "ownership_percent": 100,
    "phone_number": "555-555-1234"
  },
  "template_code": "1234YourTemplateCode",
  "email": "email@domain.com",
  "dba_name": "Discount Home Goods",
  "location": {
    "address_line_1": "1200 West Hartford Pkwy",
    "address_line_2": "Suite 2000",
    "city": "Dover",
    "state_province": "DE",
    "postal_code": "55022",
    "phone_number": "555-555-1212"
  },
  "app_delivery": null,
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
  "contact": {
    "first_name": "Jeffery",
    "last_name": "Todd",
    "email": "jtodd@example.com",
    "phone_number": "555-555-3456"
  },
  "client_app_id": "ABC123",
  "parent_id": "parent_id2",
  "business_type": "books_mags_music_and_video",
  "business_description": "business_description0"
}
```

