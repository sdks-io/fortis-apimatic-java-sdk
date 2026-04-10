
# Data 1

*This model accepts additional fields of type Object.*

## Structure

`Data1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Async` | [`Async2`](../../doc/models/async-2.md) | Optional | - | Async2 getAsync() | setAsync(Async2 async) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
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
}
```

