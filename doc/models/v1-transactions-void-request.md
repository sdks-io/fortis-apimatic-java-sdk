
# V1 Transactions Void Request

*This model accepts additional fields of type Object.*

## Structure

`V1TransactionsVoidRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Tags` | `List<String>` | Optional | Tags | List<String> getTags() | setTags(List<String> tags) |
| `Description` | `String` | Optional | Description<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `64` | String getDescription() | setDescription(String description) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "description": "some description",
  "tags": [
    "tags5",
    "tags6",
    "tags7"
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

