
# Owner

Array of merchant owners.

## Structure

`Owner`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `FirstName` | `String` | Required | Owner's first name.<br><br>**Constraints**: *Maximum Length*: `20` | String getFirstName() | setFirstName(String firstName) |
| `LastName` | `String` | Required | Owner's last name.<br><br>**Constraints**: *Maximum Length*: `20` | String getLastName() | setLastName(String lastName) |
| `MiddleName` | `String` | Optional | Owner's middle name.<br><br>**Constraints**: *Maximum Length*: `20` | String getMiddleName() | setMiddleName(String middleName) |
| `Title` | `String` | Required | Owner's title.<br><br>**Constraints**: *Maximum Length*: `20` | String getTitle() | setTitle(String title) |
| `DateOfBirth` | `String` | Required | Owner's date of birth.<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getDateOfBirth() | setDateOfBirth(String dateOfBirth) |
| `AddressLine1` | `String` | Required | Owner's street address.<br><br>**Constraints**: *Maximum Length*: `100` | String getAddressLine1() | setAddressLine1(String addressLine1) |
| `AddressLine2` | `String` | Required | Line 2 of owner's address.<br><br>**Constraints**: *Maximum Length*: `20` | String getAddressLine2() | setAddressLine2(String addressLine2) |
| `City` | `String` | Required | Owner's address city.<br><br>**Constraints**: *Maximum Length*: `50` | String getCity() | setCity(String city) |
| `StateProvince` | `String` | Required | Owner's address state/province.<br><br>**Constraints**: *Maximum Length*: `2` | String getStateProvince() | setStateProvince(String stateProvince) |
| `PostalCode` | `String` | Required | Owner's address postal code.<br><br>**Constraints**: *Maximum Length*: `10` | String getPostalCode() | setPostalCode(String postalCode) |
| `CountryCode` | `String` | Required | Owner's address country.<br><br>**Constraints**: *Maximum Length*: `2` | String getCountryCode() | setCountryCode(String countryCode) |
| `Ssn` | `String` | Required | Owner's full SSN.<br><br>**Constraints**: *Maximum Length*: `10` | String getSsn() | setSsn(String ssn) |
| `OwnershipPercent` | `int` | Required | Owner's ownership percent.<br><br>**Constraints**: `>= 0`, `<= 100` | int getOwnershipPercent() | setOwnershipPercent(int ownershipPercent) |
| `PhoneNumber` | `String` | Required | Owner's phone number.<br><br>**Constraints**: *Maximum Length*: `20` | String getPhoneNumber() | setPhoneNumber(String phoneNumber) |
| `EmailAddress` | `String` | Required | Owner's email address.<br><br>**Constraints**: *Maximum Length*: `100` | String getEmailAddress() | setEmailAddress(String emailAddress) |
| `IsController` | `boolean` | Required | Flag indicating whether this owner is the control owner. Maximum of 1 owner can be marked as control..<br><br>> Flag indicating whether this owner is the control owner. Maximum of 1 owner can be marked as control. | boolean getIsController() | setIsController(boolean isController) |
| `IsSigner` | `boolean` | Required | Flag indicating whether or not the owner is a signer for the business. Maximum of 1 owner can be marked as signer.<br><br>> Flag indicating whether or not the owner is a signer for the business. Maximum of 1 owner can be marked as signer. | boolean getIsSigner() | setIsSigner(boolean isSigner) |

## Example (as JSON)

```json
{
  "first_name": "James",
  "last_name": "Bond",
  "middle_name": "Tyler",
  "title": "CEO",
  "date_of_birth": "2021-12-01",
  "address_line_1": "133 S Goliad St",
  "address_line_2": "Suite 120",
  "city": "Rockwall",
  "state_province": "TX",
  "postal_code": "75429",
  "country_code": "US",
  "ssn": "000000000",
  "ownership_percent": 100,
  "phone_number": "9042142323",
  "email_address": "james@example.com",
  "is_controller": true,
  "is_signer": true
}
```

