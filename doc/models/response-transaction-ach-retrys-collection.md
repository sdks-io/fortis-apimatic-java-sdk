
# Response Transaction Ach Retrys Collection

*This model accepts additional fields of type Object.*

## Structure

`ResponseTransactionAchRetrysCollection`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type103`](../../doc/models/type-103.md) | Optional | - | Type103 getType() | setType(Type103 type) |
| `List` | [`List<List17>`](../../doc/models/list-17.md) | Optional | Resource Members | List<List17> getList() | setList(List<List17> list) |
| `Links` | [`Links1`](../../doc/models/links-1.md) | Optional | - | Links1 getLinks() | setLinks(Links1 links) |
| `Pagination` | [`Pagination1`](../../doc/models/pagination-1.md) | Optional | - | Pagination1 getPagination() | setPagination(Pagination1 pagination) |
| `Sort` | [`Sort1`](../../doc/models/sort-1.md) | Optional | - | Sort1 getSort() | setSort(Sort1 sort) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "TransactionAchRetrysCollection",
  "list": [
    {
      "rejected_transaction_id": "rejected_transaction_id6",
      "return_fee": 150,
      "id": "id2",
      "retry_transaction_id": "retry_transaction_id8",
      "return_fee_transaction_id": "return_fee_transaction_id6",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "rejected_transaction_id": "rejected_transaction_id6",
      "return_fee": 150,
      "id": "id2",
      "retry_transaction_id": "retry_transaction_id8",
      "return_fee_transaction_id": "return_fee_transaction_id6",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "rejected_transaction_id": "rejected_transaction_id6",
      "return_fee": 150,
      "id": "id2",
      "retry_transaction_id": "retry_transaction_id8",
      "return_fee_transaction_id": "return_fee_transaction_id6",
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

