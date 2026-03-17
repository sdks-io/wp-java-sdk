
# Settlement Rejects Search Request

Request fields for settlement rejections.

*This model accepts additional fields of type Object.*

## Structure

`SettlementRejectsSearchRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Pagination` | [`Pagination`](../../doc/models/pagination.md) | Optional | - | Pagination getPagination() | setPagination(Pagination pagination) |
| `Hierarchy` | [`Hierarchy6`](../../doc/models/hierarchy-6.md) | Required | - | Hierarchy6 getHierarchy() | setHierarchy(Hierarchy6 hierarchy) |
| `SortResultsBy` | [`SortResultsBy4`](../../doc/models/sort-results-by-4.md) | Optional | - | SortResultsBy4 getSortResultsBy() | setSortResultsBy(SortResultsBy4 sortResultsBy) |
| `DateRange` | [`DateRange1`](../../doc/models/date-range-1.md) | Required | - | DateRange1 getDateRange() | setDateRange(DateRange1 dateRange) |
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
  "pagination": {
    "pageNumber": 16776215,
    "pageSize": 1000,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "sortResultsBy": {
    "fieldName": "RESUBMIT_DATE",
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

