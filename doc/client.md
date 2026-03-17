
# Client Class Documentation

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| httpClientConfig | [`Consumer<HttpClientConfiguration.Builder>`](../doc/http-client-configuration-builder.md) | Set up Http Client Configuration instance. |
| loggingConfig | [`Consumer<ApiLoggingConfiguration.Builder>`](../doc/api-logging-configuration-builder.md) | Set up Logging Configuration instance. |
| customHeaderAuthenticationCredentials | [`CustomHeaderAuthenticationCredentials`](auth/custom-header-signature.md) | The Credentials Setter for Custom Header Signature |

The API client can be initialized as follows:

```java
import com.worldpay.cert.apis.ReportingSettlementResearchApiClient;
import com.worldpay.cert.apis.authentication.CustomHeaderAuthenticationModel;
import com.worldpay.cert.apis.exceptions.ApiException;
import com.worldpay.cert.apis.http.response.ApiResponse;
import org.slf4j.event.Level;

public class Program {
    public static void main(String[] args) {
        ReportingSettlementResearchApiClient client = new ReportingSettlementResearchApiClient.Builder()
            .loggingConfig(builder -> builder
                    .level(Level.DEBUG)
                    .requestConfig(logConfigBuilder -> logConfigBuilder.body(true))
                    .responseConfig(logConfigBuilder -> logConfigBuilder.headers(true)))
            .httpClientConfig(configBuilder -> configBuilder
                    .timeout(0))
            .customHeaderAuthenticationCredentials(new CustomHeaderAuthenticationModel.Builder(
                    "Authorization"
                )
                .build())
            .build();

    }
}
```

## Reporting: Settlement Research APIClient Class

The gateway for the SDK. This class acts as a factory for the Apis and also holds the configuration of the SDK.

### Apis

| Name | Description | Return Type |
|  --- | --- | --- |
| `getSettlementsApi()` | Provides access to Settlements controller. | `SettlementsApi` |
| `getSettlementErrorsApi()` | Provides access to SettlementErrors controller. | `SettlementErrorsApi` |
| `getSettlementDailyTotalsApi()` | Provides access to SettlementDailyTotals controller. | `SettlementDailyTotalsApi` |
| `getSettlementBatchesApi()` | Provides access to SettlementBatches controller. | `SettlementBatchesApi` |
| `getTransactionTypeApi()` | Provides access to TransactionType controller. | `TransactionTypeApi` |
| `getTransactionStatusApi()` | Provides access to TransactionStatus controller. | `TransactionStatusApi` |

### Methods

| Name | Description | Return Type |
|  --- | --- | --- |
| `shutdown()` | Shutdown the underlying HttpClient instance. | `void` |
| `getEnvironment()` | Current API environment. | `Environment` |
| `getHttpClient()` | The HTTP Client instance to use for making HTTP requests. | `HttpClient` |
| `getHttpClientConfig()` | Http Client Configuration instance. | [`ReadonlyHttpClientConfiguration`](../doc/http-client-configuration.md) |
| `getLoggingConfig()` | Logging Configuration instance. | [`ReadonlyLoggingConfiguration`](../doc/api-logging-configuration.md) |
| `getCustomHeaderAuthenticationCredentials()` | The credentials to use with CustomHeaderAuthentication. | [`CustomHeaderAuthenticationCredentials`](auth/custom-header-signature.md) |
| `getBaseUri(Server server)` | Get base URI by current environment | `String` |
| `getBaseUri()` | Get base URI by current environment | `String` |

