
# Kyc Response Object

Array of KYC response objects.

*This model accepts additional fields of type Object.*

## Structure

`KycResponseObject`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Value` | `String` | Required | KYC object value. | String getValue() | setValue(String value) |
| `Type` | `String` | Required | KYC oject type.<br><br>**Constraints**: *Maximum Length*: `32` | String getType() | setType(String type) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "value": "KYC value.",
  "type": "KYC type",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

