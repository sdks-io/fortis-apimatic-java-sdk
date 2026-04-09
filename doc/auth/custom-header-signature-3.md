
# Custom Header Signature



Documentation for accessing and setting credentials for access-token.

## Auth Credentials

| Name | Type | Description | Setter | Getter |
|  --- | --- | --- | --- | --- |
| access-token | `String` | Access Token | `accessToken` | `getAccessToken()` |



**Note:** Auth credentials can be set using `accessTokenCredentials` in the client builder and accessed through `getAccessTokenCredentials` method in the client instance.

## Usage Example

### Client Initialization

You must provide credentials in the client as shown in the following code snippet.

```java
import tech.fortis.sandbox.api.FortisAPIClient;
import tech.fortis.sandbox.api.authentication.AccessTokenModel;

public class Program {
    public static void main(String[] args) {
        FortisAPIClient client = new FortisAPIClient.Builder()
            .accessTokenCredentials(new AccessTokenModel.Builder(
                    "access-token"
                )
                .build())
            .build();
    }
}
```


