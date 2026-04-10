
# Data 33

*This model accepts additional fields of type Object.*

## Structure

`Data33`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `UserApiKey` | `String` | Optional | User Api Key<br><br>**Constraints**: *Minimum Length*: `16`, *Maximum Length*: `64` | String getUserApiKey() | setUserApiKey(String userApiKey) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "user_api_key": "234bas8dfn8238f923w2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

