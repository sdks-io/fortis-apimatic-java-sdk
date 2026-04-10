# Async Processing

```java
AsyncProcessingController asyncProcessingController = client.getAsyncProcessingController();
```

## Class Name

`AsyncProcessingController`


# Status Check

Retrieve the current status for a particular code.

```java
CompletableFuture<ApiResponse<ResponseAsyncStatus>> statusCheckAsync(
    final UUID statusCode)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `statusCode` | `UUID` | Template, Required | A [UUID v4](https://datatracker.ietf.org/doc/html/rfc4122) that's unique for the Async Request |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`ResponseAsyncStatus`](../../doc/models/response-async-status.md).

## Example Usage

```java
UUID statusCode = UUID.fromString("406c66c3-21cb-47fb-80fc-843bc42507fb");

asyncProcessingController.statusCheckAsync(statusCode).thenAccept(result -> {
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
  "type": "AsyncStatus",
  "data": {
    "code": "406c66c3-21cb-47fb-80fc-843bc42507fb",
    "type": "Transaction",
    "id": "11e95f8ec39de8fbdb0a4f1a",
    "progress": 100,
    "error": null,
    "ttl": 7956886942
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401TokenException`](../../doc/models/response-401-token-exception.md) |

