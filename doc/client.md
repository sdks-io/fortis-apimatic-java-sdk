
# Client Class Documentation

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| environment | [`Environment`](../README.md#environments) | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| httpClientConfig | [`Consumer<HttpClientConfiguration.Builder>`](../doc/http-client-configuration-builder.md) | Set up Http Client Configuration instance. |
| loggingConfig | [`Consumer<ApiLoggingConfiguration.Builder>`](../doc/api-logging-configuration-builder.md) | Set up Logging Configuration instance. |
| userIdCredentials | [`UserIdCredentials`](auth/custom-header-signature.md) | The Credentials Setter for Custom Header Signature |
| userApiKeyCredentials | [`UserApiKeyCredentials`](auth/custom-header-signature-1.md) | The Credentials Setter for Custom Header Signature |
| developerIdCredentials | [`DeveloperIdCredentials`](auth/custom-header-signature-2.md) | The Credentials Setter for Custom Header Signature |
| accessTokenCredentials | [`AccessTokenCredentials`](auth/custom-header-signature-3.md) | The Credentials Setter for Custom Header Signature |

The API client can be initialized as follows:

```java
import org.slf4j.event.Level;
import tech.fortis.sandbox.api.Environment;
import tech.fortis.sandbox.api.FortisApiClient;
import tech.fortis.sandbox.api.authentication.AccessTokenModel;
import tech.fortis.sandbox.api.authentication.DeveloperIdModel;
import tech.fortis.sandbox.api.authentication.UserApiKeyModel;
import tech.fortis.sandbox.api.authentication.UserIdModel;
import tech.fortis.sandbox.api.exceptions.ApiException;
import tech.fortis.sandbox.api.http.response.ApiResponse;

public class Program {
    public static void main(String[] args) {
        FortisApiClient client = new FortisApiClient.Builder()
            .loggingConfig(builder -> builder
                    .level(Level.DEBUG)
                    .requestConfig(logConfigBuilder -> logConfigBuilder.body(true))
                    .responseConfig(logConfigBuilder -> logConfigBuilder.headers(true)))
            .httpClientConfig(configBuilder -> configBuilder
                    .timeout(0))
            .userIdCredentials(new UserIdModel.Builder(
                    "user-id"
                )
                .build())
            .userApiKeyCredentials(new UserApiKeyModel.Builder(
                    "user-api-key"
                )
                .build())
            .developerIdCredentials(new DeveloperIdModel.Builder(
                    "developer-id"
                )
                .build())
            .accessTokenCredentials(new AccessTokenModel.Builder(
                    "access-token"
                )
                .build())
            .environment(Environment.PRODUCTION)
            .build();

    }
}
```

## Fortis APIClient Class

The gateway for the SDK. This class acts as a factory for the Controllers and also holds the configuration of the SDK.

### Controllers

| Name | Description | Return Type |
|  --- | --- | --- |
| `getAsyncProcessingController()` | Provides access to AsyncProcessing controller. | `AsyncProcessingController` |
| `getBatchesController()` | Provides access to Batches controller. | `BatchesController` |
| `getContactsController()` | Provides access to Contacts controller. | `ContactsController` |
| `getDeclinedRecurringTransactionsController()` | Provides access to DeclinedRecurringTransactions controller. | `DeclinedRecurringTransactionsController` |
| `getDeviceTermsController()` | Provides access to DeviceTerms controller. | `DeviceTermsController` |
| `getElementsController()` | Provides access to Elements controller. | `ElementsController` |
| `getFullBoardingController()` | Provides access to FullBoarding controller. | `FullBoardingController` |
| `getLocationsController()` | Provides access to Locations controller. | `LocationsController` |
| `getM3DsAuthenticationController()` | Provides access to M3DsAuthentication controller. | `M3DsAuthenticationController` |
| `getM3DsTransactionsController()` | Provides access to M3DsTransactions controller. | `M3DsTransactionsController` |
| `getMerchantDepositsController()` | Provides access to MerchantDeposits controller. | `MerchantDepositsController` |
| `getOnBoardingController()` | Provides access to OnBoarding controller. | `OnBoardingController` |
| `getPaylinksController()` | Provides access to Paylinks controller. | `PaylinksController` |
| `getPaymentCardReaderTokenController()` | Provides access to PaymentCardReaderToken controller. | `PaymentCardReaderTokenController` |
| `getQuickInvoicesController()` | Provides access to QuickInvoices controller. | `QuickInvoicesController` |
| `getRecurringController()` | Provides access to Recurring controller. | `RecurringController` |
| `getSignaturesController()` | Provides access to Signatures controller. | `SignaturesController` |
| `getTagsController()` | Provides access to Tags controller. | `TagsController` |
| `getTerminalsController()` | Provides access to Terminals controller. | `TerminalsController` |
| `getTicketsController()` | Provides access to Tickets controller. | `TicketsController` |
| `getTokensController()` | Provides access to Tokens controller. | `TokensController` |
| `getTransactionAchRetriesController()` | Provides access to TransactionAchRetries controller. | `TransactionAchRetriesController` |
| `getTransactionsAchController()` | Provides access to TransactionsAch controller. | `TransactionsAchController` |
| `getTransactionsCashController()` | Provides access to TransactionsCash controller. | `TransactionsCashController` |
| `getTransactionsCreditCardController()` | Provides access to TransactionsCreditCard controller. | `TransactionsCreditCardController` |
| `getTransactionsEbtCardController()` | Provides access to TransactionsEbtCard controller. | `TransactionsEbtCardController` |
| `getTransactionsReadController()` | Provides access to TransactionsRead controller. | `TransactionsReadController` |
| `getLevel3DataController()` | Provides access to Level3Data controller. | `Level3DataController` |
| `getTransactionsUpdatesController()` | Provides access to TransactionsUpdates controller. | `TransactionsUpdatesController` |
| `getUserVerificationsController()` | Provides access to UserVerifications controller. | `UserVerificationsController` |
| `getUsersController()` | Provides access to Users controller. | `UsersController` |
| `getApplePayValidateMerchantController()` | Provides access to ApplePayValidateMerchant controller. | `ApplePayValidateMerchantController` |
| `getMerchantDetailsController()` | Provides access to MerchantDetails controller. | `MerchantDetailsController` |
| `getWebhooksController()` | Provides access to Webhooks controller. | `WebhooksController` |

### Methods

| Name | Description | Return Type |
|  --- | --- | --- |
| `shutdown()` | Shutdown the underlying HttpClient instance. | `void` |
| `getEnvironment()` | Current API environment. | `Environment` |
| `getHttpClient()` | The HTTP Client instance to use for making HTTP requests. | `HttpClient` |
| `getHttpClientConfig()` | Http Client Configuration instance. | [`ReadonlyHttpClientConfiguration`](../doc/http-client-configuration.md) |
| `getLoggingConfig()` | Logging Configuration instance. | [`ReadonlyLoggingConfiguration`](../doc/api-logging-configuration.md) |
| `getUserIdCredentials()` | The credentials to use with UserId. | [`UserIdCredentials`](auth/custom-header-signature.md) |
| `getUserApiKeyCredentials()` | The credentials to use with UserApiKey. | [`UserApiKeyCredentials`](auth/custom-header-signature-1.md) |
| `getDeveloperIdCredentials()` | The credentials to use with DeveloperId. | [`DeveloperIdCredentials`](auth/custom-header-signature-2.md) |
| `getAccessTokenCredentials()` | The credentials to use with AccessToken. | [`AccessTokenCredentials`](auth/custom-header-signature-3.md) |
| `getBaseUri(Server server)` | Get base URI by current environment | `String` |
| `getBaseUri()` | Get base URI by current environment | `String` |

