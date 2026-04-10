
# Response Signature

*This model accepts additional fields of type Object.*

## Structure

`ResponseSignature`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type72`](../../doc/models/type-72.md) | Optional | - | Type72 getType() | setType(Type72 type) |
| `Data` | [`Data21`](../../doc/models/data-21.md) | Optional | - | Data21 getData() | setData(Data21 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "Signature",
  "data": {
    "signature": "signature8",
    "resource": "AccountVault",
    "resource_id": "resource_id6",
    "id": "id0",
    "created_ts": 114,
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

