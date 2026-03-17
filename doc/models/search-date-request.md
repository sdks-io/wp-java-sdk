
# Search Date Request

*This model accepts additional fields of type Object.*

## Structure

`SearchDateRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Pagination` | [`Pagination`](../../doc/models/pagination.md) | Optional | - | Pagination getPagination() | setPagination(Pagination pagination) |
| `Hierarchy` | [`Hierarchy2`](../../doc/models/hierarchy-2.md) | Required | - | Hierarchy2 getHierarchy() | setHierarchy(Hierarchy2 hierarchy) |
| `DateRange` | [`DateRange1`](../../doc/models/date-range-1.md) | Required | - | DateRange1 getDateRange() | setDateRange(DateRange1 dateRange) |
| `BatchCardType` | [`BatchCardType1`](../../doc/models/batch-card-type-1.md) | Optional | - | BatchCardType1 getBatchCardType() | setBatchCardType(BatchCardType1 batchCardType) |
| `SortResultsBy` | [`SortResultsBy3`](../../doc/models/sort-results-by-3.md) | Optional | - | SortResultsBy3 getSortResultsBy() | setSortResultsBy(SortResultsBy3 sortResultsBy) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "hierarchy": {
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
  "pagination": {
    "pageNumber": 16776215,
    "pageSize": 1000,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "batchCardType": "CREDIT",
  "sortResultsBy": {
    "fieldName": "PROCESS_DATE",
    "orderBy": "ASC",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

