
# Response Recurrings Collection

*This model accepts additional fields of type Object.*

## Structure

`ResponseRecurringsCollection`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type68`](../../doc/models/type-68.md) | Optional | - | Type68 getType() | setType(Type68 type) |
| `List` | [`List<List11>`](../../doc/models/list-11.md) | Optional | Resource Members | List<List11> getList() | setList(List<List11> list) |
| `Links` | [`Links1`](../../doc/models/links-1.md) | Optional | - | Links1 getLinks() | setLinks(Links1 links) |
| `Pagination` | [`Pagination1`](../../doc/models/pagination-1.md) | Optional | - | Pagination1 getPagination() | setPagination(Pagination1 pagination) |
| `Sort` | [`Sort1`](../../doc/models/sort-1.md) | Optional | - | Sort1 getSort() | setSort(Sort1 sort) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "RecurringsCollection",
  "list": [
    {
      "account_vault_id": "account_vault_id8",
      "token_id": "token_id6",
      "contact_id": "contact_id2",
      "account_vault_api_id": "account_vault_api_id6",
      "token_api_id": "token_api_id2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "account_vault_id": "account_vault_id8",
      "token_id": "token_id6",
      "contact_id": "contact_id2",
      "account_vault_api_id": "account_vault_api_id6",
      "token_api_id": "token_api_id2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "account_vault_id": "account_vault_id8",
      "token_id": "token_id6",
      "contact_id": "contact_id2",
      "account_vault_api_id": "account_vault_api_id6",
      "token_api_id": "token_api_id2",
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

