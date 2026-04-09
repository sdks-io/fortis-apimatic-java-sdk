
# Response Contact Searchs Collection

## Structure

`ResponseContactSearchsCollection`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type6Enum`](../../doc/models/type-6-enum.md) | Optional | Resource Type<br><br>**Default**: `Type6Enum.CONTACTSEARCHSCOLLECTION` | Type6Enum getType() | setType(Type6Enum type) |
| `List` | [`List<List1>`](../../doc/models/list-1.md) | Optional | Resource Members | List<List1> getList() | setList(List<List1> list) |
| `Links` | [`Links`](../../doc/models/links.md) | Optional | Pagination page links | Links getLinks() | setLinks(Links links) |
| `Pagination` | [`Pagination`](../../doc/models/pagination.md) | Optional | Pagination info | Pagination getPagination() | setPagination(Pagination pagination) |
| `Sort` | [`Sort`](../../doc/models/sort.md) | Optional | Sort information used on the results | Sort getSort() | setSort(Sort sort) |

## Example (as JSON)

```json
{
  "type": "ContactSearchsCollection",
  "list": [
    {
      "location_id": "location_id6",
      "account_number": "account_number2",
      "contact_api_id": "contact_api_id2",
      "first_name": "first_name2",
      "last_name": "last_name0"
    },
    {
      "location_id": "location_id6",
      "account_number": "account_number2",
      "contact_api_id": "contact_api_id2",
      "first_name": "first_name2",
      "last_name": "last_name0"
    },
    {
      "location_id": "location_id6",
      "account_number": "account_number2",
      "contact_api_id": "contact_api_id2",
      "first_name": "first_name2",
      "last_name": "last_name0"
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

