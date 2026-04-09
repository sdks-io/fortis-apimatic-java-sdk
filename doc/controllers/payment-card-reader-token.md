# Payment Card Reader Token

```java
PaymentCardReaderTokenController paymentCardReaderTokenController = client.getPaymentCardReaderTokenController();
```

## Class Name

`PaymentCardReaderTokenController`


# Payment Card Reader Token Request

For initializing iPhone card readers for Apple Tap to Pay transactions

```java
CompletableFuture<ResponsePaymentCardReaderToken> paymentCardReaderTokenRequestAsync(
    final String productTransactionId)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `productTransactionId` | `String` | Query, Required | Product Transaction ID to be used to initialize the card reader<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |

## Response Type

[`ResponsePaymentCardReaderToken`](../../doc/models/response-payment-card-reader-token.md)

## Example Usage

```java
String productTransactionId = "11e95f8ec39de8fbdb0a4f1a";

paymentCardReaderTokenController.paymentCardReaderTokenRequestAsync(productTransactionId).thenAccept(result -> {
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
  "type": "PaymentCardReaderToken",
  "data": {}
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401tokenException`](../../doc/models/response-401-token-exception.md) |

