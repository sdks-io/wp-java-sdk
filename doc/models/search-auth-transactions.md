
# Search Auth Transactions

Search authorization transaction information.

*This model accepts additional fields of type Object.*

## Structure

`SearchAuthTransactions`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TransactionDetails` | [`TransactionDetails2`](../../doc/models/transaction-details-2.md) | Optional | - | TransactionDetails2 getTransactionDetails() | setTransactionDetails(TransactionDetails2 transactionDetails) |
| `CardDetails` | [`CardDetails2`](../../doc/models/card-details-2.md) | Optional | - | CardDetails2 getCardDetails() | setCardDetails(CardDetails2 cardDetails) |
| `LocationDetails` | [`LocationDetails2`](../../doc/models/location-details-2.md) | Optional | - | LocationDetails2 getLocationDetails() | setLocationDetails(LocationDetails2 locationDetails) |
| `InterchangeDetails` | [`InterchangeDetails`](../../doc/models/interchange-details.md) | Optional | - | InterchangeDetails getInterchangeDetails() | setInterchangeDetails(InterchangeDetails interchangeDetails) |
| `PremiumPayback` | [`PremiumPayback`](../../doc/models/premium-payback.md) | Optional | - | PremiumPayback getPremiumPayback() | setPremiumPayback(PremiumPayback premiumPayback) |
| `OtherServices` | [`OtherServices2`](../../doc/models/other-services-2.md) | Optional | - | OtherServices2 getOtherServices() | setOtherServices(OtherServices2 otherServices) |
| `EmvDetails` | [`EmvDetails2`](../../doc/models/emv-details-2.md) | Optional | - | EmvDetails2 getEmvDetails() | setEmvDetails(EmvDetails2 emvDetails) |
| `FraudSightDetails` | [`FraudSightDetails2`](../../doc/models/fraud-sight-details-2.md) | Optional | - | FraudSightDetails2 getFraudSightDetails() | setFraudSightDetails(FraudSightDetails2 fraudSightDetails) |
| `SignifyDetails` | [`SignifyDetails`](../../doc/models/signify-details.md) | Optional | - | SignifyDetails getSignifyDetails() | setSignifyDetails(SignifyDetails signifyDetails) |
| `AdditionalDetails` | [`AdditionalDetails`](../../doc/models/additional-details.md) | Optional | - | AdditionalDetails getAdditionalDetails() | setAdditionalDetails(AdditionalDetails additionalDetails) |
| `CustomerFields` | [`CustomerFields2`](../../doc/models/customer-fields-2.md) | Optional | - | CustomerFields2 getCustomerFields() | setCustomerFields(CustomerFields2 customerFields) |
| `PaymentGatewayDetails` | [`PaymentGatewayDetails1`](../../doc/models/payment-gateway-details-1.md) | Optional | - | PaymentGatewayDetails1 getPaymentGatewayDetails() | setPaymentGatewayDetails(PaymentGatewayDetails1 paymentGatewayDetails) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "transactionDetails": {
    "transactionId": "transactionId4",
    "processDate": "2016-03-13",
    "transactionDateTime": "2016-03-13T12:52:32.123Z",
    "authorizationAmount": 190.72,
    "approvedAmount": 149.58,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "cardDetails": {
    "cardNumber": "cardNumber0",
    "cardType": "cardType8",
    "expirationDate": "2016-03-13",
    "cardNetwork": {
      "code": "code8",
      "shortDescription": "shortDescription6",
      "longDescription": "longDescription0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    "cvv2ResponseCode": {
      "code": "code8",
      "shortDescription": "shortDescription4",
      "longDescription": "longDescription0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "locationDetails": {
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
    "alternateMerchantId": "alternateMerchantId8",
    "alternateStoreNumber": "alternateStoreNumber0",
    "merchantName": "merchantName2",
    "acro": "acro2",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "interchangeDetails": {
    "cardProductResults": {
      "code": "code8",
      "shortDescription": "shortDescription4",
      "longDescription": "longDescription0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    "cardProductType": {
      "code": "code0",
      "shortDescription": "shortDescription2",
      "longDescription": "longDescription2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    "daysLate": "daysLate4",
    "discountAmount": "discountAmount0",
    "interchangeCode": {
      "code": "code2",
      "description": "description4",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "premiumPayback": {
    "indicatorPassed": false,
    "eligibleBIN": false,
    "eligible": false,
    "redemptionAccepted": false,
    "redemptionAmount": 78.86,
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

