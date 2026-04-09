
# Message Extension

## Structure

`MessageExtension`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `String` | Optional | A unique identifier for the extension. Payment System Registered Application Provider Identifier (RID) is required as prefix of the ID. The maximum length is 64 characters.<br><br>**Constraints**: *Maximum Length*: `64` | String getId() | setId(String id) |
| `Name` | `String` | Optional | The name of the extension data set as defined by the extension owner. Maximum length is 64 characters.<br><br>**Constraints**: *Maximum Length*: `64` | String getName() | setName(String name) |
| `CriticalityIndicator` | `Boolean` | Optional | A boolean value indicating whether the recipient must understand the contents of the extension to interpret the entire message. | Boolean getCriticalityIndicator() | setCriticalityIndicator(Boolean criticalityIndicator) |
| `Data` | `Object` | Optional | The data carried in the extension as. The maximum length is 8059 characters. | Object getData() | setData(Object data) |

## Example (as JSON)

```json
{
  "id": "id0",
  "name": "name0",
  "criticality_indicator": false,
  "data": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

