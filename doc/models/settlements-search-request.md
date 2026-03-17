
# Settlements Search Request

*This model accepts additional fields of type Object.*

## Structure

`SettlementsSearchRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Pagination` | [`Pagination`](../../doc/models/pagination.md) | Optional | - | Pagination getPagination() | setPagination(Pagination pagination) |
| `SortResultsBy` | [`SortResultsBy`](../../doc/models/sort-results-by.md) | Optional | - | SortResultsBy getSortResultsBy() | setSortResultsBy(SortResultsBy sortResultsBy) |
| `Hierarchy` | [`Hierarchy`](../../doc/models/hierarchy.md) | Required | - | Hierarchy getHierarchy() | setHierarchy(Hierarchy hierarchy) |
| `DateType` | [`DateType`](../../doc/models/date-type.md) | Optional | **Constraints**: *Maximum Length*: `16` | DateType getDateType() | setDateType(DateType dateType) |
| `DateRange` | [`DateRange1`](../../doc/models/date-range-1.md) | Required | - | DateRange1 getDateRange() | setDateRange(DateRange1 dateRange) |
| `CardTypes` | [`CardTypes`](../../doc/models/card-types.md) | Optional | **Constraints**: *Maximum Length*: `6` | CardTypes getCardTypes() | setCardTypes(CardTypes cardTypes) |
| `CardNetworks` | [`CardNetworks`](../../doc/models/card-networks.md) | Optional | - | CardNetworks getCardNetworks() | setCardNetworks(CardNetworks cardNetworks) |
| `CardNumber` | `String` | Optional | The number found on the card used to make a purchase, also referred to as the bank or credit card number. Searches can be done on the full card number, on the first six and last four digits, on the first six digits, or on the last four digit.<br><br>**Constraints**: *Maximum Length*: `19` | String getCardNumber() | setCardNumber(String cardNumber) |
| `Token` | `Long` | Optional | The numeric value that is the same length as the card number and is used as a substitution with proxy data. Max length of the token is 19 characters.<br><br>**Constraints**: `<= 19` | Long getToken() | setToken(Long token) |
| `ReferenceNumber` | `String` | Optional | The key to uniquely identify a card transaction based on the ISO 8583 standard. <br> Card Type is mandatory for passing search by Reference Number.<br><br>**Constraints**: *Maximum Length*: `23` | String getReferenceNumber() | setReferenceNumber(String referenceNumber) |
| `TransactionId` | `String` | Optional | The unique 12-19 digit identifier that is generated with every card transaction and from the electronic transfer of funds.<br><br>**Constraints**: *Maximum Length*: `19` | String getTransactionId() | setTransactionId(String transactionId) |
| `TransactionTypeCode` | [`TransactionTypeCode1`](../../doc/models/transaction-type-code-1.md) | Optional | **Constraints**: *Maximum Length*: `3` | TransactionTypeCode1 getTransactionTypeCode() | setTransactionTypeCode(TransactionTypeCode1 transactionTypeCode) |
| `TransactionStatusCode` | [`TransactionStatusCode1`](../../doc/models/transaction-status-code-1.md) | Optional | **Constraints**: *Maximum Length*: `3` | TransactionStatusCode1 getTransactionStatusCode() | setTransactionStatusCode(TransactionStatusCode1 transactionStatusCode) |
| `TransactionAmountRange` | [`TransactionAmountRange`](../../doc/models/transaction-amount-range.md) | Optional | - | TransactionAmountRange getTransactionAmountRange() | setTransactionAmountRange(TransactionAmountRange transactionAmountRange) |
| `FraudFields` | [`FraudFields2`](../../doc/models/fraud-fields-2.md) | Optional | - | FraudFields2 getFraudFields() | setFraudFields(FraudFields2 fraudFields) |
| `CustomerFields` | [`CustomerFields2`](../../doc/models/customer-fields-2.md) | Optional | - | CustomerFields2 getCustomerFields() | setCustomerFields(CustomerFields2 customerFields) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "hierarchy": {
    "chainCode": "PA1234",
    "level": "DIVISION",
    "values": [
      "values6",
      "values7"
    ],
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "dateRange": {
    "fromDate": "2021-12-01",
    "toDate": "2021-12-01",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "cardNumber": "123456XXXXXX9876",
  "referenceNumber": "2444677778440029",
  "transactionId": "141715459519",
  "pagination": {
    "pageNumber": 16776215,
    "pageSize": 1000,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "sortResultsBy": {
    "fieldName": "CHAIN_CODE",
    "orderBy": "ASC",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "dateType": "PROCESS_DATE",
  "cardTypes": "CREDIT",
  "cardNetworks": "POSA_GIFT_CARD",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

