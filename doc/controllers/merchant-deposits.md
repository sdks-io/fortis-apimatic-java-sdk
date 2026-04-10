# Merchant Deposits

```java
MerchantDepositsController merchantDepositsController = client.getMerchantDepositsController();
```

## Class Name

`MerchantDepositsController`

## Methods

* [View Single Merchant Deposit](../../doc/controllers/merchant-deposits.md#view-single-merchant-deposit)
* [Listall Merchant Deposits](../../doc/controllers/merchant-deposits.md#listall-merchant-deposits)


# View Single Merchant Deposit

```java
CompletableFuture<ApiResponse<ResponseMerchantDeposit>> viewSingleMerchantDepositAsync(
    final String depositId,
    final Page1 page,
    final List<Order21> order,
    final List<FilterBy> filterBy,
    final List<Expand15> expand,
    final Format1 format,
    final String typeahead,
    final List<Field37> fields,
    final ViewSingleMerchantDepositKeyword keyword)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `depositId` | `String` | Template, Required | Deposit Id |
| `page` | [`Page1`](../../doc/models/page-1.md) | Query, Optional | Use this field to specify paginate your results, by using page size and number. You can use one of the following methods:<br><br>> /endpoint?page={ "number": 1, "size": 50 }<br>> <br>> /endpoint?page[number]=1&page[size]=50 |
| `order` | [`List<Order21>`](../../doc/models/order-21.md) | Query, Optional | Criteria used in query string parameters to order results.  Most fields from the endpoint results can be used as a `key`.  Unsupported fields or operators will return a `412`.  Must be encoded, or use syntax that does not require encoding.<br><br>> /endpoint?order[0][key]=created_ts&order[0][operator]=asc<br>> <br>> /endpoint?order=[{ "key": "created_ts", "operator": "asc"}]<br>> <br>> /endpoint?order=[{ "key": "balance", "operator": "desc"},{ "key": "created_ts", "operator": "asc"}]<br><br>**Constraints**: *Minimum Items*: `1` |
| `filterBy` | [`List<FilterBy>`](../../doc/models/filter-by.md) | Query, Optional | Filter criteria that can be used in query string parameters.  Most fields from the endpoint results can be used as a `key`.  Unsupported fields or operators will return a `412`. Must be encoded, or use syntax that does not require encoding.<br><br>> ?filter_by[0][key]=first_name&filter_by[0][operator]==&filter_by[0][value]=Steve<br>> <br>> /endpoint?filter_by=[{ "key": "first_name", "operator": "=", "value": "Fred" }]<br>> <br>> /endpoint?filter_by=[{ "key": "account_type", "operator": "=", "value": "VISA" }]<br>> <br>> /endpoint?filter_by=[{ "key": "created_ts", "operator": ">=", "value": "946702799" }, { "key": "created_ts", "operator": "<=", value: "1695061891" }]<br>> <br>> /endpoint?filter_by=[{ "key": "last_name", "operator": "IN", "value": "Williams,Brown,Allman" }]<br><br>**Constraints**: *Minimum Items*: `1` |
| `expand` | [`List<Expand15>`](../../doc/models/expand-15.md) | Query, Optional | Most endpoints in the API have a way to retrieve extra data related to the current record being retrieved. For example, if the API request is for the accountvaults endpoint, and the end user also needs to know which contact the token belongs to, this data can be returned in the accountvaults endpoint request.<br><br>**Constraints**: *Unique Items Required* |
| `format` | [`Format1`](../../doc/models/format-1.md) | Query, Optional | Reporting format, valid values: csv, tsv |
| `typeahead` | `String` | Query, Optional | You can use any `field_name` from this endpoint results to order the list using the value provided as filter for the same `field_name`. It will be ordered using the following rules: 1) Exact match, 2) Starts with, 3) Contains.<br><br>> /endpoint?filter={ "field_name": "Value" }&_typeahead=field_name |
| `fields` | [`List<Field37>`](../../doc/models/field-37.md) | Query, Optional | You can use any `field_name` from this endpoint results to filter the list of fields returned on the response. |
| `keyword` | [`ViewSingleMerchantDepositKeyword`](../../doc/models/containers/view-single-merchant-deposit-keyword.md) | Query, Optional | This is a container for any-of cases. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`ResponseMerchantDeposit`](../../doc/models/response-merchant-deposit.md).

## Example Usage

```java
String depositId = "deposit_id0";
Page1 page = new Page1.Builder()
    .number(1)
    .size(50)
    .build();

List<Order21> order = Arrays.asList(
    new Order21.Builder(
        "first_name",
        Operator.ASC
    )
    .build()
);

List<FilterBy> filterBy = Arrays.asList(
    new FilterBy.Builder(
        "first_name",
        FilterByOperator.fromOperator1(
            Operator1.ENUM_1
        ),
        FilterByValue.fromFilterByValueCase1(
            FilterByValueCase1.fromString(
                "Fred"
            )
        )
    )
    .build()
);


merchantDepositsController.viewSingleMerchantDepositAsync(depositId, page, order, filterBy, null, null, null, null, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof Response401TokenException) {
        Response401TokenException response401TokenException = (Response401TokenException) cause;
        response401TokenException.printStackTrace();
    } else {
        // fallback for unexpected errors
        exception.printStackTrace();
    }

    return null;
});
```

## Example Response *(as JSON)*

```json
{
  "type": "MerchantDeposit",
  "data": {
    "company_id": "8410111",
    "merchant_id": "88441",
    "deposit_types": [
      "deposit"
    ],
    "deposit_amount": 2487.24,
    "batch_amount": 2487.24,
    "adjustment_amount": 2487.24,
    "retained_amount": 2487.24,
    "conveyed_amount": 2487.24,
    "fee_amount": 2487.24,
    "reference_number": "400000",
    "trace_number": "400000",
    "currency": "USD",
    "created_ts": 1422040992,
    "reported_date": "2021-12-01",
    "transaction_date": "2021-12-01",
    "details": [
      {
        "amount": 2487.24,
        "reported_date": "2021-12-01",
        "settled_date": "2021-12-01"
      }
    ]
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401TokenException`](../../doc/models/response-401-token-exception.md) |


# Listall Merchant Deposits

```java
CompletableFuture<ApiResponse<ResponseMerchantDepositsCollection>> listallMerchantDepositsAsync(
    final Page1 page,
    final List<Order21> order,
    final List<FilterBy> filterBy,
    final List<Expand15> expand,
    final Format1 format,
    final String typeahead,
    final List<Field38> fields,
    final ListallMerchantDepositsKeyword keyword)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `page` | [`Page1`](../../doc/models/page-1.md) | Query, Optional | Use this field to specify paginate your results, by using page size and number. You can use one of the following methods:<br><br>> /endpoint?page={ "number": 1, "size": 50 }<br>> <br>> /endpoint?page[number]=1&page[size]=50 |
| `order` | [`List<Order21>`](../../doc/models/order-21.md) | Query, Optional | Criteria used in query string parameters to order results.  Most fields from the endpoint results can be used as a `key`.  Unsupported fields or operators will return a `412`.  Must be encoded, or use syntax that does not require encoding.<br><br>> /endpoint?order[0][key]=created_ts&order[0][operator]=asc<br>> <br>> /endpoint?order=[{ "key": "created_ts", "operator": "asc"}]<br>> <br>> /endpoint?order=[{ "key": "balance", "operator": "desc"},{ "key": "created_ts", "operator": "asc"}]<br><br>**Constraints**: *Minimum Items*: `1` |
| `filterBy` | [`List<FilterBy>`](../../doc/models/filter-by.md) | Query, Optional | Filter criteria that can be used in query string parameters.  Most fields from the endpoint results can be used as a `key`.  Unsupported fields or operators will return a `412`. Must be encoded, or use syntax that does not require encoding.<br><br>> ?filter_by[0][key]=first_name&filter_by[0][operator]==&filter_by[0][value]=Steve<br>> <br>> /endpoint?filter_by=[{ "key": "first_name", "operator": "=", "value": "Fred" }]<br>> <br>> /endpoint?filter_by=[{ "key": "account_type", "operator": "=", "value": "VISA" }]<br>> <br>> /endpoint?filter_by=[{ "key": "created_ts", "operator": ">=", "value": "946702799" }, { "key": "created_ts", "operator": "<=", value: "1695061891" }]<br>> <br>> /endpoint?filter_by=[{ "key": "last_name", "operator": "IN", "value": "Williams,Brown,Allman" }]<br><br>**Constraints**: *Minimum Items*: `1` |
| `expand` | [`List<Expand15>`](../../doc/models/expand-15.md) | Query, Optional | Most endpoints in the API have a way to retrieve extra data related to the current record being retrieved. For example, if the API request is for the accountvaults endpoint, and the end user also needs to know which contact the token belongs to, this data can be returned in the accountvaults endpoint request.<br><br>**Constraints**: *Unique Items Required* |
| `format` | [`Format1`](../../doc/models/format-1.md) | Query, Optional | Reporting format, valid values: csv, tsv |
| `typeahead` | `String` | Query, Optional | You can use any `field_name` from this endpoint results to order the list using the value provided as filter for the same `field_name`. It will be ordered using the following rules: 1) Exact match, 2) Starts with, 3) Contains.<br><br>> /endpoint?filter={ "field_name": "Value" }&_typeahead=field_name |
| `fields` | [`List<Field38>`](../../doc/models/field-38.md) | Query, Optional | You can use any `field_name` from this endpoint results to filter the list of fields returned on the response. |
| `keyword` | [`ListallMerchantDepositsKeyword`](../../doc/models/containers/listall-merchant-deposits-keyword.md) | Query, Optional | This is a container for any-of cases. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`ResponseMerchantDepositsCollection`](../../doc/models/response-merchant-deposits-collection.md).

