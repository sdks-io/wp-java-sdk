# Settlement Errors

```java
SettlementErrorsApi settlementErrorsApi = client.getSettlementErrorsApi();
```

## Class Name

`SettlementErrorsApi`

## Methods

* [Search Settlement Rejects](../../doc/controllers/settlement-errors.md#search-settlement-rejects)
* [Search Bank Card Rejects](../../doc/controllers/settlement-errors.md#search-bank-card-rejects)


# Search Settlement Rejects

Search settlement rejections.

```java
CompletableFuture<ApiResponse<SettlementerrorsSettlementfileerrorsSearchResponse>> searchSettlementRejectsAsync(
    final SettlementerrorsSettlementfileerrorsSearchRequest body,
    final UUID vCorrelationId)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`SettlementerrorsSettlementfileerrorsSearchRequest`](../../doc/models/settlementerrors-settlementfileerrors-search-request.md) | Body, Required | - |
| `vCorrelationId` | `UUID` | Header, Optional | Correlation Id |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`SettlementerrorsSettlementfileerrorsSearchResponse`](../../doc/models/settlementerrors-settlementfileerrors-search-response.md).

## Example Usage

```java
SettlementerrorsSettlementfileerrorsSearchRequest body = new SettlementerrorsSettlementfileerrorsSearchRequest.Builder(
    new Hierarchy6.Builder()
        .level(Level3.CHAIN)
        .values(Arrays.asList(
            "TSTC09"
        ))
        .build(),
    new DateRange1.Builder()
        .fromDate(DateTimeHelper.fromSimpleDate("2025-10-22"))
        .toDate(DateTimeHelper.fromSimpleDate("2025-10-22"))
        .build()
)
.build();


settlementErrorsApi.searchSettlementRejectsAsync(body, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof SettlementerrorsSettlementfileerrorsSearch0ErrorException) {
        SettlementerrorsSettlementfileerrorsSearch0ErrorException settlementerrorsSettlementfileerrorsSearch0ErrorException = (SettlementerrorsSettlementfileerrorsSearch0ErrorException) cause;
        settlementerrorsSettlementfileerrorsSearch0ErrorException.printStackTrace();
    } else {
        // fallback for unexpected errors
        exception.printStackTrace();
    }

    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| Default | Default errors | [`SettlementerrorsSettlementfileerrorsSearch0ErrorException`](../../doc/models/settlementerrors-settlementfileerrors-search-0-error-exception.md) |


# Search Bank Card Rejects

Search bank card rejections.

```java
CompletableFuture<ApiResponse<SettlementerrorsPendingsettlementbatchesSearchResponse>> searchBankCardRejectsAsync(
    final SettlementerrorsPendingsettlementbatchesSearchRequest body,
    final UUID vCorrelationId)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`SettlementerrorsPendingsettlementbatchesSearchRequest`](../../doc/models/settlementerrors-pendingsettlementbatches-search-request.md) | Body, Required | - |
| `vCorrelationId` | `UUID` | Header, Optional | Correlation Id |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`SettlementerrorsPendingsettlementbatchesSearchResponse`](../../doc/models/settlementerrors-pendingsettlementbatches-search-response.md).

## Example Usage

```java
SettlementerrorsPendingsettlementbatchesSearchRequest body = new SettlementerrorsPendingsettlementbatchesSearchRequest.Builder(
    new Hierarchy6.Builder()
        .level(Level3.CHAIN)
        .values(Arrays.asList(
            "TSTC09"
        ))
        .build(),
    new DateRange1.Builder()
        .fromDate(DateTimeHelper.fromSimpleDate("2025-04-09"))
        .toDate(DateTimeHelper.fromSimpleDate("2025-04-09"))
        .build()
)
.build();


settlementErrorsApi.searchBankCardRejectsAsync(body, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof SettlementerrorsPendingsettlementbatchesSearch0ErrorException) {
        SettlementerrorsPendingsettlementbatchesSearch0ErrorException settlementerrorsPendingsettlementbatchesSearch0ErrorException = (SettlementerrorsPendingsettlementbatchesSearch0ErrorException) cause;
        settlementerrorsPendingsettlementbatchesSearch0ErrorException.printStackTrace();
    } else {
        // fallback for unexpected errors
        exception.printStackTrace();
    }

    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| Default | Default errors | [`SettlementerrorsPendingsettlementbatchesSearch0ErrorException`](../../doc/models/settlementerrors-pendingsettlementbatches-search-0-error-exception.md) |

