
# Pagination

Pagination info

## Structure

`Pagination`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type3Enum`](../../doc/models/type-3-enum.md) | Optional | Object type | Type3Enum getType() | setType(Type3Enum type) |
| `TotalCount` | `Integer` | Optional | Total records count | Integer getTotalCount() | setTotalCount(Integer totalCount) |
| `PageCount` | `Integer` | Optional | Total page count | Integer getPageCount() | setPageCount(Integer pageCount) |
| `PageNumber` | `Integer` | Optional | Current page | Integer getPageNumber() | setPageNumber(Integer pageNumber) |
| `PageSize` | `Integer` | Optional | Page size | Integer getPageSize() | setPageSize(Integer pageSize) |

## Example (as JSON)

```json
{
  "type": "Pagination",
  "total_count": 423,
  "page_count": 42,
  "page_number": 6,
  "page_size": 10
}
```

