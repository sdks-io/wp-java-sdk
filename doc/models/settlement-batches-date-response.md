
# Settlement Batches Date Response

The response of settlement batches date data.

*This model accepts additional fields of type Object.*

## Structure

`SettlementBatchesDateResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Pagination` | [`Pagination4`](../../doc/models/pagination-4.md) | Optional | - | Pagination4 getPagination() | setPagination(Pagination4 pagination) |
| `Details` | [`List<SettlementBatchesTransactionDate>`](../../doc/models/settlement-batches-transaction-date.md) | Optional | Refers to the settlement batches date details.<br><br>**Constraints**: *Minimum Items*: `1`, *Maximum Items*: `1` | List<SettlementBatchesTransactionDate> getDetails() | setDetails(List<SettlementBatchesTransactionDate> details) |
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
      "hierarchy": {
        "storeNumber": "storeNumber2",
        "merchantId": "merchantId0",
        "chainName": "chainName8",
        "merchantName": "merchantName4",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "processDate": "2016-03-13",
      "batchNumber": 226,
      "batchCardType": "batchCardType8",
      "saleCount": 66,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "hierarchy": {
        "storeNumber": "storeNumber2",
        "merchantId": "merchantId0",
        "chainName": "chainName8",
        "merchantName": "merchantName4",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "processDate": "2016-03-13",
      "batchNumber": 226,
      "batchCardType": "batchCardType8",
      "saleCount": 66,
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

