
# Credit Interchange Details

Provides information on interchange related details.

*This model accepts additional fields of type Object.*

## Structure

`CreditInterchangeDetails`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `CardProductResults` | [`CardProductResults`](../../doc/models/card-product-results.md) | Optional | - | CardProductResults getCardProductResults() | setCardProductResults(CardProductResults cardProductResults) |
| `CardProductType` | [`CardProductType`](../../doc/models/card-product-type.md) | Optional | - | CardProductType getCardProductType() | setCardProductType(CardProductType cardProductType) |
| `DaysLate` | `String` | Optional | The number of days late.<br><br>**Constraints**: *Maximum Length*: `3` | String getDaysLate() | setDaysLate(String daysLate) |
| `DiscountAmount` | `String` | Optional | The amount of the discount applied.<br><br>**Constraints**: *Maximum Length*: `255` | String getDiscountAmount() | setDiscountAmount(String discountAmount) |
| `InterchangeCode` | [`InterchangeCode`](../../doc/models/interchange-code.md) | Optional | - | InterchangeCode getInterchangeCode() | setInterchangeCode(InterchangeCode interchangeCode) |
| `InterchangeFee` | `String` | Optional | Fees between banks for processing credit and debit transactions interchangeably.<br><br>**Constraints**: *Maximum Length*: `255` | String getInterchangeFee() | setInterchangeFee(String interchangeFee) |
| `OriginalInterchangeIndicator` | `String` | Optional | Indicator of organization interchange.<br><br>**Constraints**: *Maximum Length*: `1` | String getOriginalInterchangeIndicator() | setOriginalInterchangeIndicator(String originalInterchangeIndicator) |
| `SurchargeAmount` | `String` | Optional | The additional fee added to the original cost or payment.<br><br>**Constraints**: *Maximum Length*: `255` | String getSurchargeAmount() | setSurchargeAmount(String surchargeAmount) |
| `SurchargeReason` | [`SurchargeReason`](../../doc/models/surcharge-reason.md) | Optional | - | SurchargeReason getSurchargeReason() | setSurchargeReason(SurchargeReason surchargeReason) |
| `MerchantSurchargeAmount` | `String` | Optional | The additional fee imposed by a merchant for using a particular payment method or service.<br><br>**Constraints**: *Maximum Length*: `255` | String getMerchantSurchargeAmount() | setMerchantSurchargeAmount(String merchantSurchargeAmount) |
| `ConvenienceFee` | `String` | Optional | The charge for the convenience of using a service or making a transaction, typically online.<br><br>**Constraints**: *Maximum Length*: `255` | String getConvenienceFee() | setConvenienceFee(String convenienceFee) |
| `BillingIndicator` | [`BillingIndicator`](../../doc/models/billing-indicator.md) | Optional | - | BillingIndicator getBillingIndicator() | setBillingIndicator(BillingIndicator billingIndicator) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "daysLate": "02",
  "interchangeFee": "17.25",
  "originalInterchangeIndicator": "5",
  "surchargeAmount": "893.56",
  "merchantSurchargeAmount": "893.56",
  "convenienceFee": "12.25",
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
}
```

