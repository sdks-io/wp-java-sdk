
# Search Daily Totals Details

Fields used to search daily totals.

*This model accepts additional fields of type Object.*

## Structure

`SearchDailyTotalsDetails`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `CardType` | `String` | Optional | The category or classification of a payment card based on the issuing network.<br><br>**Constraints**: *Maximum Length*: `6` | String getCardType() | setCardType(String cardType) |
| `BatchNumber` | `Integer` | Optional | The 11-byte unique identifier assigned to a group of transactions that were handled together as a single unit.<br><br>**Constraints**: `<= 11` | Integer getBatchNumber() | setBatchNumber(Integer batchNumber) |
| `ProcessDate` | `LocalDate` | Optional | The date when the transaction has been processed for settlement between the two parties. | LocalDate getProcessDate() | setProcessDate(LocalDate processDate) |
| `TransactionDate` | `LocalDate` | Optional | The date and time when the bank has settled the transaction (deposits or withdraws funds). | LocalDate getTransactionDate() | setTransactionDate(LocalDate transactionDate) |
| `Hierarchy` | [`Hierarchy10`](../../doc/models/hierarchy-10.md) | Optional | - | Hierarchy10 getHierarchy() | setHierarchy(Hierarchy10 hierarchy) |
| `TransactionSummary` | [`TransactionSummary`](../../doc/models/transaction-summary.md) | Optional | - | TransactionSummary getTransactionSummary() | setTransactionSummary(TransactionSummary transactionSummary) |
| `InterchangeDetails` | [`InterchangeDetails1`](../../doc/models/interchange-details-1.md) | Optional | - | InterchangeDetails1 getInterchangeDetails() | setInterchangeDetails(InterchangeDetails1 interchangeDetails) |
| `Terminal` | [`Terminal`](../../doc/models/terminal.md) | Optional | - | Terminal getTerminal() | setTerminal(Terminal terminal) |
| `FundedNetSettle` | [`FundedNetSettle2`](../../doc/models/funded-net-settle-2.md) | Optional | - | FundedNetSettle2 getFundedNetSettle() | setFundedNetSettle(FundedNetSettle2 fundedNetSettle) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "cardType": "CREDIT",
  "processDate": "2022-07-19",
  "transactionDate": "2023-07-19",
  "batchNumber": 11,
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
```

