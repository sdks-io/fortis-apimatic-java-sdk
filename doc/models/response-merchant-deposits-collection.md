
# Response Merchant Deposits Collection

## Structure

`ResponseMerchantDepositsCollection`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type48Enum`](../../doc/models/type-48-enum.md) | Optional | Resource Type<br><br>**Default**: `Type48Enum.MERCHANTDEPOSITSCOLLECTION` | Type48Enum getType() | setType(Type48Enum type) |
| `List` | [`List<List8>`](../../doc/models/list-8.md) | Optional | Resource Members | List<List8> getList() | setList(List<List8> list) |
| `Links` | [`Links`](../../doc/models/links.md) | Optional | Pagination page links | Links getLinks() | setLinks(Links links) |
| `Pagination` | [`Pagination`](../../doc/models/pagination.md) | Optional | Pagination info | Pagination getPagination() | setPagination(Pagination pagination) |
| `Sort` | [`Sort`](../../doc/models/sort.md) | Optional | Sort information used on the results | Sort getSort() | setSort(Sort sort) |

## Example (as JSON)

```json
{
  "type": "MerchantDepositsCollection",
  "list": [
    {
      "id": "id2",
      "company_id": "company_id8",
      "merchant_id": "merchant_id2",
      "service": "service8",
      "deposit_types": [
        "fee",
        "deposit"
      ]
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

