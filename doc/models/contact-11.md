
# Contact 11

The Contact.

## Structure

`Contact11`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `FirstName` | `String` | Optional | Contact's first name.<br><br>**Constraints**: *Maximum Length*: `20` | String getFirstName() | setFirstName(String firstName) |
| `LastName` | `String` | Optional | Contact's last name.<br><br>**Constraints**: *Maximum Length*: `20` | String getLastName() | setLastName(String lastName) |
| `Email` | `String` | Optional | Contact's email address.<br><br>**Constraints**: *Maximum Length*: `100` | String getEmail() | setEmail(String email) |
| `PhoneNumber` | `String` | Required | Contact's phone.<br><br>**Constraints**: *Maximum Length*: `20` | String getPhoneNumber() | setPhoneNumber(String phoneNumber) |

## Example (as JSON)

```json
{
  "first_name": "Jeffery",
  "last_name": "Todd",
  "email": "jtodd@example.com",
  "phone_number": "555-555-3456"
}
```

