
# Getting Started with Reporting: Settlement Research API

## Introduction

API used to search and retrieve settled transactions. This API is used to search settled transactions and retrieve individual transaction details based on card types.

## Install the Package

Install the SDK by adding the following dependency in your project's pom.xml file:

```xml
<dependency>
  <groupId>io.sdks</groupId>
  <artifactId>wp-sdk</artifactId>
  <version>1.0.1</version>
</dependency>
```

You can also view the package at:
https://central.sonatype.com/artifact/io.sdks/wp-sdk/1.0.1

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| httpClientConfig | [`Consumer<HttpClientConfiguration.Builder>`](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/http-client-configuration-builder.md) | Set up Http Client Configuration instance. |
| loggingConfig | [`Consumer<ApiLoggingConfiguration.Builder>`](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/api-logging-configuration-builder.md) | Set up Logging Configuration instance. |
| customHeaderAuthenticationCredentials | [`CustomHeaderAuthenticationCredentials`](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/auth/custom-header-signature.md) | The Credentials Setter for Custom Header Signature |

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

## Authorization

This API uses the following authentication schemes.

* [`api_key (Custom Header Signature)`](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/auth/custom-header-signature.md)

## List of APIs

* [Settlement Errors](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/controllers/settlement-errors.md)
* [Settlement Daily Totals](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/controllers/settlement-daily-totals.md)
* [Settlement Batches](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/controllers/settlement-batches.md)
* [Transaction Type](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/controllers/transaction-type.md)
* [Transaction Status](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/controllers/transaction-status.md)
* [Settlements](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/controllers/settlements.md)

## SDK Infrastructure

### Configuration

* [ApiLoggingConfiguration](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/api-logging-configuration.md)
* [ApiLoggingConfiguration.Builder](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/api-logging-configuration-builder.md)
* [ApiRequestLoggingConfiguration.Builder](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/api-request-logging-configuration-builder.md)
* [ApiResponseLoggingConfiguration.Builder](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/api-response-logging-configuration-builder.md)
* [Configuration Interface](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/configuration-interface.md)
* [HttpClientConfiguration](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/http-client-configuration.md)
* [HttpClientConfiguration.Builder](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/http-client-configuration-builder.md)
* [HttpProxyConfiguration](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/http-proxy-configuration.md)
* [HttpProxyConfiguration.Builder](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/http-proxy-configuration-builder.md)

### HTTP

* [Headers](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/headers.md)
* [HttpCallback Interface](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/http-callback-interface.md)
* [HttpContext](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/http-context.md)
* [HttpBodyRequest](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/http-body-request.md)
* [HttpRequest](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/http-request.md)
* [HttpResponse](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/http-response.md)
* [HttpStringResponse](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/http-string-response.md)

### Utilities

* [ApiException](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/api-exception.md)
* [ApiResponse](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/api-response.md)
* [ApiHelper](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/api-helper.md)
* [FileWrapper](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/file-wrapper.md)
* [DateTimeHelper](https://www.github.com/sdks-io/wp-java-sdk/tree/1.0.1/doc/date-time-helper.md)

