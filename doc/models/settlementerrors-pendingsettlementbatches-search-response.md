
# Settlementerrors Pendingsettlementbatches Search Response

*This model accepts additional fields of type Object.*

## Structure

`SettlementerrorsPendingsettlementbatchesSearchResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Pagination` | [`Pagination4`](../../doc/models/pagination-4.md) | Optional | - | Pagination4 getPagination() | setPagination(Pagination4 pagination) |
| `Details` | [`List<BankCardRejRealTimeTransaction>`](../../doc/models/bank-card-rej-real-time-transaction.md) | Optional | Refers to bank card rejection details.<br><br>**Constraints**: *Minimum Items*: `1`, *Maximum Items*: `1` | List<BankCardRejRealTimeTransaction> getDetails() | setDetails(List<BankCardRejRealTimeTransaction> details) |
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
      "processDate": "2016-03-13",
      "batchNumber": 6,
      "batchAmount": 10.0,
      "saleCount": 9999998999,
      "saleAmount": 18.34,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "processDate": "2016-03-13",
      "batchNumber": 6,
      "batchAmount": 10.0,
      "saleCount": 9999998999,
      "saleAmount": 18.34,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "processDate": "2016-03-13",
      "batchNumber": 6,
      "batchAmount": 10.0,
      "saleCount": 9999998999,
      "saleAmount": 18.34,
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

