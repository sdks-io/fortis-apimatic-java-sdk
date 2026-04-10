
# Response Token

*This model accepts additional fields of type Object.*

## Structure

`ResponseToken`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type92`](../../doc/models/type-92.md) | Optional | - | Type92 getType() | setType(Type92 type) |
| `Data` | [`Data25`](../../doc/models/data-25.md) | Optional | - | Data25 getData() | setData(Data25 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "Token",
  "data": {
    "account_holder_name": "account_holder_name0",
    "account_vault_api_id": "account_vault_api_id4",
    "token_api_id": "token_api_id6",
    "accountvault_c1": "accountvault_c14",
    "accountvault_c2": "accountvault_c28",
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

