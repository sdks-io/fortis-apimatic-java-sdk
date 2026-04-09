# 3 DS Transactions

```java
M3DSTransactionsController m3DSTransactionsController = client.getM3DSTransactionsController();
```

## Class Name

`M3DSTransactionsController`


# 3 DS Transactions Request

For getting results of successful 3DS authentication attempts

```java
CompletableFuture<ResponseThreeDSTransaction> m3DSTransactionsRequestAsync(
    final String threeDsServerTransId,
    final String productTransactionId)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `threeDsServerTransId` | `String` | Template, Required | Universally unique transaction identifier assigned by the 3DS Server to identify a single transaction. |
| `productTransactionId` | `String` | Query, Required | Product Transaction ID associated with this 3DS request<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |

## Response Type

[`ResponseThreeDSTransaction`](../../doc/models/response-three-ds-transaction.md)

## Example Usage

```java
String threeDsServerTransId = "516ef0bf-e510-4895-b0a8-c889f2eaf471";
String productTransactionId = "11e95f8ec39de8fbdb0a4f1a";

m3DSTransactionsController.m3DSTransactionsRequestAsync(threeDsServerTransId, productTransactionId).thenAccept(result -> {
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
  "type": "ThreeDSTransaction",
  "data": {
    "three_ds_server_trans_id": "516ef0bf-e510-4895-b0a8-c889f2eaf471",
    "transaction_status": "Y",
    "ds_trans_id": "f25084f0-5b16-4c0a-ae5d-b24808a95e4b",
    "acs_trans_id": "d7c1ee99-9478-44a6-b1f2-391e29c6b340",
    "message_version": "2.2.0",
    "authentication_value": "MTIzNDU2Nzg5MDA5ODc2NTQzMjE=",
    "eci": "05"
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401tokenException`](../../doc/models/response-401-token-exception.md) |

