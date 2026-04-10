# 3 DS Authentication

```java
M3DsAuthenticationController m3DsAuthenticationController = client.getM3DsAuthenticationController();
```

## Class Name

`M3DsAuthenticationController`


# 3 DS Authentication Request

Makes a 3DS Authentication request to authenticate a card or begin the challenge flow.  If a challenge is required, a POST should be made to acs_url using the value of base64_encoded_challenge_request for the value of "creq" using x-www-form-urlencoded for the challenge request to the ACS.

```java
CompletableFuture<ApiResponse<ResponseThreeDsAuthentication>> m3DsAuthenticationRequestAsync(
    final V1MerchantThreedsecureAuthenticationRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`V1MerchantThreedsecureAuthenticationRequest`](../../doc/models/v1-merchant-threedsecure-authentication-request.md) | Body, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`ResponseThreeDsAuthentication`](../../doc/models/response-three-ds-authentication.md).

## Example Usage

```java
V1MerchantThreedsecureAuthenticationRequest body = new V1MerchantThreedsecureAuthenticationRequest.Builder(
    "11ee3860e2fc7f5ea67d36b3",
    DeviceChannel.ENUM_02,
    MessageCategory.ENUM_82,
    new ThreeDsRequestor1.Builder(
        ThreeDsRequestorAuthenticationInd.ENUM_90
    )
    .threeDsRequestorChallengeInd(Arrays.asList(
            ThreeDsRequestorChallengeInd.ENUM_03
        ))
    .build(),
    new CardholderAccount1.Builder(
        "5454545454545454",
        SchemeId.VISA
    )
    .expireDate("2508")
    .build()
)
.enforcePreferredProtocolVersion(true)
.threeDsCompInd("Y")
.build();

m3DsAuthenticationController.m3DsAuthenticationRequestAsync(body).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof V1MerchantThreedsecureAuthentication400ErrorException) {
        V1MerchantThreedsecureAuthentication400ErrorException v1MerchantThreedsecureAuthentication400ErrorException = (V1MerchantThreedsecureAuthentication400ErrorException) cause;
        v1MerchantThreedsecureAuthentication400ErrorException.printStackTrace();
    } else if (cause instanceof Response401TokenException) {
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
  "type": "ThreeDSAuthentication",
  "data": {
    "three_ds_server_trans_id": "ea0c9973-4cd0-4f9f-83b3-609bf22c69e7",
    "acs_url": "https://api.sandbox.fortis.tech/v1/acs/challenge",
    "transaction_status": "C",
    "ds_trans_id": "278c7508-cac6-4233-902d-b90f31f741c6",
    "acs_trans_id": "d7c1ee99-9478-44a6-b1f2-391e29c6b340",
    "message_version": "2.2.0",
    "acs_challenge_mandated": "Y",
    "purchase_date": "20240509111532",
    "base64_encoded_challenge_request": "eyJtZXNzYWdlVHlwZSI6IkNSZXEiLCJ0aHJlZURTU2VydmVyVHJhbnNJRCI6ImVhMGM5OTczLTRjZDAtNGY5Zi04M2IzLTYwOWJmMjJjNjllNyIsImFjc1RyYW5zSUQiOiIwNWViNTE2OS02ZTFkLTQ5NTMtYWQ3NC1hZWU5YmQ4ZTc1YmIiLCJjaGFsbGVuZ2VXaW5kb3dTaXplIjoiMDEiLCJtZXNzYWdlVmVyc2lvbiI6IjIuMi4wIn0="
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 400 | Bad Request | [`V1MerchantThreedsecureAuthentication400ErrorException`](../../doc/models/v1-merchant-threedsecure-authentication-400-error-exception.md) |
| 401 | Unauthorized | [`Response401TokenException`](../../doc/models/response-401-token-exception.md) |
| 412 | Precondition Failed | [`Response412Exception`](../../doc/models/response-412-exception.md) |

