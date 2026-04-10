
# Identity Verification 1

*This model accepts additional fields of type Object.*

## Structure

`IdentityVerification1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `DlState` | `String` | Optional | Required for ACH transactions when Driver's License Verification is enabled on the terminal.  Either dl_number + dl_state OR customer_id will need to be passed in this scenario.<br><br>**Constraints**: *Minimum Length*: `2`, *Maximum Length*: `2` | String getDlState() | setDlState(String dlState) |
| `DlNumber` | `String` | Optional | Required for ACH transactions when Driver's License Verification is enabled on the terminal.  Either dl_number + dl_state OR customer_id will need to be passed in this scenario.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `50` | String getDlNumber() | setDlNumber(String dlNumber) |
| `DobYear` | `String` | Optional | Required for certain ACH transactions where Identity Verification has been enabled for the terminal.  Either ssn4 or dob_year will need to be passed in this scenario but NOT BOTH.<br><br>**Constraints**: *Minimum Length*: `4`, *Maximum Length*: `4`, *Pattern*: `^(19\d{2})\|20\d{2}$` | String getDobYear() | setDobYear(String dobYear) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "dl_state": "MI",
  "dl_number": "1235567",
  "dob_year": "1980",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

