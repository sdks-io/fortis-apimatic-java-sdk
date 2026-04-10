
# V1 Onboarding Request

*This model accepts additional fields of type Object.*

## Structure

`V1OnboardingRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ParentId` | `String` | Optional | Location ID | String getParentId() | setParentId(String parentId) |
| `PrimaryPrincipal` | [`PrimaryPrincipal2`](../../doc/models/primary-principal-2.md) | Required | - | PrimaryPrincipal2 getPrimaryPrincipal() | setPrimaryPrincipal(PrimaryPrincipal2 primaryPrincipal) |
| `TemplateCode` | `String` | Required | The ID of the template to be used - this value will be provided by Fortis.<br><br>**Constraints**: *Maximum Length*: `20`, *Pattern*: `^[a-zA-Z0-9]*$` | String getTemplateCode() | setTemplateCode(String templateCode) |
| `Email` | `String` | Required | Merchant email address.<br><br>**Constraints**: *Maximum Length*: `100` | String getEmail() | setEmail(String email) |
| `DbaName` | `String` | Required | Merchant 'Doing Business As' name.<br><br>**Constraints**: *Maximum Length*: `100` | String getDbaName() | setDbaName(String dbaName) |
| `Location` | [`Location19`](../../doc/models/location-19.md) | Required | - | Location19 getLocation() | setLocation(Location19 location) |
| `AppDelivery` | [`AppDelivery`](../../doc/models/app-delivery.md) | Required | **Constraints**: *Maximum Length*: `12` | AppDelivery getAppDelivery() | setAppDelivery(AppDelivery appDelivery) |
| `BusinessCategory` | `Object` | Optional | - | Object getBusinessCategory() | setBusinessCategory(Object businessCategory) |
| `BusinessType` | `Object` | Optional | - | Object getBusinessType() | setBusinessType(Object businessType) |
| `BusinessDescription` | `String` | Optional | Description of Goods or Services.<br><br>**Constraints**: *Maximum Length*: `200` | String getBusinessDescription() | setBusinessDescription(String businessDescription) |
| `SwipedPercent` | `Integer` | Optional | Card present/swiped percentage<br><br>> The sum total of "swiped_percent", "keyed_percent" and "ecommerce_percent" must add up to 100.<br><br>**Constraints**: `>= 0`, `<= 100` | Integer getSwipedPercent() | setSwipedPercent(Integer swipedPercent) |
| `KeyedPercent` | `Integer` | Optional | Card not present/keyed percentage<br><br>> The sum total of "swiped_percent", "keyed_percent" and "ecommerce_percent" must add up to 100.<br><br>**Constraints**: `>= 0`, `<= 100` | Integer getKeyedPercent() | setKeyedPercent(Integer keyedPercent) |
| `EcommercePercent` | `Integer` | Optional | eCommerce percentage.<br><br>> The sum total of "swiped_percent", "keyed_percent" and "ecommerce_percent" must add up to 100.<br><br>**Constraints**: `>= 0`, `<= 100` | Integer getEcommercePercent() | setEcommercePercent(Integer ecommercePercent) |
| `OwnershipType` | `Object` | Optional | - | Object getOwnershipType() | setOwnershipType(Object ownershipType) |
| `FedTaxId` | `String` | Optional | Federal Tax ID (EIN).<br><br>**Constraints**: *Maximum Length*: `10` | String getFedTaxId() | setFedTaxId(String fedTaxId) |
| `CcAverageTicketRange` | `Integer` | Optional | Average Transaction Amount Range<br><br>> (Applicable when Template Application Type is 'credit_card' or 'both').<br><br>**Constraints**: `>= 1`, `<= 7` | Integer getCcAverageTicketRange() | setCcAverageTicketRange(Integer ccAverageTicketRange) |
| `CcMonthlyVolumeRange` | `Integer` | Optional | Monthly Processing Volume Range<br><br>> (Applicable when Template Application Type is 'credit_card' or 'both').<br><br>**Constraints**: `>= 1`, `<= 7` | Integer getCcMonthlyVolumeRange() | setCcMonthlyVolumeRange(Integer ccMonthlyVolumeRange) |
| `CcHighTicket` | `Integer` | Optional | Highest transaction amount rounded to the next dollar<br><br>> (No decimal and applicable when Template Application Type is 'credit_card' or 'both').<br><br>**Constraints**: `>= 0`, `<= 30000` | Integer getCcHighTicket() | setCcHighTicket(Integer ccHighTicket) |
| `EcAverageTicketRange` | `Integer` | Optional | Average Transaction Amount Range<br><br>> (Applicable when Template Application Type is 'echeck' or 'both').<br><br>**Constraints**: `>= 1`, `<= 7` | Integer getEcAverageTicketRange() | setEcAverageTicketRange(Integer ecAverageTicketRange) |
| `EcMonthlyVolumeRange` | `Integer` | Optional | Monthly Processing Volume Range<br><br>> (Applicable when Template Application Type is 'echeck' or 'both').<br><br>**Constraints**: `>= 1`, `<= 7` | Integer getEcMonthlyVolumeRange() | setEcMonthlyVolumeRange(Integer ecMonthlyVolumeRange) |
| `EcHighTicket` | `Integer` | Optional | Highest transaction amount rounded to the next dollar<br><br>> (No decimal and applicable when Template Application Type is 'echeck' or 'both').<br><br>**Constraints**: `>= 0`, `<= 30000` | Integer getEcHighTicket() | setEcHighTicket(Integer ecHighTicket) |
| `Website` | `String` | Optional | Merchant's business website.<br><br>> (Required if "ecommerce_percent" is greater than 0).<br><br>**Constraints**: *Maximum Length*: `100` | String getWebsite() | setWebsite(String website) |
| `BankAccount` | [`BankAccount3`](../../doc/models/bank-account-3.md) | Optional | - | BankAccount3 getBankAccount() | setBankAccount(BankAccount3 bankAccount) |
| `AltBankAccount` | [`AltBankAccount2`](../../doc/models/alt-bank-account-2.md) | Optional | - | AltBankAccount2 getAltBankAccount() | setAltBankAccount(AltBankAccount2 altBankAccount) |
| `LegalName` | `String` | Optional | Merchant legal name.<br><br>> (leave blank if same as DBA name).<br><br>**Constraints**: *Maximum Length*: `100` | String getLegalName() | setLegalName(String legalName) |
| `Contact` | [`Contact13`](../../doc/models/contact-13.md) | Required | - | Contact13 getContact() | setContact(Contact13 contact) |
| `ClientAppId` | `String` | Optional | Client Issues Id to track that can be used to track each submitted merchant application. This id should be generated and sent in the request payload, and will be returned in the response payload. If no id is submitted in the payload request, this field will be null in the response.<br><br>**Constraints**: *Maximum Length*: `50` | String getClientAppId() | setClientAppId(String clientAppId) |
| `SecCodes` | [`List<SecCode>`](../../doc/models/sec-code.md) | Optional | Array of SEC codes that will be allowed, Only applicable for ACH. Valid values are 'PPD', 'WEB', 'TEL', 'CCD'. | List<SecCode> getSecCodes() | setSecCodes(List<SecCode> secCodes) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

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
    "phone_number": "555-555-1234",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
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
    "phone_number": "555-555-1212",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "app_delivery": "direct",
  "swiped_percent": 0,
  "keyed_percent": 0,
  "ecommerce_percent": 100,
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
    "phone_number": "555-555-3456",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "client_app_id": "ABC123",
  "parent_id": "parent_id8",
  "business_category": {
    "key1": "val1",
    "key2": "val2"
  },
  "business_type": {
    "key1": "val1",
    "key2": "val2"
  },
  "business_description": "business_description0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

