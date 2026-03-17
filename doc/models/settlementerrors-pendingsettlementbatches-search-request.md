
# Settlementerrors Pendingsettlementbatches Search Request

*This model accepts additional fields of type Object.*

## Structure

`SettlementerrorsPendingsettlementbatchesSearchRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Pagination` | [`Pagination`](../../doc/models/pagination.md) | Optional | - | Pagination getPagination() | setPagination(Pagination pagination) |
| `Hierarchy` | [`Hierarchy6`](../../doc/models/hierarchy-6.md) | Required | - | Hierarchy6 getHierarchy() | setHierarchy(Hierarchy6 hierarchy) |
| `SortResultsBy` | [`SortResultsBy5`](../../doc/models/sort-results-by-5.md) | Optional | - | SortResultsBy5 getSortResultsBy() | setSortResultsBy(SortResultsBy5 sortResultsBy) |
| `DateRange` | [`DateRange1`](../../doc/models/date-range-1.md) | Required | - | DateRange1 getDateRange() | setDateRange(DateRange1 dateRange) |
| `BatchNumber` | `Integer` | Optional | The 11-byte unique identifier assigned to a group of transactions that were handled together as a single unit.<br><br>**Constraints**: `<= 11` | Integer getBatchNumber() | setBatchNumber(Integer batchNumber) |
| `BatchHoldStatus` | `String` | Optional | Indicates the batch hold status of the transaction.<br><br>**Constraints**: *Maximum Length*: `256` | String getBatchHoldStatus() | setBatchHoldStatus(String batchHoldStatus) |
| `BatchAmount` | `Double` | Optional | The total amount of all the transactions that are part of the batch file.<br><br>**Constraints**: `>= 0`, `<= 9999999999999.99` | Double getBatchAmount() | setBatchAmount(Double batchAmount) |
| `SaleAmount` | `Double` | Optional | The sale amount of the transaction.<br><br>**Constraints**: `>= 0`, `<= 9999999999999.99` | Double getSaleAmount() | setSaleAmount(Double saleAmount) |
| `ReturnAmount` | `Double` | Optional | The return amount of the transaction.<br><br>**Constraints**: `>= 0`, `<= 9999999999999.99` | Double getReturnAmount() | setReturnAmount(Double returnAmount) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "hierarchy": {
    "chainCode": "PA1234",
    "level": "MERCHANT",
    "values": [
      "values6",
      "values7"
    ],
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "dateRange": {
    "fromDate": "2021-12-01",
    "toDate": "2021-12-01",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "batchHoldStatus": "RELEASE BATCH",
  "batchAmount": 37551.09,
  "saleAmount": 36551.08,
  "returnAmount": 113.08,
  "pagination": {
    "pageNumber": 16776215,
    "pageSize": 1000,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "sortResultsBy": {
    "fieldName": "BATCH_NUMBER",
    "orderBy": "ASC",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "batchNumber": 11,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

