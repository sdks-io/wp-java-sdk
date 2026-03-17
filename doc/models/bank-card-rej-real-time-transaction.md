
# Bank Card Rej Real Time Transaction

The details of the real-time bank card transaction rejection.

*This model accepts additional fields of type Object.*

## Structure

`BankCardRejRealTimeTransaction`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ProcessDate` | `LocalDate` | Optional | The date when the transaction has been processed for settlement between the two parties. | LocalDate getProcessDate() | setProcessDate(LocalDate processDate) |
| `BatchNumber` | `Integer` | Optional | The unique identifier assigned to a group of transactions that were handled together as a single unit.<br><br>**Constraints**: `<= 6` | Integer getBatchNumber() | setBatchNumber(Integer batchNumber) |
| `BatchAmount` | `Double` | Optional | The total amount of all the transactions that are part of the batch file.<br><br>**Constraints**: `<= 10` | Double getBatchAmount() | setBatchAmount(Double batchAmount) |
| `SaleCount` | `Integer` | Optional | The sale count of the transaction.<br><br>**Constraints**: `<= 9999999999` | Integer getSaleCount() | setSaleCount(Integer saleCount) |
| `SaleAmount` | `Double` | Optional | The sale amount of the transaction.<br><br>**Constraints**: `>= 0`, `<= 9999999.99` | Double getSaleAmount() | setSaleAmount(Double saleAmount) |
| `ReturnCount` | `Integer` | Optional | The number of items sent back from a transaction.<br><br>**Constraints**: `<= 9999999999` | Integer getReturnCount() | setReturnCount(Integer returnCount) |
| `ReturnAmount` | `Double` | Optional | The amount returned from a transaction.<br><br>**Constraints**: `>= 0`, `<= 9999999.99` | Double getReturnAmount() | setReturnAmount(Double returnAmount) |
| `RejectionReason` | [`RejectionReason`](../../doc/models/rejection-reason.md) | Optional | - | RejectionReason getRejectionReason() | setRejectionReason(RejectionReason rejectionReason) |
| `BatchHoldStatus` | [`BatchHoldStatus`](../../doc/models/batch-hold-status.md) | Optional | - | BatchHoldStatus getBatchHoldStatus() | setBatchHoldStatus(BatchHoldStatus batchHoldStatus) |
| `Hierarchy` | [`Hierarchy9`](../../doc/models/hierarchy-9.md) | Optional | - | Hierarchy9 getHierarchy() | setHierarchy(Hierarchy9 hierarchy) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "processDate": "2021-07-19",
  "saleCount": 7,
  "saleAmount": 37551.08,
  "returnCount": 2,
  "returnAmount": 113.08,
  "batchNumber": 6,
  "batchAmount": 10.0,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

