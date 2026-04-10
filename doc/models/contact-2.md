
# Contact 2

*This model accepts additional fields of type Object.*

## Structure

`Contact2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `FirstName` | `String` | Optional | Contact's first name.<br><br>**Constraints**: *Maximum Length*: `20` | String getFirstName() | setFirstName(String firstName) |
| `LastName` | `String` | Optional | Contact's last name.<br><br>**Constraints**: *Maximum Length*: `20` | String getLastName() | setLastName(String lastName) |
| `Email` | `String` | Optional | Contact's email address.<br><br>**Constraints**: *Maximum Length*: `100` | String getEmail() | setEmail(String email) |
| `PhoneNumber` | `String` | Optional | Contact's phone.<br><br>**Constraints**: *Maximum Length*: `20` | String getPhoneNumber() | setPhoneNumber(String phoneNumber) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "first_name": "Jeffery",
  "last_name": "Todd",
  "email": "jtodd@example.com",
  "phone_number": "555-555-3456",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

