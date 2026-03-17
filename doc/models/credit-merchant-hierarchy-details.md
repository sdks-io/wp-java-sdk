
# Credit Merchant Hierarchy Details

Provides the merchant related details.

*This model accepts additional fields of type Object.*

## Structure

`CreditMerchantHierarchyDetails`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Hierarchy` | [`Hierarchy10`](../../doc/models/hierarchy-10.md) | Optional | - | Hierarchy10 getHierarchy() | setHierarchy(Hierarchy10 hierarchy) |
| `AlternateMerchantId` | `String` | Optional | An alternate 12-16 digit unique identifier assigned to each merchant.<br><br>**Constraints**: *Maximum Length*: `16` | String getAlternateMerchantId() | setAlternateMerchantId(String alternateMerchantId) |
| `AlternateStoreNumber` | `String` | Optional | Alternate store number is a secondary ID used to uniquely identify a store within a merchant's hierarchy.<br><br>**Constraints**: *Maximum Length*: `9` | String getAlternateStoreNumber() | setAlternateStoreNumber(String alternateStoreNumber) |
| `MerchantName` | `String` | Optional | The name of a business or registered name of the company or entity operating the business.<br><br>**Constraints**: *Maximum Length*: `40` | String getMerchantName() | setMerchantName(String merchantName) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "alternateMerchantId": "521112355854",
  "alternateStoreNumber": "147582547",
  "merchantName": "CLIENT SERVICES TEST",
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

