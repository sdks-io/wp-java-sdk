
# Merchant Info

The merchant information.

*This model accepts additional fields of type Object.*

## Structure

`MerchantInfo`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ChainCode` | `String` | Optional | The level of the merchant hierarchy that groups merchant identifiers (MIDs) and any related roll-up values under a common identifier for settlement, billing, and reporting. Chain Code is the primary identifier for merchants boarded in MDB (Merchant Database) system.<br><br>**Constraints**: *Maximum Length*: `6` | String getChainCode() | setChainCode(String chainCode) |
| `DivisionNumber` | `String` | Optional | The hierarchy level that enables merchants to roll-up child entities for Stores/Locations into different groups under a Chain. The Division Code is an optional hierarchy level, but if created, is required for all child entities under the Division Number."<br><br>**Constraints**: *Maximum Length*: `3` | String getDivisionNumber() | setDivisionNumber(String divisionNumber) |
| `StoreNumber` | `String` | Optional | The lowest roll-up level in the hierarchy system, grouping multiple merchant account numbers (MIDs) used in a single merchant location. The Store/Locations are used to link multiple merchant numbers assigned to different terminals and/or business lines (MCC’s).<br><br>**Constraints**: *Maximum Length*: `9` | String getStoreNumber() | setStoreNumber(String storeNumber) |
| `MerchantId` | `String` | Optional | The identifier code associated with a given merchant under a Store-level hierarchy.<br><br>**Constraints**: *Maximum Length*: `16` | String getMerchantId() | setMerchantId(String merchantId) |
| `AlternateMerchantId` | `String` | Optional | The lowest level in the Merchant Hierarchy structure.<br><br>**Constraints**: *Maximum Length*: `16` | String getAlternateMerchantId() | setAlternateMerchantId(String alternateMerchantId) |
| `MerchantName` | `String` | Optional | The name of a business or registered name of the company or entity operating the business.<br><br>**Constraints**: *Maximum Length*: `40` | String getMerchantName() | setMerchantName(String merchantName) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "chainCode": "PA1234",
  "divisionNumber": "002",
  "storeNumber": "000000001",
  "merchantId": "2555091034216",
  "alternateMerchantId": "521112355854",
  "merchantName": "CLIENT SERVICES TEST",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

