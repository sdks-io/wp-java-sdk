
# Settlement Batches Transaction Store

Request fields for settlement batches for a store.

*This model accepts additional fields of type Object.*

## Structure

`SettlementBatchesTransactionStore`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Hierarchy` | [`Hierarchy4`](../../doc/models/hierarchy-4.md) | Optional | - | Hierarchy4 getHierarchy() | setHierarchy(Hierarchy4 hierarchy) |
| `ProcessDate` | `LocalDate` | Optional | The date when the transaction has been processed for settlement between the two parties. | LocalDate getProcessDate() | setProcessDate(LocalDate processDate) |
| `NumberOfBatches` | `Integer` | Optional | Refers to a group of processed transaction records. | Integer getNumberOfBatches() | setNumberOfBatches(Integer numberOfBatches) |
| `BatchCardType` | `String` | Optional | The category or classification of a payment card based on the issuing network. Types are CREDIT,DEBIT, and EBT.<br><br>**Constraints**: *Maximum Length*: `6` | String getBatchCardType() | setBatchCardType(String batchCardType) |
| `SaleCount` | `Double` | Optional | Indicates the number of items sold within a specific batch quantity.<br><br>**Constraints**: `>= 0`, `<= 999999999` | Double getSaleCount() | setSaleCount(Double saleCount) |
| `SaleAmount` | `Double` | Optional | Total revenue generated from selling items within a specific batch.<br><br>**Constraints**: `>= 0`, `<= 99999999.99` | Double getSaleAmount() | setSaleAmount(Double saleAmount) |
| `ReturnCount` | `Double` | Optional | Indicates the number of items sent back within a batch.<br><br>**Constraints**: `>= 0`, `<= 999999999` | Double getReturnCount() | setReturnCount(Double returnCount) |
| `ReturnAmount` | `Double` | Optional | Indicates amount refunded within a batch.<br><br>**Constraints**: `>= 0`, `<= 999999999.99` | Double getReturnAmount() | setReturnAmount(Double returnAmount) |
| `CashAdvanceCount` | `Double` | Optional | The total number of cash advances that were issued.<br><br>**Constraints**: `>= 0`, `<= 999999999` | Double getCashAdvanceCount() | setCashAdvanceCount(Double cashAdvanceCount) |
| `CashAdvanceAmount` | `Double` | Optional | The sum of the borrowed funds.<br><br>**Constraints**: `>= 0`, `<= 99999999.99` | Double getCashAdvanceAmount() | setCashAdvanceAmount(Double cashAdvanceAmount) |
| `NetCount` | `Double` | Optional | The total remaining amount after deductions.<br><br>**Constraints**: `>= 0`, `<= 999999999` | Double getNetCount() | setNetCount(Double netCount) |
| `NetAmount` | `Double` | Optional | The count minus deductions.<br><br>**Constraints**: `>= 0`, `<= 99999999.99` | Double getNetAmount() | setNetAmount(Double netAmount) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "processDate": "2023-07-19",
  "numberOfBatches": 125,
  "batchCardType": "CREDIT",
  "saleCount": 2458.0,
  "saleAmount": 37551.08,
  "returnCount": 6589,
  "returnAmount": 113.08,
  "cashAdvanceCount": 548,
  "cashAdvanceAmount": 199.51,
  "netCount": 1845,
  "netAmount": 77.52,
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
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

