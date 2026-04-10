
# Response Tickets Collection

*This model accepts additional fields of type Object.*

## Structure

`ResponseTicketsCollection`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type88`](../../doc/models/type-88.md) | Optional | - | Type88 getType() | setType(Type88 type) |
| `List` | [`List<List15>`](../../doc/models/list-15.md) | Optional | Resource Members | List<List15> getList() | setList(List<List15> list) |
| `Links` | [`Links1`](../../doc/models/links-1.md) | Optional | - | Links1 getLinks() | setLinks(Links1 links) |
| `Pagination` | [`Pagination1`](../../doc/models/pagination-1.md) | Optional | - | Pagination1 getPagination() | setPagination(Pagination1 pagination) |
| `Sort` | [`Sort1`](../../doc/models/sort-1.md) | Optional | - | Sort1 getSort() | setSort(Sort1 sort) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "TicketsCollection",
  "list": [
    {
      "account_holder_name": "account_holder_name8",
      "exp_date": "exp_date0",
      "cvv": "cvv0",
      "account_number": "account_number2",
      "billing_address": {
        "postal_code": "postal_code0",
        "street": "street8",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "account_holder_name": "account_holder_name8",
      "exp_date": "exp_date0",
      "cvv": "cvv0",
      "account_number": "account_number2",
      "billing_address": {
        "postal_code": "postal_code0",
        "street": "street8",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "account_holder_name": "account_holder_name8",
      "exp_date": "exp_date0",
      "cvv": "cvv0",
      "account_number": "account_number2",
      "billing_address": {
        "postal_code": "postal_code0",
        "street": "street8",
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

