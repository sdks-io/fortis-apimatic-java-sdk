
# Getting Started with Fortis API

## Install the Package

Install the SDK by adding the following dependency in your project's pom.xml file:

```xml
<dependency>
  <groupId>io.sdks</groupId>
  <artifactId>fortis-apimatic-sdk</artifactId>
  <version>1.0.5</version>
</dependency>
```

You can also view the package at:
https://central.sonatype.com/artifact/io.sdks/fortis-apimatic-sdk/1.0.5

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| environment | [`Environment`](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/README.md#environments) | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| httpClientConfig | [`Consumer<HttpClientConfiguration.Builder>`](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/http-client-configuration-builder.md) | Set up Http Client Configuration instance. |
| loggingConfig | [`Consumer<ApiLoggingConfiguration.Builder>`](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/api-logging-configuration-builder.md) | Set up Logging Configuration instance. |
| userIdCredentials | [`UserIdCredentials`](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/auth/custom-header-signature.md) | The Credentials Setter for Custom Header Signature |
| userApiKeyCredentials | [`UserApiKeyCredentials`](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/auth/custom-header-signature-1.md) | The Credentials Setter for Custom Header Signature |
| developerIdCredentials | [`DeveloperIdCredentials`](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/auth/custom-header-signature-2.md) | The Credentials Setter for Custom Header Signature |
| accessTokenCredentials | [`AccessTokenCredentials`](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/auth/custom-header-signature-3.md) | The Credentials Setter for Custom Header Signature |

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

## Environments

The SDK can be configured to use a different environment for making API calls. Available environments are:

### Fields

| Name | Description |
|  --- | --- |
| PRODUCTION | **Default** |
| ENVIRONMENT2 | - |

## Authorization

This API uses the following authentication schemes.

* [`user-id (Custom Header Signature)`](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/auth/custom-header-signature.md)
* [`user-api-key (Custom Header Signature)`](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/auth/custom-header-signature-1.md)
* [`developer-id (Custom Header Signature)`](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/auth/custom-header-signature-2.md)
* [`access-token (Custom Header Signature)`](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/auth/custom-header-signature-3.md)

## List of APIs

* [Async Processing](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/async-processing.md)
* [Declined Recurring Transactions](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/declined-recurring-transactions.md)
* [Device Terms](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/device-terms.md)
* [Full Boarding](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/full-boarding.md)
* [3 DS Authentication](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/3-ds-authentication.md)
* [3 DS Transactions](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/3-ds-transactions.md)
* [Merchant Deposits](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/merchant-deposits.md)
* [On Boarding](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/on-boarding.md)
* [Payment Card Reader Token](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/payment-card-reader-token.md)
* [Quick Invoices](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/quick-invoices.md)
* [Transaction ACH Retries](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/transaction-ach-retries.md)
* [Transactions-ACH](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/transactions-ach.md)
* [Transactions-Cash](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/transactions-cash.md)
* [Transactions-Credit Card](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/transactions-credit-card.md)
* [Transactions-EBT Card](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/transactions-ebt-card.md)
* [Transactions-Read](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/transactions-read.md)
* [Level 3 Data](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/level-3-data.md)
* [Transactions-Updates](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/transactions-updates.md)
* [User Verifications](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/user-verifications.md)
* [Apple Pay Validate Merchant](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/apple-pay-validate-merchant.md)
* [Merchant Details](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/merchant-details.md)
* [Batches](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/batches.md)
* [Contacts](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/contacts.md)
* [Elements](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/elements.md)
* [Locations](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/locations.md)
* [Paylinks](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/paylinks.md)
* [Recurring](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/recurring.md)
* [Signatures](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/signatures.md)
* [Tags](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/tags.md)
* [Terminals](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/terminals.md)
* [Tickets](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/tickets.md)
* [Tokens](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/tokens.md)
* [Users](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/users.md)
* [Webhooks](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/controllers/webhooks.md)

## SDK Infrastructure

### Configuration

* [ApiLoggingConfiguration](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/api-logging-configuration.md)
* [ApiLoggingConfiguration.Builder](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/api-logging-configuration-builder.md)
* [ApiRequestLoggingConfiguration.Builder](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/api-request-logging-configuration-builder.md)
* [ApiResponseLoggingConfiguration.Builder](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/api-response-logging-configuration-builder.md)
* [Configuration Interface](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/configuration-interface.md)
* [HttpClientConfiguration](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/http-client-configuration.md)
* [HttpClientConfiguration.Builder](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/http-client-configuration-builder.md)
* [HttpProxyConfiguration](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/http-proxy-configuration.md)
* [HttpProxyConfiguration.Builder](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/http-proxy-configuration-builder.md)

### HTTP

* [Headers](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/headers.md)
* [HttpCallback Interface](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/http-callback-interface.md)
* [HttpContext](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/http-context.md)
* [HttpBodyRequest](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/http-body-request.md)
* [HttpRequest](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/http-request.md)
* [HttpResponse](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/http-response.md)
* [HttpStringResponse](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/http-string-response.md)

### Utilities

* [ApiException](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/api-exception.md)
* [ApiResponse](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/api-response.md)
* [ApiHelper](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/api-helper.md)
* [FileWrapper](https://www.github.com/sdks-io/fortis-apimatic-java-sdk/tree/1.0.5/doc/file-wrapper.md)

