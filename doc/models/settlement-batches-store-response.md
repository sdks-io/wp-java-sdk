
# Settlement Batches Store Response

Response used for pagination.

*This model accepts additional fields of type Object.*

## Structure

`SettlementBatchesStoreResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Pagination` | [`Pagination4`](../../doc/models/pagination-4.md) | Optional | - | Pagination4 getPagination() | setPagination(Pagination4 pagination) |
| `Details` | [`List<SettlementBatchesTransactionStore>`](../../doc/models/settlement-batches-transaction-store.md) | Optional | The settlement batches details.<br><br>**Constraints**: *Maximum Items*: `1` | List<SettlementBatchesTransactionStore> getDetails() | setDetails(List<SettlementBatchesTransactionStore> details) |
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
      "numberOfBatches": 208,
      "batchCardType": "batchCardType8",
      "saleCount": 213.14,
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
      "numberOfBatches": 208,
      "batchCardType": "batchCardType8",
      "saleCount": 213.14,
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

