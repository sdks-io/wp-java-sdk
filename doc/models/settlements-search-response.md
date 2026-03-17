
# Settlements Search Response

*This model accepts additional fields of type Object.*

## Structure

`SettlementsSearchResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Pagination` | [`PaginationResponse`](../../doc/models/pagination-response.md) | Optional | The format used to display your resources. | PaginationResponse getPagination() | setPagination(PaginationResponse pagination) |
| `Settlements` | [`List<SearchAuthTransactions>`](../../doc/models/search-auth-transactions.md) | Optional | The details of the settlement transactions.<br><br>**Constraints**: *Maximum Items*: `12` | List<SearchAuthTransactions> getSettlements() | setSettlements(List<SearchAuthTransactions> settlements) |
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
  "settlements": [
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
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