## Example Usage

```java
Page1 page = new Page1.Builder()
    .number(1)
    .size(50)
    .build();

List<Order21> order = Arrays.asList(
    new Order21.Builder(
        "first_name",
        Operator.ASC
    )
    .build()
);

List<FilterBy> filterBy = Arrays.asList(
    new FilterBy.Builder(
        "first_name",
        FilterByOperator.fromOperator1(
            Operator1.ENUM_1
        ),
        FilterByValue.fromFilterByValueCase1(
            FilterByValueCase1.fromString(
                "Fred"
            )
        )
    )
    .build()
);


merchantDepositsController.listallMerchantDepositsAsync(page, order, filterBy, null, null, null, null, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof Response401TokenException) {
        Response401TokenException response401TokenException = (Response401TokenException) cause;
        response401TokenException.printStackTrace();
    } else {
        // fallback for unexpected errors
        exception.printStackTrace();
    }

    return null;
});
```

## Example Response *(as JSON)*

```json
{
  "type": "MerchantDepositsCollection",
  "list": [
    {
      "company_id": "8410111",
      "merchant_id": "88441",
      "deposit_types": [
        "deposit"
      ],
      "deposit_amount": 2487.24,
      "batch_amount": 2487.24,
      "adjustment_amount": 2487.24,
      "retained_amount": 2487.24,
      "conveyed_amount": 2487.24,
      "fee_amount": 2487.24,
      "reference_number": "400000",
      "trace_number": "400000",
      "currency": "USD",
      "created_ts": 1422040992,
      "reported_date": "2021-12-01",
      "transaction_date": "2021-12-01",
      "details": [
        {
          "amount": 2487.24,
          "reported_date": "2021-12-01",
          "settled_date": "2021-12-01"
        }
      ]
    }
  ],
  "links": {
    "type": "Links",
    "first": "/v1/endpoint?page[size]=10&page[number]=1",
    "previous": "/v1/endpoint?page[size]=10&page[number]=5",
    "next": "/v1/endpoint?page[size]=10&page[number]=7",
    "last": "/v1/endpoint?page[size]=10&page[number]=42"
  },
  "pagination": {
    "type": "Pagination",
    "total_count": 423,
    "page_count": 42,
    "page_number": 6,
    "page_size": 10
  },
  "sort": {
    "type": "Sorting",
    "fields": [
      {
        "field": "last_name",
        "order": "asc"
      }
    ]
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401TokenException`](../../doc/models/response-401-token-exception.md) |

