# Settlement Batches

```java
SettlementBatchesApi settlementBatchesApi = client.getSettlementBatchesApi();
```

## Class Name

`SettlementBatchesApi`

## Methods

* [Search Settlement Batches Store](../../doc/controllers/settlement-batches.md#search-settlement-batches-store)
* [Search Settlement Batches Date](../../doc/controllers/settlement-batches.md#search-settlement-batches-date)


# Search Settlement Batches Store

Search settlement batches grouped by store.

```java
CompletableFuture<ApiResponse<SearchStoreResponse>> searchSettlementBatchesStoreAsync(
    final SearchStoreRequest body,
    final UUID vCorrelationId)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`SearchStoreRequest`](../../doc/models/search-store-request.md) | Body, Required | - |
| `vCorrelationId` | `UUID` | Header, Optional | Correlation Id |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`SearchStoreResponse`](../../doc/models/search-store-response.md).

## Example Usage

```java
SearchStoreRequest body = new SearchStoreRequest.Builder(
    new Hierarchy2.Builder()
        .level(Level2.CHAIN)
        .values(Arrays.asList(
            "TSTC09"
        ))
        .build(),
    new DateRange1.Builder()
        .fromDate(DateTimeHelper.fromSimpleDate("2025-10-06"))
        .toDate(DateTimeHelper.fromSimpleDate("2025-10-06"))
        .build()
)
.additionalProperty("dateType", ApiHelper.deserialize("\"PROCESS_DATE\""))
.build();


settlementBatchesApi.searchSettlementBatchesStoreAsync(body, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof SearchStore0ErrorException) {
        SearchStore0ErrorException searchStore0ErrorException = (SearchStore0ErrorException) cause;
        searchStore0ErrorException.printStackTrace();
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
| Default | Default errors | [`SearchStore0ErrorException`](../../doc/models/search-store-0-error-exception.md) |


# Search Settlement Batches Date

Search settlement batches grouped by date.

```java
CompletableFuture<ApiResponse<SearchDateResponse>> searchSettlementBatchesDateAsync(
    final SearchDateRequest body,
    final UUID vCorrelationId)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`SearchDateRequest`](../../doc/models/search-date-request.md) | Body, Required | - |
| `vCorrelationId` | `UUID` | Header, Optional | Correlation Id |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`SearchDateResponse`](../../doc/models/search-date-response.md).

## Example Usage

```java
SearchDateRequest body = new SearchDateRequest.Builder(
    new Hierarchy2.Builder()
        .level(Level2.CHAIN)
        .values(Arrays.asList(
            "TSTC09"
        ))
        .build(),
    new DateRange1.Builder()
        .fromDate(DateTimeHelper.fromSimpleDate("2025-10-06"))
        .toDate(DateTimeHelper.fromSimpleDate("2025-10-06"))
        .build()
)
.additionalProperty("dateType", ApiHelper.deserialize("\"PROCESS_DATE\""))
.build();


settlementBatchesApi.searchSettlementBatchesDateAsync(body, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof SearchDate0ErrorException) {
        SearchDate0ErrorException searchDate0ErrorException = (SearchDate0ErrorException) cause;
        searchDate0ErrorException.printStackTrace();
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
| Default | Default errors | [`SearchDate0ErrorException`](../../doc/models/search-date-0-error-exception.md) |

