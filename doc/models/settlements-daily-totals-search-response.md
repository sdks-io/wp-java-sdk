
# Settlements Daily Totals Search Response

*This model accepts additional fields of type Object.*

## Structure

`SettlementsDailyTotalsSearchResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Pagination` | [`PaginationResponse`](../../doc/models/pagination-response.md) | Optional | The format used to display your resources. | PaginationResponse getPagination() | setPagination(PaginationResponse pagination) |
| `Details` | [`List<SearchDailyTotalsDetails>`](../../doc/models/search-daily-totals-details.md) | Optional | Retrieves the daily total information.<br><br>**Constraints**: *Minimum Items*: `1`, *Maximum Items*: `1` | List<SearchDailyTotalsDetails> getDetails() | setDetails(List<SearchDailyTotalsDetails> details) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "pagination": {
    "pageNumber": 16776215,
    "pageSize": 1000,
    "totalRowCount": 8999,
    "totalReturnedCount": 1000,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "details": [
    {
      "cardType": "cardType4",
      "batchNumber": 11,
      "processDate": "2016-03-13",
      "transactionDate": "2016-03-13",
      "hierarchy": {
        "chainCode": "chainCode0",
        "divisionNumber": "divisionNumber4",
        "storeNumber": "storeNumber2",
        "merchantId": "merchantId0",
        "alternateMerchantId": "alternateMerchantId0",
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
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

