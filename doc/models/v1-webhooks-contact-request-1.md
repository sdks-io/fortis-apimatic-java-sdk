
# V1 Webhooks Contact Request 1

*This model accepts additional fields of type Object.*

## Structure

`V1WebhooksContactRequest1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AttemptInterval` | `Integer` | Optional | Number of seconds before another retry is submitted<br><br>**Default**: `300`<br><br>**Constraints**: `>= 300`, `<= 86400` | Integer getAttemptInterval() | setAttemptInterval(Integer attemptInterval) |
| `BasicAuthUsername` | `String` | Optional | The Basic authorization username for the URL, if not supplied, the postback will be submitted without Basic authorization headers<br><br>> This is only expandable for response but settable in the POST/PUT request<br><br>**Constraints**: *Maximum Length*: `512` | String getBasicAuthUsername() | setBasicAuthUsername(String basicAuthUsername) |
| `BasicAuthPassword` | `String` | Optional | The basic authorization password<br><br>> This is only expandable for response but settable in the POST/PUT request<br><br>**Constraints**: *Maximum Length*: `512` | String getBasicAuthPassword() | setBasicAuthPassword(String basicAuthPassword) |
| `Expands` | `String` | Optional | An option list of expanded data to send with base data. (i.e. set this field to “contact,account_vault” to get the contact an accountvault used to run a transaction.)<br><br>**Constraints**: *Maximum Length*: `512` | String getExpands() | setExpands(String expands) |
| `Format` | `Object` | Optional | - | Object getFormat() | setFormat(Object format) |
| `IsActive` | `Boolean` | Optional | Flag to indicate whether configuration is active (in effect). | Boolean getIsActive() | setIsActive(Boolean isActive) |
| `LocationId` | `String` | Optional | The location identifier of the resource you want to recieve postbacks from.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `LocationApiId` | `String` | Optional | Location Api ID | String getLocationApiId() | setLocationApiId(String locationApiId) |
| `OnCreate` | `Boolean` | Optional | To receive postbacks on the creation of a resource | Boolean getOnCreate() | setOnCreate(Boolean onCreate) |
| `OnUpdate` | `Boolean` | Optional | To receive postbacks on the updating of a resource | Boolean getOnUpdate() | setOnUpdate(Boolean onUpdate) |
| `OnDelete` | `Boolean` | Optional | To receive postbacks when the record is deleted | Boolean getOnDelete() | setOnDelete(Boolean onDelete) |
| `Legacy` | `Boolean` | Optional | Prefer the legacy api format.<br><br>**Default**: `true` | Boolean getLegacy() | setLegacy(Boolean legacy) |
| `PostbackConfigId` | `String` | Optional | Postback Config ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getPostbackConfigId() | setPostbackConfigId(String postbackConfigId) |
| `ProductTransactionId` | `String` | Optional | Required when using 'transaction' or 'transactionbatch' resource<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getProductTransactionId() | setProductTransactionId(String productTransactionId) |
| `Resource` | `Object` | Optional | - | Object getResource() | setResource(Object resource) |
| `NumberOfAttempts` | `Integer` | Optional | Maximum number of attempts on failure<br><br>**Constraints**: `>= 1`, `<= 5` | Integer getNumberOfAttempts() | setNumberOfAttempts(Integer numberOfAttempts) |
| `Url` | `String` | Optional | The URL where the postback will be submitted<br><br>**Constraints**: *Maximum Length*: `512` | String getUrl() | setUrl(String url) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "attempt_interval": 300,
  "basic_auth_username": "tester",
  "basic_auth_password": "Test@522",
  "expands": "changelogs,tags",
  "is_active": true,
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "on_create": true,
  "on_update": true,
  "on_delete": true,
  "legacy": true,
  "postback_config_id": "11e95f8ec39de8fbdb0a4f1a",
  "product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "number_of_attempts": 1,
  "url": "https://127.0.0.1/receiver",
  "format": {
    "key1": "val1",
    "key2": "val2"
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

