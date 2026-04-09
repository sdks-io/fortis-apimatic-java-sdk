
# Custom Header Signature



Documentation for accessing and setting credentials for user-id.

## Auth Credentials

| Name | Type | Description | Setter | Getter |
|  --- | --- | --- | --- | --- |
| user-id | `String` | User ID | `userId` | `getUserId()` |



**Note:** Auth credentials can be set using `userIdCredentials` in the client builder and accessed through `getUserIdCredentials` method in the client instance.

## Usage Example

### Client Initialization

You must provide credentials in the client as shown in the following code snippet.

```java
import tech.fortis.sandbox.api.FortisAPIClient;
import tech.fortis.sandbox.api.authentication.UserIdModel;

public class Program {
    public static void main(String[] args) {
        FortisAPIClient client = new FortisAPIClient.Builder()
            .userIdCredentials(new UserIdModel.Builder(
                    "user-id"
                )
                .build())
            .build();
    }
}
```


