
# Custom Header Signature



Documentation for accessing and setting credentials for user-api-key.

## Auth Credentials

| Name | Type | Description | Setter | Getter |
|  --- | --- | --- | --- | --- |
| user-api-key | `String` | User API Key | `userApiKey` | `getUserApiKey()` |



**Note:** Auth credentials can be set using `userApiKeyCredentials` in the client builder and accessed through `getUserApiKeyCredentials` method in the client instance.

## Usage Example

### Client Initialization

You must provide credentials in the client as shown in the following code snippet.

```java
import tech.fortis.sandbox.api.FortisApiClient;
import tech.fortis.sandbox.api.authentication.UserApiKeyModel;

public class Program {
    public static void main(String[] args) {
        FortisApiClient client = new FortisApiClient.Builder()
            .userApiKeyCredentials(new UserApiKeyModel.Builder(
                    "user-api-key"
                )
                .build())
            .build();
    }
}
```


