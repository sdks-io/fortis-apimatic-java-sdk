
# Links

Pagination page links

*This model accepts additional fields of type Object.*

## Structure

`Links`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type2`](../../doc/models/type-2.md) | Optional | - | Type2 getType() | setType(Type2 type) |
| `First` | `String` | Optional | Link to the first page | String getFirst() | setFirst(String first) |
| `Previous` | `String` | Optional | Link to the previous page | String getPrevious() | setPrevious(String previous) |
| `Next` | `String` | Optional | Link to the next page | String getNext() | setNext(String next) |
| `Last` | `String` | Optional | Link to the last page | String getLast() | setLast(String last) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "first": "/v1/endpoint?page[size]=10&page[number]=1",
  "previous": "/v1/endpoint?page[size]=10&page[number]=5",
  "next": "/v1/endpoint?page[size]=10&page[number]=7",
  "last": "/v1/endpoint?page[size]=10&page[number]=42",
  "type": "Links",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

