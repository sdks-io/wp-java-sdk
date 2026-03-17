# Transaction Type

```java
TransactionTypeApi transactionTypeApi = client.getTransactionTypeApi();
```

## Class Name

`TransactionTypeApi`


# Get Transaction Type

The specific nature or purpose of a financial activity, such as purchases, withdrawals, or transfers.

```java
CompletableFuture<ApiResponse<List<TransactionTypeCode>>> getTransactionTypeAsync(
    final UUID vCorrelationId)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vCorrelationId` | `UUID` | Header, Optional | Correlation Id |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`List<TransactionTypeCode>`](../../doc/models/transaction-type-code.md).

## Example Usage

```java
UUID vCorrelationId = UUID.fromString("24578e35-9bd2-238f-b4c2-0bc9ad9aed2b");

transactionTypeApi.getTransactionTypeAsync(vCorrelationId).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof TransactionTypes0ErrorException) {
        TransactionTypes0ErrorException transactionTypes0ErrorException = (TransactionTypes0ErrorException) cause;
        transactionTypes0ErrorException.printStackTrace();
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
    "code": "GAX",
    "shortDescription": "Actvn Revsl    ",
    "longDescription": "Activation Reversal"
  },
  {
    "code": "253",
    "shortDescription": "SALE",
    "longDescription": "SALE"
  },
  {
    "code": "49",
    "shortDescription": "INTERBANK CR",
    "longDescription": "INTERBANK TRANSFER CREDIT"
  }
]
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| Default | Default errors | [`TransactionTypes0ErrorException`](../../doc/models/transaction-types-0-error-exception.md) |

