
# Response Three Ds Authentication

*This model accepts additional fields of type Object.*

## Structure

`ResponseThreeDsAuthentication`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type45`](../../doc/models/type-45.md) | Optional | - | Type45 getType() | setType(Type45 type) |
| `Data` | [`Data12`](../../doc/models/data-12.md) | Optional | - | Data12 getData() | setData(Data12 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "ThreeDSAuthentication",
  "data": {
    "three_ds_server_trans_id": "three_ds_server_trans_id0",
    "acs_url": "acs_url2",
    "transaction_status": "D",
    "authentication_value": "authentication_value2",
    "eci": "eci0",
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

