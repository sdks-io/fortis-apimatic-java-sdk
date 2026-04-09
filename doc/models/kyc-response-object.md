
# Kyc Response Object

Array of KYC response objects.

## Structure

`KycResponseObject`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Value` | `String` | Required | KYC object value. | String getValue() | setValue(String value) |
| `Type` | `String` | Required | KYC oject type.<br><br>**Constraints**: *Maximum Length*: `32` | String getType() | setType(String type) |

## Example (as JSON)

```json
{
  "value": "KYC value.",
  "type": "KYC type"
}
```

