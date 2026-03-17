
# Settlement Rejects Search Response

Response used for pagination.

*This model accepts additional fields of type Object.*

## Structure

`SettlementRejectsSearchResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Pagination` | [`Pagination4`](../../doc/models/pagination-4.md) | Optional | - | Pagination4 getPagination() | setPagination(Pagination4 pagination) |
| `Details` | [`List<SettlementRejRealTimeTransaction>`](../../doc/models/settlement-rej-real-time-transaction.md) | Optional | The settlement rejection details.<br><br>**Constraints**: *Minimum Items*: `1`, *Maximum Items*: `1` | List<SettlementRejRealTimeTransaction> getDetails() | setDetails(List<SettlementRejRealTimeTransaction> details) |
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
      "processedDate": "2016-03-13",
      "transactionDate": "2016-03-13",
      "resubmitDate": "2016-03-13",
      "accountNumber": "accountNumber8",
      "ddaNumber": "ddaNumber8",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "processedDate": "2016-03-13",
      "transactionDate": "2016-03-13",
      "resubmitDate": "2016-03-13",
      "accountNumber": "accountNumber8",
      "ddaNumber": "ddaNumber8",
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

