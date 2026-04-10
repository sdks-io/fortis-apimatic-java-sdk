
# Response Transaction Processing

*This model accepts additional fields of type Object.*

## Structure

`ResponseTransactionProcessing`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type5`](../../doc/models/type-5.md) | Optional | - | Type5 getType() | setType(Type5 type) |
| `Data` | [`Data1`](../../doc/models/data-1.md) | Optional | - | Data1 getData() | setData(Data1 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "TransactionProcessing",
  "data": {
    "async": {
      "code": "00000038-0000-0000-0000-000000000000",
      "link": "link8",
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

