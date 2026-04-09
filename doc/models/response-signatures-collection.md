
# Response Signatures Collection

## Structure

`ResponseSignaturesCollection`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type73Enum`](../../doc/models/type-73-enum.md) | Optional | Resource Type<br><br>**Default**: `Type73Enum.SIGNATURESCOLLECTION` | Type73Enum getType() | setType(Type73Enum type) |
| `List` | [`List<List12>`](../../doc/models/list-12.md) | Optional | Resource Members | List<List12> getList() | setList(List<List12> list) |
| `Links` | [`Links`](../../doc/models/links.md) | Optional | Pagination page links | Links getLinks() | setLinks(Links links) |
| `Pagination` | [`Pagination`](../../doc/models/pagination.md) | Optional | Pagination info | Pagination getPagination() | setPagination(Pagination pagination) |
| `Sort` | [`Sort`](../../doc/models/sort.md) | Optional | Sort information used on the results | Sort getSort() | setSort(Sort sort) |

## Example (as JSON)

```json
{
  "type": "SignaturesCollection",
  "list": [
    {
      "signature": "signature0",
      "resource": "Recurring",
      "resource_id": "resource_id8",
      "id": "id2",
      "created_ts": 56
    },
    {
      "signature": "signature0",
      "resource": "Recurring",
      "resource_id": "resource_id8",
      "id": "id2",
      "created_ts": 56
    }
  ],
  "links": {
    "type": "Links",
    "first": "first0",
    "previous": "previous2",
    "next": "next2",
    "last": "last4"
  },
  "pagination": {
    "type": "Pagination",
    "total_count": 100,
    "page_count": 212,
    "page_number": 28,
    "page_size": 6
  },
  "sort": {
    "type": "Sorting",
    "fields": [
      {
        "field": "field2",
        "order": "asc"
      },
      {
        "field": "field2",
        "order": "asc"
      },
      {
        "field": "field2",
        "order": "asc"
      }
    ]
  }
}
```

