
# Response Transactions Collection

*This model accepts additional fields of type Object.*

## Structure

`ResponseTransactionsCollection`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type117`](../../doc/models/type-117.md) | Optional | - | Type117 getType() | setType(Type117 type) |
| `List` | [`List<List18>`](../../doc/models/list-18.md) | Optional | Resource Members | List<List18> getList() | setList(List<List18> list) |
| `Links` | [`Links1`](../../doc/models/links-1.md) | Optional | - | Links1 getLinks() | setLinks(Links1 links) |
| `Pagination` | [`Pagination1`](../../doc/models/pagination-1.md) | Optional | - | Pagination1 getPagination() | setPagination(Pagination1 pagination) |
| `Sort` | [`Sort1`](../../doc/models/sort-1.md) | Optional | - | Sort1 getSort() | setSort(Sort1 sort) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "TransactionsCollection",
  "list": [
    {
      "additional_amounts": [
        {
          "type": {
            "key1": "val1",
            "key2": "val2"
          },
          "amount": 6,
          "account_type": {
            "key1": "val1",
            "key2": "val2"
          },
          "currency": 154.64,
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        }
      ],
      "billing_address": {
        "city": "city2",
        "state": "state6",
        "postal_code": "postal_code0",
        "street": "street8",
        "phone": "phone2",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "checkin_date": "checkin_date4",
      "checkout_date": "checkout_date6",
      "clerk_number": "clerk_number6",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "additional_amounts": [
        {
          "type": {
            "key1": "val1",
            "key2": "val2"
          },
          "amount": 6,
          "account_type": {
            "key1": "val1",
            "key2": "val2"
          },
          "currency": 154.64,
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        }
      ],
      "billing_address": {
        "city": "city2",
        "state": "state6",
        "postal_code": "postal_code0",
        "street": "street8",
        "phone": "phone2",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "checkin_date": "checkin_date4",
      "checkout_date": "checkout_date6",
      "clerk_number": "clerk_number6",
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

