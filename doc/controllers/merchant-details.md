# Merchant Details

```java
MerchantDetailsController merchantDetailsController = client.getMerchantDetailsController();
```

## Class Name

`MerchantDetailsController`


# Merchant Details

Merchant Details

```java
CompletableFuture<ApiResponse<ResponseMerchantDetails>> merchantDetailsAsync(
    final V1WalletProviderMerchantDetailsRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`V1WalletProviderMerchantDetailsRequest`](../../doc/models/v1-wallet-provider-merchant-details-request.md) | Body, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`ResponseMerchantDetails`](../../doc/models/response-merchant-details.md).

## Example Usage

```java
V1WalletProviderMerchantDetailsRequest body = new V1WalletProviderMerchantDetailsRequest.Builder(
    "dev.pay.site"
)
.build();

merchantDetailsController.merchantDetailsAsync(body).thenAccept(result -> {
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
  "type": "MerchantDetails",
  "data": {
    "resultCode": false,
    "merchantID": "abc1234",
    "applePay": true,
    "googlePay": true,
    "applePayDomains": [
      null
    ],
    "message": "valid user",
    "googleJWT": "45r8v29bvj4gc904jfd932nm"
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401TokenException`](../../doc/models/response-401-token-exception.md) |
| 412 | Precondition Failed | [`Response412Exception`](../../doc/models/response-412-exception.md) |

