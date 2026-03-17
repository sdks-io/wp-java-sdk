
# Settlement Rej Real Time Transaction

The details of the real-time transactions settlement rejections.

*This model accepts additional fields of type Object.*

## Structure

`SettlementRejRealTimeTransaction`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ProcessedDate` | `LocalDate` | Optional | The date when the transaction has been processed for settlement between the two parties. | LocalDate getProcessedDate() | setProcessedDate(LocalDate processedDate) |
| `TransactionDate` | `LocalDate` | Optional | The date and time when the bank has settled/rejected the transaction (deposits or withdraws funds). | LocalDate getTransactionDate() | setTransactionDate(LocalDate transactionDate) |
| `ResubmitDate` | `LocalDate` | Optional | The resubmission date of the transaction. | LocalDate getResubmitDate() | setResubmitDate(LocalDate resubmitDate) |
| `AccountNumber` | `String` | Optional | The account number or card number involved in the rejected transaction.<br><br>**Constraints**: *Maximum Length*: `19` | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `DdaNumber` | `String` | Optional | Demand deposit account is a type of bank account that offers access to money.<br><br>**Constraints**: *Maximum Length*: `17` | String getDdaNumber() | setDdaNumber(String ddaNumber) |
| `Amount` | `Double` | Optional | The rejected transaction amount.<br><br>**Constraints**: `<= 10` | Double getAmount() | setAmount(Double amount) |
| `RejectionReason` | [`RejectionReason`](../../doc/models/rejection-reason.md) | Optional | - | RejectionReason getRejectionReason() | setRejectionReason(RejectionReason rejectionReason) |
| `Hierarchy` | [`Hierarchy7`](../../doc/models/hierarchy-7.md) | Optional | - | Hierarchy7 getHierarchy() | setHierarchy(Hierarchy7 hierarchy) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "processedDate": "2022-07-19",
  "transactionDate": "2022-07-19",
  "resubmitDate": "2022-07-21",
  "accountNumber": "4445123456789012",
  "ddaNumber": "4020016689",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

