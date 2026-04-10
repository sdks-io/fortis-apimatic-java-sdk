
# Response Terminals Collection

*This model accepts additional fields of type Object.*

## Structure

`ResponseTerminalsCollection`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type83`](../../doc/models/type-83.md) | Optional | - | Type83 getType() | setType(Type83 type) |
| `List` | [`List<List14>`](../../doc/models/list-14.md) | Optional | Resource Members | List<List14> getList() | setList(List<List14> list) |
| `Links` | [`Links1`](../../doc/models/links-1.md) | Optional | - | Links1 getLinks() | setLinks(Links1 links) |
| `Pagination` | [`Pagination1`](../../doc/models/pagination-1.md) | Optional | - | Pagination1 getPagination() | setPagination(Pagination1 pagination) |
| `Sort` | [`Sort1`](../../doc/models/sort-1.md) | Optional | - | Sort1 getSort() | setSort(Sort1 sort) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "TerminalsCollection",
  "list": [
    {
      "location_id": "location_id6",
      "default_product_transaction_id": "default_product_transaction_id8",
      "terminal_application_id": "terminal_application_id2",
      "terminal_cvm_id": "terminal_cvm_id8",
      "terminal_manufacturer_code": "4",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "location_id": "location_id6",
      "default_product_transaction_id": "default_product_transaction_id8",
      "terminal_application_id": "terminal_application_id2",
      "terminal_cvm_id": "terminal_cvm_id8",
      "terminal_manufacturer_code": "4",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "location_id": "location_id6",
      "default_product_transaction_id": "default_product_transaction_id8",
      "terminal_application_id": "terminal_application_id2",
      "terminal_cvm_id": "terminal_cvm_id8",
      "terminal_manufacturer_code": "4",
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

