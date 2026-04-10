
# Pagination 1

*This model accepts additional fields of type Object.*

## Structure

`Pagination1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type3`](../../doc/models/type-3.md) | Optional | - | Type3 getType() | setType(Type3 type) |
| `TotalCount` | `Integer` | Optional | Total records count | Integer getTotalCount() | setTotalCount(Integer totalCount) |
| `PageCount` | `Integer` | Optional | Total page count | Integer getPageCount() | setPageCount(Integer pageCount) |
| `PageNumber` | `Integer` | Optional | Current page | Integer getPageNumber() | setPageNumber(Integer pageNumber) |
| `PageSize` | `Integer` | Optional | Page size | Integer getPageSize() | setPageSize(Integer pageSize) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "total_count": 423,
  "page_count": 42,
  "page_number": 6,
  "page_size": 10,
  "type": "Pagination",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

