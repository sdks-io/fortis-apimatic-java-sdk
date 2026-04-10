# Apple Pay Validate Merchant

```java
ApplePayValidateMerchantController applePayValidateMerchantController = client.getApplePayValidateMerchantController();
```

## Class Name

`ApplePayValidateMerchantController`


# Apple Pay Validate Merchant

Apple Pay Validate Merchant

```java
CompletableFuture<ApiResponse<ResponseApplePayValidateMerchant>> applePayValidateMerchantAsync(
    final V1WalletProviderApplePayValidateMerchantRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`V1WalletProviderApplePayValidateMerchantRequest`](../../doc/models/v1-wallet-provider-apple-pay-validate-merchant-request.md) | Body, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`ResponseApplePayValidateMerchant`](../../doc/models/response-apple-pay-validate-merchant.md).

## Example Usage

```java
V1WalletProviderApplePayValidateMerchantRequest body = new V1WalletProviderApplePayValidateMerchantRequest.Builder(
    "https://apple-pay-gateway-cert.apple.com/paymentservices/startSession",
    "abc1234",
    "website.domain.com",
    "Sandwich Market"
)
.build();

applePayValidateMerchantController.applePayValidateMerchantAsync(body).thenAccept(result -> {
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
  "type": "ApplePayValidateMerchant",
  "data": {
    "merchantSession": "{\"epochTimestamp\":1689772866529,\"expiresAt\":1689776466529,\"merchantSessionIdentifier\":\"SSH3D9224\",\"nonce\":\"d70dbe8a\",\"merchantIdentifier\":\"46A940\",\"domainName\":\"paygistixcert.paymentlogistics.net\",\"displayName\":\"F\",\"signature\":\"30800609f6e2\",\"operationalAnalyticsIdentifier\":\"F:46A4E40\",\"retries\":0,\"pspId\":\"ADD36D\"}"
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401TokenException`](../../doc/models/response-401-token-exception.md) |
| 412 | Precondition Failed | [`Response412Exception`](../../doc/models/response-412-exception.md) |

