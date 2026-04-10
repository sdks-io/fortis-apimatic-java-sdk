
# Response Users Collection

*This model accepts additional fields of type Object.*

## Structure

`ResponseUsersCollection`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type130`](../../doc/models/type-130.md) | Optional | - | Type130 getType() | setType(Type130 type) |
| `List` | [`List<List20>`](../../doc/models/list-20.md) | Optional | Resource Members | List<List20> getList() | setList(List<List20> list) |
| `Links` | [`Links1`](../../doc/models/links-1.md) | Optional | - | Links1 getLinks() | setLinks(Links1 links) |
| `Pagination` | [`Pagination1`](../../doc/models/pagination-1.md) | Optional | - | Pagination1 getPagination() | setPagination(Pagination1 pagination) |
| `Sort` | [`Sort1`](../../doc/models/sort-1.md) | Optional | - | Sort1 getSort() | setSort(Sort1 sort) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "UsersCollection",
  "list": [
    {
      "account_number": "account_number2",
      "branding_domain_url": "branding_domain_url8",
      "cell_phone": "cell_phone8",
      "company_name": "company_name8",
      "contact_id": "contact_id2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "account_number": "account_number2",
      "branding_domain_url": "branding_domain_url8",
      "cell_phone": "cell_phone8",
      "company_name": "company_name8",
      "contact_id": "contact_id2",
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

