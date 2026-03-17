# Transaction Status

```java
TransactionStatusApi transactionStatusApi = client.getTransactionStatusApi();
```

## Class Name

`TransactionStatusApi`


# Get Transaction Status

Indicates the current state of a financial transaction, whether it's pending, completed, failed, or under review.

```java
CompletableFuture<ApiResponse<List<TransactionStatusCode>>> getTransactionStatusAsync(
    final UUID vCorrelationId)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vCorrelationId` | `UUID` | Header, Optional | Correlation Id |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`List<TransactionStatusCode>`](../../doc/models/transaction-status-code.md).

## Example Usage

```java
UUID vCorrelationId = UUID.fromString("24578e35-9bd2-238f-b4c2-0bc9ad9aed2b");

transactionStatusApi.getTransactionStatusAsync(vCorrelationId).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof TransactionStatuses0ErrorException) {
        TransactionStatuses0ErrorException transactionStatuses0ErrorException = (TransactionStatuses0ErrorException) cause;
        transactionStatuses0ErrorException.printStackTrace();
    } else {
        // fallback for unexpected errors
        exception.printStackTrace();
    }

    return null;
});
```

## Example Response *(as JSON)*

```json
[
  {
    "code": "AA",
    "shortDescription": "APPROVAL",
    "longDescription": "APPROVAL"
  },
  {
    "code": "AB",
    "shortDescription": "APPRVL FOR LESS",
    "longDescription": "APPROVAL FOR LESSER AMOUNT (GIFT CARD)"
  },
  {
    "code": "014",
    "shortDescription": "NO FROM ACCT",
    "longDescription": "NO FROM ACCT"
  }
]
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| Default | Default errors | [`TransactionStatuses0ErrorException`](../../doc/models/transaction-statuses-0-error-exception.md) |

