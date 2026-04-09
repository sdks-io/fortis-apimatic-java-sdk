
# Custom Header Signature



Documentation for accessing and setting credentials for developer-id.

## Auth Credentials

| Name | Type | Description | Setter | Getter |
|  --- | --- | --- | --- | --- |
| developer-id | `String` | Developer ID | `developerId` | `getDeveloperId()` |



**Note:** Auth credentials can be set using `developerIdCredentials` in the client builder and accessed through `getDeveloperIdCredentials` method in the client instance.

## Usage Example

### Client Initialization

You must provide credentials in the client as shown in the following code snippet.

```java
import tech.fortis.sandbox.api.FortisAPIClient;
import tech.fortis.sandbox.api.authentication.DeveloperIdModel;

public class Program {
    public static void main(String[] args) {
        FortisAPIClient client = new FortisAPIClient.Builder()
            .developerIdCredentials(new DeveloperIdModel.Builder(
                    "developer-id"
                )
                .build())
            .build();
    }
}
```


