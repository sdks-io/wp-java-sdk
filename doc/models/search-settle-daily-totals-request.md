
# Search Settle Daily Totals Request

The request fields for search settle daily totals.

*This model accepts additional fields of type Object.*

## Structure

`SearchSettleDailyTotalsRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Pagination` | [`Pagination`](../../doc/models/pagination.md) | Optional | - | Pagination getPagination() | setPagination(Pagination pagination) |
| `SortResultsBy` | [`SortResultsBy1`](../../doc/models/sort-results-by-1.md) | Optional | - | SortResultsBy1 getSortResultsBy() | setSortResultsBy(SortResultsBy1 sortResultsBy) |
| `Hierarchy` | [`Hierarchy1`](../../doc/models/hierarchy-1.md) | Required | - | Hierarchy1 getHierarchy() | setHierarchy(Hierarchy1 hierarchy) |
| `DateType` | [`DateType`](../../doc/models/date-type.md) | Required | **Constraints**: *Maximum Length*: `16` | DateType getDateType() | setDateType(DateType dateType) |
| `DateRange` | [`DateRange1`](../../doc/models/date-range-1.md) | Required | - | DateRange1 getDateRange() | setDateRange(DateRange1 dateRange) |
| `CardTypes` | [`List<CardTypes1>`](../../doc/models/card-types-1.md) | Optional | The category or classification of a payment card based on the issuing network. Possible values are CREDIT, DEBIT, GIFT, and EBT. | List<CardTypes1> getCardTypes() | setCardTypes(List<CardTypes1> cardTypes) |
| `TerminalData` | `Boolean` | Optional | Display the terminal data. | Boolean getTerminalData() | setTerminalData(Boolean terminalData) |
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
  "dateType": "PROCESS_DATE",
  "dateRange": {
    "fromDate": "2021-12-01",
    "toDate": "2021-12-01",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "terminalData": true,
  "pagination": {
    "pageNumber": 16776215,
    "pageSize": 1000,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "sortResultsBy": {
    "fieldName": "MERCHANT_ID",
    "orderBy": "ASC",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "cardTypes": [
    "CREDIT"
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

