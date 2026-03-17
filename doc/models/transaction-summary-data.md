
# Transaction Summary Data

The summary of the transaction data.

*This model accepts additional fields of type Object.*

## Structure

`TransactionSummaryData`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `SettlementAmount` | `Double` | Optional | The total sum of transactions processed and finalized within a specific time period.<br><br>**Constraints**: `>= 0`, `<= 999999999.99` | Double getSettlementAmount() | setSettlementAmount(Double settlementAmount) |
| `AuthorizationAmount` | `Double` | Optional | The approved amount of money to be charged.<br><br>**Constraints**: `>= 0`, `<= 1E+17` | Double getAuthorizationAmount() | setAuthorizationAmount(Double authorizationAmount) |
| `DiscountAmount` | `Double` | Optional | The amount of the discount applied.<br><br>**Constraints**: `>= 0`, `<= 999999.999999999` | Double getDiscountAmount() | setDiscountAmount(Double discountAmount) |
| `SalesCount` | `Double` | Optional | The number of card sales over a given period of time.<br><br>**Constraints**: `<= 999999999` | Double getSalesCount() | setSalesCount(Double salesCount) |
| `ReturnsCount` | `Double` | Optional | The number of returns over a given period of time.<br><br>**Constraints**: `<= 999999999` | Double getReturnsCount() | setReturnsCount(Double returnsCount) |
| `TransactionsCount` | `Double` | Optional | The number of transactions over a given period of time.<br><br>**Constraints**: `<= 999999999` | Double getTransactionsCount() | setTransactionsCount(Double transactionsCount) |
| `ReversalsCount` | `Double` | Optional | The number of reversals over a given period of time.<br><br>**Constraints**: `<= 999999999` | Double getReversalsCount() | setReversalsCount(Double reversalsCount) |
| `AdjustmentsCount` | `Double` | Optional | The number of corrections or changes made to finalized transactions.<br><br>**Constraints**: `<= 999999999` | Double getAdjustmentsCount() | setAdjustmentsCount(Double adjustmentsCount) |
| `AdjustmentsAmount` | `Double` | Optional | The amount of the transaction totals changed for accuracy and reconciliation purposes.<br><br>**Constraints**: `>= 0`, `<= 999999999.99` | Double getAdjustmentsAmount() | setAdjustmentsAmount(Double adjustmentsAmount) |
| `ApprovedAmount` | `Double` | Optional | The agreed upon sum for a transaction after authorization and processing steps.<br><br>**Constraints**: `>= 0`, `<= 999999999.99` | Double getApprovedAmount() | setApprovedAmount(Double approvedAmount) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "settlementAmount": 100.04,
  "authorizationAmount": 150.87,
  "salesCount": 485.0,
  "returnsCount": 275.0,
  "transactionsCount": 548,
  "reversalsCount": 563,
  "adjustmentsCount": 3487,
  "adjustmentsAmount": 54.09,
  "approvedAmount": 29.04,
  "discountAmount": 226.18,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

