# Settlement Daily Totals

```java
SettlementDailyTotalsApi settlementDailyTotalsApi = client.getSettlementDailyTotalsApi();
```

## Class Name

`SettlementDailyTotalsApi`


# Search Settlements Daily Totals

Retrieve the settled transactions daily financial activity for a given hierarchy and date range. Optional fields help refine the search.

```java
CompletableFuture<ApiResponse<SettlementsDailyTotalsSearchResponse>> searchSettlementsDailyTotalsAsync(
    final SettlementsDailyTotalsSearchRequest body,
    final UUID vCorrelationId)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`SettlementsDailyTotalsSearchRequest`](../../doc/models/settlements-daily-totals-search-request.md) | Body, Required | - |
| `vCorrelationId` | `UUID` | Header, Optional | Correlation Id |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`SettlementsDailyTotalsSearchResponse`](../../doc/models/settlements-daily-totals-search-response.md).

## Example Usage

```java
SettlementsDailyTotalsSearchRequest body = new SettlementsDailyTotalsSearchRequest.Builder(
    new Hierarchy1.Builder()
        .level(Level1.CHAIN)
        .values(Arrays.asList(
            "TSTC09"
        ))
        .build(),
    DateType.PROCESS_DATE,
    new DateRange1.Builder()
        .fromDate(DateTimeHelper.fromSimpleDate("2025-10-06"))
        .toDate(DateTimeHelper.fromSimpleDate("2025-10-06"))
        .build()
)
.build();


settlementDailyTotalsApi.searchSettlementsDailyTotalsAsync(body, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof SettlementsDailyTotalsSearch0ErrorException) {
        SettlementsDailyTotalsSearch0ErrorException settlementsDailyTotalsSearch0ErrorException = (SettlementsDailyTotalsSearch0ErrorException) cause;
        settlementsDailyTotalsSearch0ErrorException.printStackTrace();
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
| Default | Default errors | [`SettlementsDailyTotalsSearch0ErrorException`](../../doc/models/settlements-daily-totals-search-0-error-exception.md) |

