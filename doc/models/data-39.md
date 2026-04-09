
# Data 39

## Structure

`Data39`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AttemptInterval` | `Integer` | Optional | Number of seconds before another retry is submitted<br><br>**Default**: `300`<br><br>**Constraints**: `>= 300`, `<= 86400` | Integer getAttemptInterval() | setAttemptInterval(Integer attemptInterval) |
| `BasicAuthUsername` | `String` | Optional | Basic Auth Username Information on `expand` | String getBasicAuthUsername() | setBasicAuthUsername(String basicAuthUsername) |
| `BasicAuthPassword` | `String` | Optional | Basic Auth Password Information on `expand` | String getBasicAuthPassword() | setBasicAuthPassword(String basicAuthPassword) |
| `Expands` | `String` | Optional | An option list of expanded data to send with base data. (i.e. set this field to “contact,account_vault” to get the contact an accountvault used to run a transaction.)<br><br>**Constraints**: *Maximum Length*: `512` | String getExpands() | setExpands(String expands) |
| `Format` | [`FormatEnum`](../../doc/models/format-enum.md) | Optional | Options include: api-default | FormatEnum getFormat() | setFormat(FormatEnum format) |
| `IsActive` | `Boolean` | Optional | Flag to indicate whether configuration is active (in effect). | Boolean getIsActive() | setIsActive(Boolean isActive) |
| `LocationId` | `String` | Optional | The location identifier of the resource you want to recieve postbacks from.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `LocationApiId` | `String` | Optional | Location Api ID | String getLocationApiId() | setLocationApiId(String locationApiId) |
| `OnCreate` | `Boolean` | Optional | To receive postbacks on the creation of a resource | Boolean getOnCreate() | setOnCreate(Boolean onCreate) |
| `OnUpdate` | `Boolean` | Optional | To receive postbacks on the updating of a resource | Boolean getOnUpdate() | setOnUpdate(Boolean onUpdate) |
| `OnDelete` | `Boolean` | Optional | To receive postbacks when the record is deleted | Boolean getOnDelete() | setOnDelete(Boolean onDelete) |
| `Legacy` | `Boolean` | Optional | Prefer the legacy api format.<br><br>**Default**: `true` | Boolean getLegacy() | setLegacy(Boolean legacy) |
| `PostbackConfigId` | `String` | Optional | Postback Config ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getPostbackConfigId() | setPostbackConfigId(String postbackConfigId) |
| `ProductTransactionId` | `String` | Optional | Required when using 'transaction' or 'transactionbatch' resource<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getProductTransactionId() | setProductTransactionId(String productTransactionId) |
| `Resource` | [`Resource12Enum`](../../doc/models/resource-12-enum.md) | Optional | The resource you want to subscribe the postbacks to.<br><br>> Possible values include: 'contact', 'transaction', 'transactionbatch'<br><br>**Constraints**: *Maximum Length*: `128` | Resource12Enum getResource() | setResource(Resource12Enum resource) |
| `NumberOfAttempts` | `Integer` | Optional | Maximum number of attempts on failure<br><br>**Constraints**: `>= 1`, `<= 5` | Integer getNumberOfAttempts() | setNumberOfAttempts(Integer numberOfAttempts) |
| `Url` | `String` | Optional | The URL where the postback will be submitted<br><br>**Constraints**: *Maximum Length*: `512` | String getUrl() | setUrl(String url) |
| `Id` | `String` | Optional | Postback Config ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `PostbackLogs` | [`List<PostbackLog>`](../../doc/models/postback-log.md) | Optional | Postback Log Information on `expand` | List<PostbackLog> getPostbackLogs() | setPostbackLogs(List<PostbackLog> postbackLogs) |

## Example (as JSON)

```json
{
  "attempt_interval": 300,
  "basic_auth_username": "username",
  "basic_auth_password": "password",
  "expands": "changelogs,tags",
  "format": "api-default",
  "is_active": true,
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "on_create": true,
  "on_update": true,
  "on_delete": true,
  "legacy": true,
  "postback_config_id": "11e95f8ec39de8fbdb0a4f1a",
  "product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "resource": "contact",
  "number_of_attempts": 1,
  "url": "https://127.0.0.1/receiver",
  "id": "11e95f8ec39de8fbdb0a4f1a"
}
```

