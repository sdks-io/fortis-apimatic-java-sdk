
# V1 Transactions Void Request

## Structure

`V1TransactionsVoidRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Tags` | `List<String>` | Optional | Tags | List<String> getTags() | setTags(List<String> tags) |
| `Description` | `String` | Optional | Description<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `64` | String getDescription() | setDescription(String description) |

## Example (as JSON)

```json
{
  "description": "some description",
  "tags": [
    "tags7"
  ]
}
```

