
# Response User Api Key

*This model accepts additional fields of type Object.*

## Structure

`ResponseUserApiKey`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type128`](../../doc/models/type-128.md) | Optional | - | Type128 getType() | setType(Type128 type) |
| `Data` | [`Data33`](../../doc/models/data-33.md) | Optional | - | Data33 getData() | setData(Data33 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "UserApiKey",
  "data": {
    "user_api_key": "user_api_key2",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

