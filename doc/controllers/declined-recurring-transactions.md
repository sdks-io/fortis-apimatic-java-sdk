# Declined Recurring Transactions

```java
DeclinedRecurringTransactionsController declinedRecurringTransactionsController = client.getDeclinedRecurringTransactionsController();
```

## Class Name

`DeclinedRecurringTransactionsController`

## Methods

* [Get One Declined Recurring Transaction](../../doc/controllers/declined-recurring-transactions.md#get-one-declined-recurring-transaction)
* [List All Declined Recurring Transactions](../../doc/controllers/declined-recurring-transactions.md#list-all-declined-recurring-transactions)
* [Create a Payment](../../doc/controllers/declined-recurring-transactions.md#create-a-payment)
* [Rerun the Transaction](../../doc/controllers/declined-recurring-transactions.md#rerun-the-transaction)
* [Resend the Transaction](../../doc/controllers/declined-recurring-transactions.md#resend-the-transaction)


# Get One Declined Recurring Transaction

```java
CompletableFuture<ResponseDeclinedRecurringTransaction> getOneDeclinedRecurringTransactionAsync(
    final String declinedRecurringTransactionId,
    final List<Expand5Enum> expand)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `declinedRecurringTransactionId` | `String` | Template, Required | Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `expand` | [`List<Expand5Enum>`](../../doc/models/expand-5-enum.md) | Query, Optional | Most endpoints in the API have a way to retrieve extra data related to the current record being retrieved. For example, if the API request is for the accountvaults endpoint, and the end user also needs to know which contact the token belongs to, this data can be returned in the accountvaults endpoint request.<br><br>**Constraints**: *Unique Items Required*, *Pattern*: `^[\w]+$` |

## Response Type

[`ResponseDeclinedRecurringTransaction`](../../doc/models/response-declined-recurring-transaction.md)

## Example Usage

```java
String declinedRecurringTransactionId = "11e95f8ec39de8fbdb0a4f1a";
declinedRecurringTransactionsController.getOneDeclinedRecurringTransactionAsync(declinedRecurringTransactionId, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof Response401tokenException) {
        Response401tokenException response401tokenException = (Response401tokenException) cause;
        response401tokenException.printStackTrace();
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
  "type": "DeclinedRecurringTransaction",
  "data": {
    "id": "11e95f8ec39de8fbdb0a4f1a",
    "status": "paid",
    "recurring_id": "11e95f8ec39de8fbdb0a4f1a",
    "created_ts": 1422040992,
    "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
    "modified_ts": 1422040992,
    "modified_user_id": "11e95f8ec39de8fbdb0a4f1a"
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401tokenException`](../../doc/models/response-401-token-exception.md) |


# List All Declined Recurring Transactions

```java
CompletableFuture<ResponseDeclinedRecurringTransactionsCollection> listAllDeclinedRecurringTransactionsAsync(
    final Page page,
    final List<Order21> order,
    final List<FilterBy> filterBy,
    final List<Expand5Enum> expand,
    final Format1Enum format,
    final String typeahead,
    final List<Field30Enum> fields)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `page` | [`Page`](../../doc/models/page.md) | Query, Optional | Use this field to specify paginate your results, by using page size and number. You can use one of the following methods:<br><br>> /endpoint?page={ "number": 1, "size": 50 }<br>> <br>> /endpoint?page[number]=1&page[size]=50 |
| `order` | [`List<Order21>`](../../doc/models/order-21.md) | Query, Optional | Criteria used in query string parameters to order results.  Most fields from the endpoint results can be used as a `key`.  Unsupported fields or operators will return a `412`.  Must be encoded, or use syntax that does not require encoding.<br><br>> /endpoint?order[0][key]=created_ts&order[0][operator]=asc<br>> <br>> /endpoint?order=[{ "key": "created_ts", "operator": "asc"}]<br>> <br>> /endpoint?order=[{ "key": "balance", "operator": "desc"},{ "key": "created_ts", "operator": "asc"}]<br><br>**Constraints**: *Minimum Items*: `1` |
| `filterBy` | [`List<FilterBy>`](../../doc/models/filter-by.md) | Query, Optional | Filter criteria that can be used in query string parameters.  Most fields from the endpoint results can be used as a `key`.  Unsupported fields or operators will return a `412`. Must be encoded, or use syntax that does not require encoding.<br><br>> ?filter_by[0][key]=first_name&filter_by[0][operator]==&filter_by[0][value]=Steve<br>> <br>> /endpoint?filter_by=[{ "key": "first_name", "operator": "=", "value": "Fred" }]<br>> <br>> /endpoint?filter_by=[{ "key": "account_type", "operator": "=", "value": "VISA" }]<br>> <br>> /endpoint?filter_by=[{ "key": "created_ts", "operator": ">=", "value": "946702799" }, { "key": "created_ts", "operator": "<=", value: "1695061891" }]<br>> <br>> /endpoint?filter_by=[{ "key": "last_name", "operator": "IN", "value": "Williams,Brown,Allman" }]<br><br>**Constraints**: *Minimum Items*: `1` |
| `expand` | [`List<Expand5Enum>`](../../doc/models/expand-5-enum.md) | Query, Optional | Most endpoints in the API have a way to retrieve extra data related to the current record being retrieved. For example, if the API request is for the accountvaults endpoint, and the end user also needs to know which contact the token belongs to, this data can be returned in the accountvaults endpoint request.<br><br>**Constraints**: *Unique Items Required*, *Pattern*: `^[\w]+$` |
| `format` | [`Format1Enum`](../../doc/models/format-1-enum.md) | Query, Optional | Reporting format, valid values: csv, tsv |
| `typeahead` | `String` | Query, Optional | You can use any `field_name` from this endpoint results to order the list using the value provided as filter for the same `field_name`. It will be ordered using the following rules: 1) Exact match, 2) Starts with, 3) Contains.<br><br>> /endpoint?filter={ "field_name": "Value" }&_typeahead=field_name |
| `fields` | [`List<Field30Enum>`](../../doc/models/field-30-enum.md) | Query, Optional | You can use any `field_name` from this endpoint results to filter the list of fields returned on the response. |

## Response Type

[`ResponseDeclinedRecurringTransactionsCollection`](../../doc/models/response-declined-recurring-transactions-collection.md)

## Example Usage

```java
Page page = new Page.Builder()
    .number(1)
    .size(50)
    .build();

List<Order21> order = Arrays.asList(
    new Order21.Builder(
        "first_name",
        OperatorEnum.ASC
    )
    .build()
);

List<FilterBy> filterBy = Arrays.asList(
    new FilterBy.Builder(
        "first_name",
        FilterByOperator.fromOperator1(
            Operator1Enum.ENUM_1
        ),
        FilterByValue.fromFilterByValueCase1(
            FilterByValueCase1.fromString(
                "Fred"
            )
        )
    )
    .build()
);

declinedRecurringTransactionsController.listAllDeclinedRecurringTransactionsAsync(page, order, filterBy, null, null, null, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof Response401tokenException) {
        Response401tokenException response401tokenException = (Response401tokenException) cause;
        response401tokenException.printStackTrace();
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
  "type": "DeclinedRecurringTransactionsCollection",
  "list": [
    {
      "id": "11e95f8ec39de8fbdb0a4f1a",
      "status": "paid",
      "recurring_id": "11e95f8ec39de8fbdb0a4f1a",
      "created_ts": 1422040992,
      "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
      "modified_ts": 1422040992,
      "modified_user_id": "11e95f8ec39de8fbdb0a4f1a"
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
| 401 | Unauthorized | [`Response401tokenException`](../../doc/models/response-401-token-exception.md) |


# Create a Payment

```java
CompletableFuture<ResponseDeclinedRecurringTransactionPayment> createAPaymentAsync(
    final V1DeclinedRecurringTransactionPaymentsRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`V1DeclinedRecurringTransactionPaymentsRequest`](../../doc/models/v1-declined-recurring-transaction-payments-request.md) | Body, Required | - |

## Response Type

[`ResponseDeclinedRecurringTransactionPayment`](../../doc/models/response-declined-recurring-transaction-payment.md)

## Example Usage

```java
V1DeclinedRecurringTransactionPaymentsRequest body = new V1DeclinedRecurringTransactionPaymentsRequest.Builder(
    "11e95f8ec39de8fbdb0a4f1a",
    "5454545454545454",
    "0722",
    0
)
.accountHolderName("John Doe")
.description("Description")
.saveAccountTitle("John Account")
.subtotalAmount(599)
.surchargeAmount(599)
.build();

declinedRecurringTransactionsController.createAPaymentAsync(body).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof Response401tokenException) {
        Response401tokenException response401tokenException = (Response401tokenException) cause;
        response401tokenException.printStackTrace();
    } else if (cause instanceof Response412Exception) {
        Response412Exception response412Exception = (Response412Exception) cause;
        response412Exception.printStackTrace();
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
  "type": "DeclinedRecurringTransactionPayment",
  "data": {
    "declined_recurring_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
    "account_number": "5454545454545454",
    "account_holder_name": "John Doe",
    "exp_date": "0722",
    "transaction_amount": 0,
    "description": "Description",
    "billing_address": {
      "postal_code": "48375",
      "city": "Novi",
      "state": "Michigan",
      "phone": "3339998822",
      "country": "USA"
    },
    "tags": [
      "Walk-in Customer"
    ],
    "id": "11e95f8ec39de8fbdb0a4f1a",
    "first_six": "700953",
    "last_four": "3657",
    "routing": null,
    "reason_code_id": 1000,
    "created_ts": 1422040992,
    "created_user_id": "11e95f8ec39de8fbdb0a4f1a"
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401tokenException`](../../doc/models/response-401-token-exception.md) |
| 412 | Precondition Failed | [`Response412Exception`](../../doc/models/response-412-exception.md) |


# Rerun the Transaction

```java
CompletableFuture<ResponseDeclinedRecurringTransaction> rerunTheTransactionAsync(
    final String declinedRecurringTransactionId,
    final List<Expand5Enum> expand)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `declinedRecurringTransactionId` | `String` | Template, Required | Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `expand` | [`List<Expand5Enum>`](../../doc/models/expand-5-enum.md) | Query, Optional | Most endpoints in the API have a way to retrieve extra data related to the current record being retrieved. For example, if the API request is for the accountvaults endpoint, and the end user also needs to know which contact the token belongs to, this data can be returned in the accountvaults endpoint request.<br><br>**Constraints**: *Unique Items Required*, *Pattern*: `^[\w]+$` |

## Response Type

[`ResponseDeclinedRecurringTransaction`](../../doc/models/response-declined-recurring-transaction.md)

## Example Usage

```java
String declinedRecurringTransactionId = "11e95f8ec39de8fbdb0a4f1a";
declinedRecurringTransactionsController.rerunTheTransactionAsync(declinedRecurringTransactionId, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof Response401tokenException) {
        Response401tokenException response401tokenException = (Response401tokenException) cause;
        response401tokenException.printStackTrace();
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
  "type": "DeclinedRecurringTransaction",
  "data": {
    "id": "11e95f8ec39de8fbdb0a4f1a",
    "status": "paid",
    "recurring_id": "11e95f8ec39de8fbdb0a4f1a",
    "created_ts": 1422040992,
    "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
    "modified_ts": 1422040992,
    "modified_user_id": "11e95f8ec39de8fbdb0a4f1a"
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401tokenException`](../../doc/models/response-401-token-exception.md) |


# Resend the Transaction

```java
CompletableFuture<ResponseDeclinedRecurringTransactionResend> resendTheTransactionAsync(
    final String declinedRecurringTransactionId)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `declinedRecurringTransactionId` | `String` | Template, Required | Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |

## Response Type

[`ResponseDeclinedRecurringTransactionResend`](../../doc/models/response-declined-recurring-transaction-resend.md)

## Example Usage

```java
String declinedRecurringTransactionId = "11e95f8ec39de8fbdb0a4f1a";

declinedRecurringTransactionsController.resendTheTransactionAsync(declinedRecurringTransactionId).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof Response401tokenException) {
        Response401tokenException response401tokenException = (Response401tokenException) cause;
        response401tokenException.printStackTrace();
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
  "type": "DeclinedRecurringTransactionResend",
  "data": {
    "id": "11e95f8ec39de8fbdb0a4f1a",
    "email_log_id": "11e95f8ec39de8fbdb0a4f1a",
    "email": "email@domain.com"
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401tokenException`](../../doc/models/response-401-token-exception.md) |

