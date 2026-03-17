
# Hierarchy 4

*This model accepts additional fields of type Object.*

## Structure

`Hierarchy4`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `StoreNumber` | `String` | Optional | The lowest roll-up level in the hierarchy system, grouping multiple merchant account numbers (MIDs) used in a single merchant location. The Store/Locations are used to link multiple merchant numbers assigned to different terminals and/or business lines (MCC’s). A Store Number is nine digits and unique to a particular Chain.<br><br>**Constraints**: *Maximum Length*: `9` | String getStoreNumber() | setStoreNumber(String storeNumber) |
| `MerchantId` | `String` | Optional | The identifier code associated with a given merchant under a Store-level hierarchy.<br><br>**Constraints**: *Maximum Length*: `16` | String getMerchantId() | setMerchantId(String merchantId) |
| `ChainName` | `String` | Optional | The name associated with a given merchant under a chain-level hierarchy.<br><br>**Constraints**: *Maximum Length*: `40` | String getChainName() | setChainName(String chainName) |
| `MerchantName` | `String` | Optional | The name of a business or registered name of the company or entity operating the business.<br><br>**Constraints**: *Maximum Length*: `40` | String getMerchantName() | setMerchantName(String merchantName) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "storeNumber": "000000001",
  "merchantId": "2555091034216",
  "chainName": "ABC KLM Tech",
  "merchantName": "CLIENT SERVICES TEST",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

