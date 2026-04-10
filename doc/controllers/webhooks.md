# Webhooks

```java
WebhooksController webhooksController = client.getWebhooksController();
```

## Class Name

`WebhooksController`

## Methods

* [Createanewtransactionbatchpostbackconfig](../../doc/controllers/webhooks.md#createanewtransactionbatchpostbackconfig)
* [Createanewcontactpostbackconfig](../../doc/controllers/webhooks.md#createanewcontactpostbackconfig)
* [Createanewtransactionpostbackconfig](../../doc/controllers/webhooks.md#createanewtransactionpostbackconfig)
* [Deleteapostbackconfig](../../doc/controllers/webhooks.md#deleteapostbackconfig)
* [Updatetransactionbatchpostbackconfig](../../doc/controllers/webhooks.md#updatetransactionbatchpostbackconfig)
* [Updatecontactpostbackconfig](../../doc/controllers/webhooks.md#updatecontactpostbackconfig)
* [Updatetransactionpostbackconfig](../../doc/controllers/webhooks.md#updatetransactionpostbackconfig)


# Createanewtransactionbatchpostbackconfig

```java
CompletableFuture<ApiResponse<ResponseWebhook>> createanewtransactionbatchpostbackconfigAsync(
    final V1WebhooksBatchRequest body,
    final List<Expand123> expand)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`V1WebhooksBatchRequest`](../../doc/models/v1-webhooks-batch-request.md) | Body, Required | - |
| `expand` | [`List<Expand123>`](../../doc/models/expand-123.md) | Query, Optional | Most endpoints in the API have a way to retrieve extra data related to the current record being retrieved. For example, if the API request is for the accountvaults endpoint, and the end user also needs to know which contact the token belongs to, this data can be returned in the accountvaults endpoint request.<br><br>**Constraints**: *Unique Items Required* |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`ResponseWebhook`](../../doc/models/response-webhook.md).

## Example Usage

```java
V1WebhooksBatchRequest body = new V1WebhooksBatchRequest.Builder(
    true,
    "11e95f8ec39de8fbdb0a4f1a",
    true,
    true,
    true,
    "11e95f8ec39de8fbdb0a4f1a",
    1,
    "https://127.0.0.1/receiver"
)
.attemptInterval(300)
.basicAuthUsername("tester")
.basicAuthPassword("Test@522")
.expands("changelogs,tags")
.legacy(true)
.postbackConfigId("11e95f8ec39de8fbdb0a4f1a")
.build();

webhooksController.createanewtransactionbatchpostbackconfigAsync(body, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof Response401TokenException) {
        Response401TokenException response401TokenException = (Response401TokenException) cause;
        response401TokenException.printStackTrace();
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
  "type": "Webhook",
  "data": {
    "attempt_interval": 300,
    "basic_auth_username": "username",
    "basic_auth_password": "password",
    "expands": "changelogs,tags",
    "format": "api-default",
    "is_active": true,
    "location_id": "11e95f8ec39de8fbdb0a4f1a",
    "on_create": true,
    "on_update": true,
    "on_delete": true,
    "legacy": true,
    "postback_config_id": "11e95f8ec39de8fbdb0a4f1a",
    "product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
    "resource": "contact",
    "number_of_attempts": 1,
    "url": "https://127.0.0.1/receiver",
    "id": "11e95f8ec39de8fbdb0a4f1a",
    "postback_logs": [
      {
        "id": "11e95f8ec39de8fbdb0a4f1a",
        "postback_config_id": "11e95f8ec39de8fbdb0a4f1a",
        "changelog_id": "11e95f8ec39de8fbdb0a4f1a",
        "next_run_ts": 1422040992,
        "created_ts": 1422040992,
        "model_id": "11e95f8ec39de8fbdb0a4f1a"
      }
    ]
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401TokenException`](../../doc/models/response-401-token-exception.md) |
| 412 | Precondition Failed | [`Response412Exception`](../../doc/models/response-412-exception.md) |


# Createanewcontactpostbackconfig

```java
CompletableFuture<ApiResponse<ResponseWebhook>> createanewcontactpostbackconfigAsync(
    final V1WebhooksContactRequest body,
    final List<Expand123> expand)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`V1WebhooksContactRequest`](../../doc/models/v1-webhooks-contact-request.md) | Body, Required | - |
| `expand` | [`List<Expand123>`](../../doc/models/expand-123.md) | Query, Optional | Most endpoints in the API have a way to retrieve extra data related to the current record being retrieved. For example, if the API request is for the accountvaults endpoint, and the end user also needs to know which contact the token belongs to, this data can be returned in the accountvaults endpoint request.<br><br>**Constraints**: *Unique Items Required* |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`ResponseWebhook`](../../doc/models/response-webhook.md).

## Example Usage

```java
V1WebhooksContactRequest body = new V1WebhooksContactRequest.Builder(
    true,
    "11e95f8ec39de8fbdb0a4f1a",
    true,
    true,
    true,
    1,
    "https://127.0.0.1/receiver"
)
.attemptInterval(300)
.basicAuthUsername("tester")
.basicAuthPassword("Test@522")
.expands("changelogs,tags")
.legacy(true)
.postbackConfigId("11e95f8ec39de8fbdb0a4f1a")
.productTransactionId("11e95f8ec39de8fbdb0a4f1a")
.build();

webhooksController.createanewcontactpostbackconfigAsync(body, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof Response401TokenException) {
        Response401TokenException response401TokenException = (Response401TokenException) cause;
        response401TokenException.printStackTrace();
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
  "type": "Webhook",
  "data": {
    "attempt_interval": 300,
    "basic_auth_username": "username",
    "basic_auth_password": "password",
    "expands": "changelogs,tags",
    "format": "api-default",
    "is_active": true,
    "location_id": "11e95f8ec39de8fbdb0a4f1a",
    "on_create": true,
    "on_update": true,
    "on_delete": true,
    "legacy": true,
    "postback_config_id": "11e95f8ec39de8fbdb0a4f1a",
    "product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
    "resource": "contact",
    "number_of_attempts": 1,
    "url": "https://127.0.0.1/receiver",
    "id": "11e95f8ec39de8fbdb0a4f1a",
    "postback_logs": [
      {
        "id": "11e95f8ec39de8fbdb0a4f1a",
        "postback_config_id": "11e95f8ec39de8fbdb0a4f1a",
        "changelog_id": "11e95f8ec39de8fbdb0a4f1a",
        "next_run_ts": 1422040992,
        "created_ts": 1422040992,
        "model_id": "11e95f8ec39de8fbdb0a4f1a"
      }
    ]
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401TokenException`](../../doc/models/response-401-token-exception.md) |
| 412 | Precondition Failed | [`Response412Exception`](../../doc/models/response-412-exception.md) |


# Createanewtransactionpostbackconfig

```java
CompletableFuture<ApiResponse<ResponseWebhook>> createanewtransactionpostbackconfigAsync(
    final V1WebhooksTransactionRequest body,
    final List<Expand123> expand)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`V1WebhooksTransactionRequest`](../../doc/models/v1-webhooks-transaction-request.md) | Body, Required | - |
| `expand` | [`List<Expand123>`](../../doc/models/expand-123.md) | Query, Optional | Most endpoints in the API have a way to retrieve extra data related to the current record being retrieved. For example, if the API request is for the accountvaults endpoint, and the end user also needs to know which contact the token belongs to, this data can be returned in the accountvaults endpoint request.<br><br>**Constraints**: *Unique Items Required* |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`ResponseWebhook`](../../doc/models/response-webhook.md).

## Example Usage

```java
V1WebhooksTransactionRequest body = new V1WebhooksTransactionRequest.Builder(
    true,
    "11e95f8ec39de8fbdb0a4f1a",
    true,
    true,
    true,
    "11e95f8ec39de8fbdb0a4f1a",
    1,
    "https://127.0.0.1/receiver"
)
.attemptInterval(300)
.basicAuthUsername("tester")
.basicAuthPassword("Test@522")
.expands("changelogs,tags")
.legacy(true)
.postbackConfigId("11e95f8ec39de8fbdb0a4f1a")
.build();

webhooksController.createanewtransactionpostbackconfigAsync(body, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof Response401TokenException) {
        Response401TokenException response401TokenException = (Response401TokenException) cause;
        response401TokenException.printStackTrace();
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
  "type": "Webhook",
  "data": {
    "attempt_interval": 300,
    "basic_auth_username": "username",
    "basic_auth_password": "password",
    "expands": "changelogs,tags",
    "format": "api-default",
    "is_active": true,
    "location_id": "11e95f8ec39de8fbdb0a4f1a",
    "on_create": true,
    "on_update": true,
    "on_delete": true,
    "legacy": true,
    "postback_config_id": "11e95f8ec39de8fbdb0a4f1a",
    "product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
    "resource": "contact",
    "number_of_attempts": 1,
    "url": "https://127.0.0.1/receiver",
    "id": "11e95f8ec39de8fbdb0a4f1a",
    "postback_logs": [
      {
        "id": "11e95f8ec39de8fbdb0a4f1a",
        "postback_config_id": "11e95f8ec39de8fbdb0a4f1a",
        "changelog_id": "11e95f8ec39de8fbdb0a4f1a",
        "next_run_ts": 1422040992,
        "created_ts": 1422040992,
        "model_id": "11e95f8ec39de8fbdb0a4f1a"
      }
    ]
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401TokenException`](../../doc/models/response-401-token-exception.md) |
| 412 | Precondition Failed | [`Response412Exception`](../../doc/models/response-412-exception.md) |


# Deleteapostbackconfig

```java
CompletableFuture<ApiResponse<ResponseWebhook>> deleteapostbackconfigAsync(
    final String webhookId)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `webhookId` | `String` | Template, Required | Postback Config ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`ResponseWebhook`](../../doc/models/response-webhook.md).

## Example Usage

```java
String webhookId = "11e95f8ec39de8fbdb0a4f1a";

webhooksController.deleteapostbackconfigAsync(webhookId).thenAccept(result -> {
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
  "type": "Webhook",
  "data": {
    "attempt_interval": 300,
    "basic_auth_username": "username",
    "basic_auth_password": "password",
    "expands": "changelogs,tags",
    "format": "api-default",
    "is_active": true,
    "location_id": "11e95f8ec39de8fbdb0a4f1a",
    "on_create": true,
    "on_update": true,
    "on_delete": true,
    "legacy": true,
    "postback_config_id": "11e95f8ec39de8fbdb0a4f1a",
    "product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
    "resource": "contact",
    "number_of_attempts": 1,
    "url": "https://127.0.0.1/receiver",
    "id": "11e95f8ec39de8fbdb0a4f1a",
    "postback_logs": [
      {
        "id": "11e95f8ec39de8fbdb0a4f1a",
        "postback_config_id": "11e95f8ec39de8fbdb0a4f1a",
        "changelog_id": "11e95f8ec39de8fbdb0a4f1a",
        "next_run_ts": 1422040992,
        "created_ts": 1422040992,
        "model_id": "11e95f8ec39de8fbdb0a4f1a"
      }
    ]
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401TokenException`](../../doc/models/response-401-token-exception.md) |


# Updatetransactionbatchpostbackconfig

```java
CompletableFuture<ApiResponse<ResponseWebhook>> updatetransactionbatchpostbackconfigAsync(
    final String webhookId,
    final V1WebhooksBatchRequest1 body,
    final List<Expand123> expand)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `webhookId` | `String` | Template, Required | Postback Config ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `body` | [`V1WebhooksBatchRequest1`](../../doc/models/v1-webhooks-batch-request-1.md) | Body, Required | - |
| `expand` | [`List<Expand123>`](../../doc/models/expand-123.md) | Query, Optional | Most endpoints in the API have a way to retrieve extra data related to the current record being retrieved. For example, if the API request is for the accountvaults endpoint, and the end user also needs to know which contact the token belongs to, this data can be returned in the accountvaults endpoint request.<br><br>**Constraints**: *Unique Items Required* |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`ResponseWebhook`](../../doc/models/response-webhook.md).

## Example Usage

```java
String webhookId = "11e95f8ec39de8fbdb0a4f1a";
V1WebhooksBatchRequest1 body = new V1WebhooksBatchRequest1.Builder()
    .attemptInterval(300)
    .basicAuthUsername("tester")
    .basicAuthPassword("Test@522")
    .expands("changelogs,tags")
    .isActive(true)
    .locationId("11e95f8ec39de8fbdb0a4f1a")
    .onCreate(true)
    .onUpdate(true)
    .onDelete(true)
    .legacy(true)
    .postbackConfigId("11e95f8ec39de8fbdb0a4f1a")
    .productTransactionId("11e95f8ec39de8fbdb0a4f1a")
    .numberOfAttempts(1)
    .url("https://127.0.0.1/receiver")
    .build();

webhooksController.updatetransactionbatchpostbackconfigAsync(webhookId, body, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof Response401TokenException) {
        Response401TokenException response401TokenException = (Response401TokenException) cause;
        response401TokenException.printStackTrace();
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
  "type": "Webhook",
  "data": {
    "attempt_interval": 300,
    "basic_auth_username": "username",
    "basic_auth_password": "password",
    "expands": "changelogs,tags",
    "format": "api-default",
    "is_active": true,
    "location_id": "11e95f8ec39de8fbdb0a4f1a",
    "on_create": true,
    "on_update": true,
    "on_delete": true,
    "legacy": true,
    "postback_config_id": "11e95f8ec39de8fbdb0a4f1a",
    "product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
    "resource": "contact",
    "number_of_attempts": 1,
    "url": "https://127.0.0.1/receiver",
    "id": "11e95f8ec39de8fbdb0a4f1a",
    "postback_logs": [
      {
        "id": "11e95f8ec39de8fbdb0a4f1a",
        "postback_config_id": "11e95f8ec39de8fbdb0a4f1a",
        "changelog_id": "11e95f8ec39de8fbdb0a4f1a",
        "next_run_ts": 1422040992,
        "created_ts": 1422040992,
        "model_id": "11e95f8ec39de8fbdb0a4f1a"
      }
    ]
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401TokenException`](../../doc/models/response-401-token-exception.md) |
| 412 | Precondition Failed | [`Response412Exception`](../../doc/models/response-412-exception.md) |


# Updatecontactpostbackconfig

```java
CompletableFuture<ApiResponse<ResponseWebhook>> updatecontactpostbackconfigAsync(
    final String webhookId,
    final V1WebhooksContactRequest1 body,
    final List<Expand123> expand)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `webhookId` | `String` | Template, Required | Postback Config ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `body` | [`V1WebhooksContactRequest1`](../../doc/models/v1-webhooks-contact-request-1.md) | Body, Required | - |
| `expand` | [`List<Expand123>`](../../doc/models/expand-123.md) | Query, Optional | Most endpoints in the API have a way to retrieve extra data related to the current record being retrieved. For example, if the API request is for the accountvaults endpoint, and the end user also needs to know which contact the token belongs to, this data can be returned in the accountvaults endpoint request.<br><br>**Constraints**: *Unique Items Required* |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`ResponseWebhook`](../../doc/models/response-webhook.md).

## Example Usage

```java
String webhookId = "11e95f8ec39de8fbdb0a4f1a";
V1WebhooksContactRequest1 body = new V1WebhooksContactRequest1.Builder()
    .attemptInterval(300)
    .basicAuthUsername("tester")
    .basicAuthPassword("Test@522")
    .expands("changelogs,tags")
    .isActive(true)
    .locationId("11e95f8ec39de8fbdb0a4f1a")
    .onCreate(true)
    .onUpdate(true)
    .onDelete(true)
    .legacy(true)
    .postbackConfigId("11e95f8ec39de8fbdb0a4f1a")
    .productTransactionId("11e95f8ec39de8fbdb0a4f1a")
    .numberOfAttempts(1)
    .url("https://127.0.0.1/receiver")
    .build();

webhooksController.updatecontactpostbackconfigAsync(webhookId, body, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof Response401TokenException) {
        Response401TokenException response401TokenException = (Response401TokenException) cause;
        response401TokenException.printStackTrace();
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
  "type": "Webhook",
  "data": {
    "attempt_interval": 300,
    "basic_auth_username": "username",
    "basic_auth_password": "password",
    "expands": "changelogs,tags",
    "format": "api-default",
    "is_active": true,
    "location_id": "11e95f8ec39de8fbdb0a4f1a",
    "on_create": true,
    "on_update": true,
    "on_delete": true,
    "legacy": true,
    "postback_config_id": "11e95f8ec39de8fbdb0a4f1a",
    "product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
    "resource": "contact",
    "number_of_attempts": 1,
    "url": "https://127.0.0.1/receiver",
    "id": "11e95f8ec39de8fbdb0a4f1a",
    "postback_logs": [
      {
        "id": "11e95f8ec39de8fbdb0a4f1a",
        "postback_config_id": "11e95f8ec39de8fbdb0a4f1a",
        "changelog_id": "11e95f8ec39de8fbdb0a4f1a",
        "next_run_ts": 1422040992,
        "created_ts": 1422040992,
        "model_id": "11e95f8ec39de8fbdb0a4f1a"
      }
    ]
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401TokenException`](../../doc/models/response-401-token-exception.md) |
| 412 | Precondition Failed | [`Response412Exception`](../../doc/models/response-412-exception.md) |


# Updatetransactionpostbackconfig

```java
CompletableFuture<ApiResponse<ResponseWebhook>> updatetransactionpostbackconfigAsync(
    final String webhookId,
    final V1WebhooksTransactionRequest1 body,
    final List<Expand123> expand)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `webhookId` | `String` | Template, Required | Postback Config ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `body` | [`V1WebhooksTransactionRequest1`](../../doc/models/v1-webhooks-transaction-request-1.md) | Body, Required | - |
| `expand` | [`List<Expand123>`](../../doc/models/expand-123.md) | Query, Optional | Most endpoints in the API have a way to retrieve extra data related to the current record being retrieved. For example, if the API request is for the accountvaults endpoint, and the end user also needs to know which contact the token belongs to, this data can be returned in the accountvaults endpoint request.<br><br>**Constraints**: *Unique Items Required* |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`ResponseWebhook`](../../doc/models/response-webhook.md).

## Example Usage

```java
String webhookId = "11e95f8ec39de8fbdb0a4f1a";
V1WebhooksTransactionRequest1 body = new V1WebhooksTransactionRequest1.Builder()
    .attemptInterval(300)
    .basicAuthUsername("tester")
    .basicAuthPassword("Test@522")
    .expands("changelogs,tags")
    .isActive(true)
    .locationId("11e95f8ec39de8fbdb0a4f1a")
    .onCreate(true)
    .onUpdate(true)
    .onDelete(true)
    .legacy(true)
    .postbackConfigId("11e95f8ec39de8fbdb0a4f1a")
    .productTransactionId("11e95f8ec39de8fbdb0a4f1a")
    .numberOfAttempts(1)
    .url("https://127.0.0.1/receiver")
    .build();

webhooksController.updatetransactionpostbackconfigAsync(webhookId, body, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof Response401TokenException) {
        Response401TokenException response401TokenException = (Response401TokenException) cause;
        response401TokenException.printStackTrace();
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
  "type": "Webhook",
  "data": {
    "attempt_interval": 300,
    "basic_auth_username": "username",
    "basic_auth_password": "password",
    "expands": "changelogs,tags",
    "format": "api-default",
    "is_active": true,
    "location_id": "11e95f8ec39de8fbdb0a4f1a",
    "on_create": true,
    "on_update": true,
    "on_delete": true,
    "legacy": true,
    "postback_config_id": "11e95f8ec39de8fbdb0a4f1a",
    "product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
    "resource": "contact",
    "number_of_attempts": 1,
    "url": "https://127.0.0.1/receiver",
    "id": "11e95f8ec39de8fbdb0a4f1a",
    "postback_logs": [
      {
        "id": "11e95f8ec39de8fbdb0a4f1a",
        "postback_config_id": "11e95f8ec39de8fbdb0a4f1a",
        "changelog_id": "11e95f8ec39de8fbdb0a4f1a",
        "next_run_ts": 1422040992,
        "created_ts": 1422040992,
        "model_id": "11e95f8ec39de8fbdb0a4f1a"
      }
    ]
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401TokenException`](../../doc/models/response-401-token-exception.md) |
| 412 | Precondition Failed | [`Response412Exception`](../../doc/models/response-412-exception.md) |

