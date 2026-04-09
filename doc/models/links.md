
# Links

Pagination page links

## Structure

`Links`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type2Enum`](../../doc/models/type-2-enum.md) | Optional | Object type | Type2Enum getType() | setType(Type2Enum type) |
| `First` | `String` | Optional | Link to the first page | String getFirst() | setFirst(String first) |
| `Previous` | `String` | Optional | Link to the previous page | String getPrevious() | setPrevious(String previous) |
| `Next` | `String` | Optional | Link to the next page | String getNext() | setNext(String next) |
| `Last` | `String` | Optional | Link to the last page | String getLast() | setLast(String last) |

## Example (as JSON)

```json
{
  "type": "Links",
  "first": "/v1/endpoint?page[size]=10&page[number]=1",
  "previous": "/v1/endpoint?page[size]=10&page[number]=5",
  "next": "/v1/endpoint?page[size]=10&page[number]=7",
  "last": "/v1/endpoint?page[size]=10&page[number]=42"
}
```

