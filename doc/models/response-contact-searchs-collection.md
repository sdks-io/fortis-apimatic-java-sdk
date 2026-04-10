
# Response Contact Searchs Collection

*This model accepts additional fields of type Object.*

## Structure

`ResponseContactSearchsCollection`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type6`](../../doc/models/type-6.md) | Optional | - | Type6 getType() | setType(Type6 type) |
| `List` | [`List<List1>`](../../doc/models/list-1.md) | Optional | Resource Members | List<List1> getList() | setList(List<List1> list) |
| `Links` | [`Links1`](../../doc/models/links-1.md) | Optional | - | Links1 getLinks() | setLinks(Links1 links) |
| `Pagination` | [`Pagination1`](../../doc/models/pagination-1.md) | Optional | - | Pagination1 getPagination() | setPagination(Pagination1 pagination) |
| `Sort` | [`Sort1`](../../doc/models/sort-1.md) | Optional | - | Sort1 getSort() | setSort(Sort1 sort) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

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
      "last_name": "last_name0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "location_id": "location_id6",
      "account_number": "account_number2",
      "contact_api_id": "contact_api_id2",
      "first_name": "first_name2",
      "last_name": "last_name0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "location_id": "location_id6",
      "account_number": "account_number2",
      "contact_api_id": "contact_api_id2",
      "first_name": "first_name2",
      "last_name": "last_name0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "links": {
    "type": "Links",
    "first": "first0",
    "previous": "previous2",
    "next": "next2",
    "last": "last4",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "pagination": {
    "type": "Pagination",
    "total_count": 100,
    "page_count": 212,
    "page_number": 28,
    "page_size": 6,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "sort": {
    "type": "Sorting",
    "fields": [
      {
        "field": "field2",
        "order": "asc",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      {
        "field": "field2",
        "order": "asc",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      {
        "field": "field2",
        "order": "asc",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      }
    ],
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

