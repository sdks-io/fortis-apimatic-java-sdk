
# User 4

*This model accepts additional fields of type Object.*

## Structure

`User4`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `String` | Optional | ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `Username` | `String` | Optional | Username | String getUsername() | setUsername(String username) |
| `FirstName` | `String` | Optional | First Name | String getFirstName() | setFirstName(String firstName) |
| `LastName` | `String` | Optional | Last Name | String getLastName() | setLastName(String lastName) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "username": "email@domain.com",
  "first_name": "Bob",
  "last_name": "Fairview",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

