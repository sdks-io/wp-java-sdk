# Settlements

Endpoint to retrieve the settled transaction details for a given hierarchy and date range with a 45-day limit and unrestricted lookup period. Optional fields help refine the search.

```java
SettlementsApi settlementsApi = client.getSettlementsApi();
```

## Class Name

`SettlementsApi`


# Search Settlements

Endpoint to retrieve the settled transaction details for a given hierarchy and date range, with a 45-day limit and unrestricted lookup period. Optional fields help refine the search.

```java
CompletableFuture<ApiResponse<SettlementsSearchResponse>> searchSettlementsAsync(
    final SettlementsSearchRequest body,
    final UUID vCorrelationId)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`SettlementsSearchRequest`](../../doc/models/settlements-search-request.md) | Body, Required | - |
| `vCorrelationId` | `UUID` | Header, Optional | Correlation Id |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`SettlementsSearchResponse`](../../doc/models/settlements-search-response.md).

## Example Usage

```java
SettlementsSearchRequest body = new SettlementsSearchRequest.Builder(
    new Hierarchy.Builder()
        .level(Level.CHAIN)
        .values(Arrays.asList(
            "TSTC04",
            "TSTC05",
            "TSTC06",
            "TSTC07",
            "TSTC08",
            "TSTC09"
        ))
        .build(),
    new DateRange1.Builder()
        .fromDate(DateTimeHelper.fromSimpleDate("2024-03-10"))
        .toDate(DateTimeHelper.fromSimpleDate("2024-04-09"))
        .build()
)
.build();


settlementsApi.searchSettlementsAsync(body, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof SettlementsSearch0ErrorException) {
        SettlementsSearch0ErrorException settlementsSearch0ErrorException = (SettlementsSearch0ErrorException) cause;
        settlementsSearch0ErrorException.printStackTrace();
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
| Default | Default errors | [`SettlementsSearch0ErrorException`](../../doc/models/settlements-search-0-error-exception.md) |

