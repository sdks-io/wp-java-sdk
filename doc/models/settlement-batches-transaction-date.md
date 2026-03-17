
# Settlement Batches Transaction Date

The settlement batches transaction date.

*This model accepts additional fields of type Object.*

## Structure

`SettlementBatchesTransactionDate`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Hierarchy` | [`Hierarchy4`](../../doc/models/hierarchy-4.md) | Optional | - | Hierarchy4 getHierarchy() | setHierarchy(Hierarchy4 hierarchy) |
| `ProcessDate` | `LocalDate` | Optional | The date when the transaction has been processed for settlement between the two parties. | LocalDate getProcessDate() | setProcessDate(LocalDate processDate) |
| `BatchNumber` | `Integer` | Optional | The 11-byte unique identifier assigned to a group of transactions that were handled together as a single unit. | Integer getBatchNumber() | setBatchNumber(Integer batchNumber) |
| `BatchCardType` | `String` | Optional | The category or classification of a payment card based on the issuing network. The type is either Credit or Debit.<br><br>**Constraints**: *Maximum Length*: `6` | String getBatchCardType() | setBatchCardType(String batchCardType) |
| `SaleCount` | `Integer` | Optional | The number of items sold within a specific batch quantity.<br><br>**Constraints**: `>= 0`, `<= 9999999999` | Integer getSaleCount() | setSaleCount(Integer saleCount) |
| `SaleAmount` | `Double` | Optional | The total revenue generated from selling items within a specific batch.<br><br>**Constraints**: `>= 0`, `<= 9999999999999.99` | Double getSaleAmount() | setSaleAmount(Double saleAmount) |
| `ReturnCount` | `Integer` | Optional | The number of items sent back within a batch.<br><br>**Constraints**: `>= 0`, `<= 9999` | Integer getReturnCount() | setReturnCount(Integer returnCount) |
| `ReturnAmount` | `Double` | Optional | The amount refunded within a batch.<br><br>**Constraints**: `>= 0`, `<= 9999999999999.99` | Double getReturnAmount() | setReturnAmount(Double returnAmount) |
| `CashAdvanceCount` | `Integer` | Optional | The total number of cash advances issued.<br><br>**Constraints**: `>= 0`, `<= 9999` | Integer getCashAdvanceCount() | setCashAdvanceCount(Integer cashAdvanceCount) |
| `CashAdvanceAmount` | `Double` | Optional | The sum of the borrowed funds.<br><br>**Constraints**: `>= 0`, `<= 9999999999999.99` | Double getCashAdvanceAmount() | setCashAdvanceAmount(Double cashAdvanceAmount) |
| `NetCount` | `Integer` | Optional | The total remaining amount after deductions.<br><br>**Constraints**: `>= 0`, `<= 9999` | Integer getNetCount() | setNetCount(Integer netCount) |
| `NetAmount` | `Double` | Optional | The count minus deductions.<br><br>**Constraints**: `>= 0`, `<= 9999999999999.99` | Double getNetAmount() | setNetAmount(Double netAmount) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "processDate": "2023-07-19",
  "batchNumber": 311111,
  "batchCardType": "CREDIT",
  "saleCount": 7,
  "saleAmount": 37551.08,
  "returnCount": 2,
  "returnAmount": 113.08,
  "cashAdvanceCount": 2,
  "cashAdvanceAmount": 109.51,
  "netCount": 1,
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

