
# Result

*This model accepts additional fields of type Object.*

## Structure

`Result`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ClientAppId` | `String` | Optional | Client Issues Id to track that can be used to track each submitted merchant application. This id should be generated and sent in the request payload, and will be returned in the response payload. If no id is submitted in the payload request, this field will be null in the response.<br><br>**Constraints**: *Maximum Length*: `50` | String getClientAppId() | setClientAppId(String clientAppId) |
| `DbaName` | `String` | Optional | Merchant 'Doing Business As' name.<br><br>**Constraints**: *Maximum Length*: `100` | String getDbaName() | setDbaName(String dbaName) |
| `Email` | `String` | Optional | Merchant email address.<br><br>**Constraints**: *Maximum Length*: `100` | String getEmail() | setEmail(String email) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "client_app_id": "ABC123",
  "dba_name": "Discount Home Goods",
  "email": "jtodd@example.com",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

