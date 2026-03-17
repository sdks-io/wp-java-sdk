
# Custom Header Signature



Documentation for accessing and setting credentials for api_key.

## Auth Credentials

| Name | Type | Description | Setter | Getter |
|  --- | --- | --- | --- | --- |
| Authorization | `String` | ` License format is WORLDPAY license='xxxx'` | `authorization` | `getAuthorization()` |



**Note:** Auth credentials can be set using `customHeaderAuthenticationCredentials` in the client builder and accessed through `getCustomHeaderAuthenticationCredentials` method in the client instance.

## Usage Example

### Client Initialization

You must provide credentials in the client as shown in the following code snippet.

```java
import com.worldpay.cert.apis.ReportingSettlementResearchApiClient;
import com.worldpay.cert.apis.authentication.CustomHeaderAuthenticationModel;

public class Program {
    public static void main(String[] args) {
        ReportingSettlementResearchApiClient client = new ReportingSettlementResearchApiClient.Builder()
            .customHeaderAuthenticationCredentials(new CustomHeaderAuthenticationModel.Builder(
                    "Authorization"
                )
                .build())
            .build();
    }
}
```


