
# Response Location

*This model accepts additional fields of type Object.*

## Structure

`ResponseLocation`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type43`](../../doc/models/type-43.md) | Optional | - | Type43 getType() | setType(Type43 type) |
| `Data` | [`Data10`](../../doc/models/data-10.md) | Optional | - | Data10 getData() | setData(Data10 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "Location",
  "data": {
    "id": "id0",
    "created_ts": 114,
    "modified_ts": 190,
    "account_number": "account_number0",
    "address": {
      "city": "city6",
      "state": "state2",
      "postal_code": "postal_code8",
      "country": {
        "key1": "val1",
        "key2": "val2"
      },
      "street": "street6",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
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

