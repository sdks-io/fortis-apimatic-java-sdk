# Paylinks

Paylinks is a way for merchants to create a link that can be used to make a payment. The link can optionally be sent out via email/sms to a customer. Paylinks is similar to Quick Invoices but much simpler.

```java
PaylinksController paylinksController = client.getPaylinksController();
```

## Class Name

`PaylinksController`

## Methods

* [Create a New Paylink](../../doc/controllers/paylinks.md#create-a-new-paylink)
* [List All Paylinks](../../doc/controllers/paylinks.md#list-all-paylinks)
* [Delete Paylink](../../doc/controllers/paylinks.md#delete-paylink)
* [View Single Paylink](../../doc/controllers/paylinks.md#view-single-paylink)
* [Update Paylink](../../doc/controllers/paylinks.md#update-paylink)
* [Resend Paylink](../../doc/controllers/paylinks.md#resend-paylink)


# Create a New Paylink

Generate a new Paylink to be sent via email, sms or grab the payment_url to embed in you own messaging system.

```java
CompletableFuture<ResponsePaylink> createANewPaylinkAsync(
    final V1PaylinksRequest body,
    final List<Expand17Enum> expand)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`V1PaylinksRequest`](../../doc/models/v1-paylinks-request.md) | Body, Required | - |
| `expand` | [`List<Expand17Enum>`](../../doc/models/expand-17-enum.md) | Query, Optional | Most endpoints in the API have a way to retrieve extra data related to the current record being retrieved. For example, if the API request is for the accountvaults endpoint, and the end user also needs to know which contact the token belongs to, this data can be returned in the accountvaults endpoint request.<br><br>**Constraints**: *Unique Items Required*, *Pattern*: `^[\w]+$` |

## Response Type

[`ResponsePaylink`](../../doc/models/response-paylink.md)

## Example Usage

```java
V1PaylinksRequest body = new V1PaylinksRequest.Builder(
    1
)
.locationId("11e95f8ec39de8fbdb0a4f1a")
.ccProductTransactionId("11e95f8ec39de8fbdb0a4f1a")
.email("email@domain.com")
.contactId("11e95f8ec39de8fbdb0a4f1a")
.achProductTransactionId("11e95f8ec39de8fbdb0a4f1a")
.expireDate("2021-12-01")
.displayProductTransactionReceiptDetails(true)
.displayBillingFields(true)
.deliveryMethod(DeliveryMethodEnum.ENUM_0)
.cellPhone("3339998822")
.description("Description")
.storeToken(false)
.storeTokenTitle("John Account")
.bankFundedOnlyOverride(false)
.redirectUrlDelay(15D)
.build();

paylinksController.createANewPaylinkAsync(body, null).thenAccept(result -> {
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
  "type": "Paylink",
  "data": {
    "location_id": "11e95f8ec39de8fbdb0a4f1a",
    "cc_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
    "email": "email@domain.com",
    "amount_due": 1,
    "contact_id": "11e95f8ec39de8fbdb0a4f1a",
    "ach_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
    "expire_date": "2021-12-01",
    "display_product_transaction_receipt_details": true,
    "display_billing_fields": true,
    "delivery_method": 0,
    "cell_phone": "3339998822",
    "description": "Description",
    "store_token": false,
    "store_token_title": "John Account",
    "bank_funded_only_override": false,
    "tags": [
      "Tag 1"
    ],
    "redirect_url_delay": 15,
    "redirect_url_on_approve": null,
    "redirect_url_on_decline": null,
    "id": "11e95f8ec39de8fbdb0a4f1a",
    "status_id": true,
    "status_code": 1,
    "active": true,
    "created_ts": 1422040992,
    "modified_ts": 1422040992,
    "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
    "modified_user_id": "11e95f8ec39de8fbdb0a4f1a"
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401tokenException`](../../doc/models/response-401-token-exception.md) |
| 412 | Precondition Failed | [`Response412Exception`](../../doc/models/response-412-exception.md) |


# List All Paylinks

Pull in all Paylinks associated with the location_id.

```java
CompletableFuture<ResponsePaylinksCollection> listAllPaylinksAsync(
    final Page page,
    final List<Order21> order,
    final List<FilterBy> filterBy,
    final List<Expand18Enum> expand,
    final Format1Enum format,
    final String typeahead,
    final List<Field39Enum> fields)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `page` | [`Page`](../../doc/models/page.md) | Query, Optional | Use this field to specify paginate your results, by using page size and number. You can use one of the following methods:<br><br>> /endpoint?page={ "number": 1, "size": 50 }<br>> <br>> /endpoint?page[number]=1&page[size]=50 |
| `order` | [`List<Order21>`](../../doc/models/order-21.md) | Query, Optional | Criteria used in query string parameters to order results.  Most fields from the endpoint results can be used as a `key`.  Unsupported fields or operators will return a `412`.  Must be encoded, or use syntax that does not require encoding.<br><br>> /endpoint?order[0][key]=created_ts&order[0][operator]=asc<br>> <br>> /endpoint?order=[{ "key": "created_ts", "operator": "asc"}]<br>> <br>> /endpoint?order=[{ "key": "balance", "operator": "desc"},{ "key": "created_ts", "operator": "asc"}]<br><br>**Constraints**: *Minimum Items*: `1` |
| `filterBy` | [`List<FilterBy>`](../../doc/models/filter-by.md) | Query, Optional | Filter criteria that can be used in query string parameters.  Most fields from the endpoint results can be used as a `key`.  Unsupported fields or operators will return a `412`. Must be encoded, or use syntax that does not require encoding.<br><br>> ?filter_by[0][key]=first_name&filter_by[0][operator]==&filter_by[0][value]=Steve<br>> <br>> /endpoint?filter_by=[{ "key": "first_name", "operator": "=", "value": "Fred" }]<br>> <br>> /endpoint?filter_by=[{ "key": "account_type", "operator": "=", "value": "VISA" }]<br>> <br>> /endpoint?filter_by=[{ "key": "created_ts", "operator": ">=", "value": "946702799" }, { "key": "created_ts", "operator": "<=", value: "1695061891" }]<br>> <br>> /endpoint?filter_by=[{ "key": "last_name", "operator": "IN", "value": "Williams,Brown,Allman" }]<br><br>**Constraints**: *Minimum Items*: `1` |
| `expand` | [`List<Expand18Enum>`](../../doc/models/expand-18-enum.md) | Query, Optional | Most endpoints in the API have a way to retrieve extra data related to the current record being retrieved. For example, if the API request is for the accountvaults endpoint, and the end user also needs to know which contact the token belongs to, this data can be returned in the accountvaults endpoint request.<br><br>**Constraints**: *Unique Items Required*, *Pattern*: `^[\w]+$` |
| `format` | [`Format1Enum`](../../doc/models/format-1-enum.md) | Query, Optional | Reporting format, valid values: csv, tsv |
| `typeahead` | `String` | Query, Optional | You can use any `field_name` from this endpoint results to order the list using the value provided as filter for the same `field_name`. It will be ordered using the following rules: 1) Exact match, 2) Starts with, 3) Contains.<br><br>> /endpoint?filter={ "field_name": "Value" }&_typeahead=field_name |
| `fields` | [`List<Field39Enum>`](../../doc/models/field-39-enum.md) | Query, Optional | You can use any `field_name` from this endpoint results to filter the list of fields returned on the response. |

## Response Type

[`ResponsePaylinksCollection`](../../doc/models/response-paylinks-collection.md)

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

paylinksController.listAllPaylinksAsync(page, order, filterBy, null, null, null, null).thenAccept(result -> {
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
  "type": "PaylinksCollection",
  "list": [
    {
      "location_id": "11e95f8ec39de8fbdb0a4f1a",
      "cc_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
      "email": "email@domain.com",
      "amount_due": 1,
      "contact_id": "11e95f8ec39de8fbdb0a4f1a",
      "ach_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
      "expire_date": "2021-12-01",
      "display_product_transaction_receipt_details": true,
      "display_billing_fields": true,
      "delivery_method": 0,
      "cell_phone": "3339998822",
      "description": "Description",
      "store_token": false,
      "store_token_title": "John Account",
      "bank_funded_only_override": false,
      "tags": [
        "Tag 1"
      ],
      "redirect_url_delay": 15,
      "redirect_url_on_approve": null,
      "redirect_url_on_decline": null,
      "id": "11e95f8ec39de8fbdb0a4f1a",
      "status_id": true,
      "status_code": 1,
      "active": true,
      "created_ts": 1422040992,
      "modified_ts": 1422040992,
      "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
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


# Delete Paylink

Delete an existing Paylink_id

```java
CompletableFuture<ResponsePaylink> deletePaylinkAsync(
    final String paylinkId)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `paylinkId` | `String` | Template, Required | System generatedPaylink Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |

## Response Type

[`ResponsePaylink`](../../doc/models/response-paylink.md)

## Example Usage

```java
String paylinkId = "11e95f8ec39de8fbdb0a4f1a";

paylinksController.deletePaylinkAsync(paylinkId).thenAccept(result -> {
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
  "type": "Paylink",
  "data": {
    "location_id": "11e95f8ec39de8fbdb0a4f1a",
    "cc_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
    "email": "email@domain.com",
    "amount_due": 1,
    "contact_id": "11e95f8ec39de8fbdb0a4f1a",
    "ach_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
    "expire_date": "2021-12-01",
    "display_product_transaction_receipt_details": true,
    "display_billing_fields": true,
    "delivery_method": 0,
    "cell_phone": "3339998822",
    "description": "Description",
    "store_token": false,
    "store_token_title": "John Account",
    "bank_funded_only_override": false,
    "tags": [
      "Tag 1"
    ],
    "redirect_url_delay": 15,
    "redirect_url_on_approve": null,
    "redirect_url_on_decline": null,
    "id": "11e95f8ec39de8fbdb0a4f1a",
    "status_id": true,
    "status_code": 1,
    "active": true,
    "created_ts": 1422040992,
    "modified_ts": 1422040992,
    "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
    "modified_user_id": "11e95f8ec39de8fbdb0a4f1a"
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401tokenException`](../../doc/models/response-401-token-exception.md) |


# View Single Paylink

Use the Paylink_id obtained from the Create request to look up the status

```java
CompletableFuture<ResponsePaylink> viewSinglePaylinkAsync(
    final String paylinkId,
    final List<Expand18Enum> expand,
    final List<Field39Enum> fields)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `paylinkId` | `String` | Template, Required | System generatedPaylink Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `expand` | [`List<Expand18Enum>`](../../doc/models/expand-18-enum.md) | Query, Optional | Most endpoints in the API have a way to retrieve extra data related to the current record being retrieved. For example, if the API request is for the accountvaults endpoint, and the end user also needs to know which contact the token belongs to, this data can be returned in the accountvaults endpoint request.<br><br>**Constraints**: *Unique Items Required*, *Pattern*: `^[\w]+$` |
| `fields` | [`List<Field39Enum>`](../../doc/models/field-39-enum.md) | Query, Optional | You can use any `field_name` from this endpoint results to filter the list of fields returned on the response. |

## Response Type

[`ResponsePaylink`](../../doc/models/response-paylink.md)

## Example Usage

```java
String paylinkId = "11e95f8ec39de8fbdb0a4f1a";
paylinksController.viewSinglePaylinkAsync(paylinkId, null, null).thenAccept(result -> {
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
  "type": "Paylink",
  "data": {
    "location_id": "11e95f8ec39de8fbdb0a4f1a",
    "cc_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
    "email": "email@domain.com",
    "amount_due": 1,
    "contact_id": "11e95f8ec39de8fbdb0a4f1a",
    "ach_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
    "expire_date": "2021-12-01",
    "display_product_transaction_receipt_details": true,
    "display_billing_fields": true,
    "delivery_method": 0,
    "cell_phone": "3339998822",
    "description": "Description",
    "store_token": false,
    "store_token_title": "John Account",
    "bank_funded_only_override": false,
    "tags": [
      "Tag 1"
    ],
    "redirect_url_delay": 15,
    "redirect_url_on_approve": null,
    "redirect_url_on_decline": null,
    "id": "11e95f8ec39de8fbdb0a4f1a",
    "status_id": true,
    "status_code": 1,
    "active": true,
    "created_ts": 1422040992,
    "modified_ts": 1422040992,
    "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
    "modified_user_id": "11e95f8ec39de8fbdb0a4f1a"
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401tokenException`](../../doc/models/response-401-token-exception.md) |


# Update Paylink

Update an existing Paylink_id

```java
CompletableFuture<ResponsePaylink> updatePaylinkAsync(
    final String paylinkId,
    final V1PaylinksRequest1 body,
    final List<Expand17Enum> expand)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `paylinkId` | `String` | Template, Required | System generatedPaylink Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `body` | [`V1PaylinksRequest1`](../../doc/models/v1-paylinks-request-1.md) | Body, Required | - |
| `expand` | [`List<Expand17Enum>`](../../doc/models/expand-17-enum.md) | Query, Optional | Most endpoints in the API have a way to retrieve extra data related to the current record being retrieved. For example, if the API request is for the accountvaults endpoint, and the end user also needs to know which contact the token belongs to, this data can be returned in the accountvaults endpoint request.<br><br>**Constraints**: *Unique Items Required*, *Pattern*: `^[\w]+$` |

## Response Type

[`ResponsePaylink`](../../doc/models/response-paylink.md)

## Example Usage

```java
String paylinkId = "11e95f8ec39de8fbdb0a4f1a";
V1PaylinksRequest1 body = new V1PaylinksRequest1.Builder()
    .locationId("11e95f8ec39de8fbdb0a4f1a")
    .ccProductTransactionId("11e95f8ec39de8fbdb0a4f1a")
    .email("email@domain.com")
    .amountDue(1)
    .contactId("11e95f8ec39de8fbdb0a4f1a")
    .achProductTransactionId("11e95f8ec39de8fbdb0a4f1a")
    .expireDate("2021-12-01")
    .displayProductTransactionReceiptDetails(true)
    .displayBillingFields(true)
    .deliveryMethod(DeliveryMethodEnum.ENUM_0)
    .cellPhone("3339998822")
    .description("Description")
    .storeToken(false)
    .storeTokenTitle("John Account")
    .bankFundedOnlyOverride(false)
    .redirectUrlDelay(15D)
    .build();

paylinksController.updatePaylinkAsync(paylinkId, body, null).thenAccept(result -> {
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
  "type": "Paylink",
  "data": {
    "location_id": "11e95f8ec39de8fbdb0a4f1a",
    "cc_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
    "email": "email@domain.com",
    "amount_due": 1,
    "contact_id": "11e95f8ec39de8fbdb0a4f1a",
    "ach_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
    "expire_date": "2021-12-01",
    "display_product_transaction_receipt_details": true,
    "display_billing_fields": true,
    "delivery_method": 0,
    "cell_phone": "3339998822",
    "description": "Description",
    "store_token": false,
    "store_token_title": "John Account",
    "bank_funded_only_override": false,
    "tags": [
      "Tag 1"
    ],
    "redirect_url_delay": 15,
    "redirect_url_on_approve": null,
    "redirect_url_on_decline": null,
    "id": "11e95f8ec39de8fbdb0a4f1a",
    "status_id": true,
    "status_code": 1,
    "active": true,
    "created_ts": 1422040992,
    "modified_ts": 1422040992,
    "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
    "modified_user_id": "11e95f8ec39de8fbdb0a4f1a"
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401tokenException`](../../doc/models/response-401-token-exception.md) |
| 412 | Precondition Failed | [`Response412Exception`](../../doc/models/response-412-exception.md) |


# Resend Paylink

Resend the Paylink via email or sms

```java
CompletableFuture<ResponsePaylink> resendPaylinkAsync(
    final String paylinkId,
    final List<Expand17Enum> expand,
    final EmailEnum email,
    final SmsEnum sms)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `paylinkId` | `String` | Template, Required | System generatedPaylink Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `expand` | [`List<Expand17Enum>`](../../doc/models/expand-17-enum.md) | Query, Optional | Most endpoints in the API have a way to retrieve extra data related to the current record being retrieved. For example, if the API request is for the accountvaults endpoint, and the end user also needs to know which contact the token belongs to, this data can be returned in the accountvaults endpoint request.<br><br>**Constraints**: *Unique Items Required*, *Pattern*: `^[\w]+$` |
| `email` | [`EmailEnum`](../../doc/models/email-enum.md) | Query, Optional | Resend Email |
| `sms` | [`SmsEnum`](../../doc/models/sms-enum.md) | Query, Optional | Resend SMS |

## Response Type

[`ResponsePaylink`](../../doc/models/response-paylink.md)

## Example Usage

```java
String paylinkId = "11e95f8ec39de8fbdb0a4f1a";

paylinksController.resendPaylinkAsync(paylinkId, null, null, null).thenAccept(result -> {
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
  "type": "Paylink",
  "data": {
    "location_id": "11e95f8ec39de8fbdb0a4f1a",
    "cc_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
    "email": "email@domain.com",
    "amount_due": 1,
    "contact_id": "11e95f8ec39de8fbdb0a4f1a",
    "ach_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
    "expire_date": "2021-12-01",
    "display_product_transaction_receipt_details": true,
    "display_billing_fields": true,
    "delivery_method": 0,
    "cell_phone": "3339998822",
    "description": "Description",
    "store_token": false,
    "store_token_title": "John Account",
    "bank_funded_only_override": false,
    "tags": [
      "Tag 1"
    ],
    "redirect_url_delay": 15,
    "redirect_url_on_approve": null,
    "redirect_url_on_decline": null,
    "id": "11e95f8ec39de8fbdb0a4f1a",
    "status_id": true,
    "status_code": 1,
    "active": true,
    "created_ts": 1422040992,
    "modified_ts": 1422040992,
    "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
    "modified_user_id": "11e95f8ec39de8fbdb0a4f1a"
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401tokenException`](../../doc/models/response-401-token-exception.md) |

