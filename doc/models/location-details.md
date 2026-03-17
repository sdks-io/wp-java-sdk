
# Location Details

Provides details of the transaction location and merchant related information.

*This model accepts additional fields of type Object.*

## Structure

`LocationDetails`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Hierarchy` | [`Hierarchy10`](../../doc/models/hierarchy-10.md) | Optional | - | Hierarchy10 getHierarchy() | setHierarchy(Hierarchy10 hierarchy) |
| `AlternateMerchantId` | `String` | Optional | An alternate 12-16 digit unique identifier assigned to each merchant.<br><br>**Constraints**: *Maximum Length*: `16` | String getAlternateMerchantId() | setAlternateMerchantId(String alternateMerchantId) |
| `AlternateStoreNumber` | `String` | Optional | Alternate store number is a secondary ID used to uniquely identify a store within a merchant's hierarchy.<br><br>**Constraints**: *Maximum Length*: `9` | String getAlternateStoreNumber() | setAlternateStoreNumber(String alternateStoreNumber) |
| `MerchantName` | `String` | Optional | The name of a business or registered name of the company or entity operating the business.<br><br>**Constraints**: *Maximum Length*: `40` | String getMerchantName() | setMerchantName(String merchantName) |
| `Acro` | `String` | Optional | Each hierarchy has a generic ACRO defined by default per banking relationship. All merchants have a four character billing acronym.<br><br>**Constraints**: *Maximum Length*: `4` | String getAcro() | setAcro(String acro) |
| `MerchantTimeZone` | `String` | Optional | The region where a merchant conducts business, reflecting local time.<br><br>**Constraints**: *Maximum Length*: `3` | String getMerchantTimeZone() | setMerchantTimeZone(String merchantTimeZone) |
| `SalesPerson` | `Integer` | Optional | The unique identifier of the Sales Person/Employee/Clerk for transcation handling accountability.<br><br>**Constraints**: `<= 9` | Integer getSalesPerson() | setSalesPerson(Integer salesPerson) |
| `AgentBank` | `String` | Optional | The gift card agent allowing merchants to distinguish between different card programs, if necessary. Worldpay assigns these 4-digit values.<br><br>**Constraints**: *Maximum Length*: `4` | String getAgentBank() | setAgentBank(String agentBank) |
| `CountryOfOrigin` | [`CountryOfOrigin`](../../doc/models/country-of-origin.md) | Optional | - | CountryOfOrigin getCountryOfOrigin() | setCountryOfOrigin(CountryOfOrigin countryOfOrigin) |
| `GovernmentControlledEntity` | `Boolean` | Optional | If the entity is owned, controlled, or influenced by the government for public interest. <br> Possible values are True or False. | Boolean getGovernmentControlledEntity() | setGovernmentControlledEntity(Boolean governmentControlledEntity) |
| `MerchantCategory` | [`MerchantCategory`](../../doc/models/merchant-category.md) | Optional | - | MerchantCategory getMerchantCategory() | setMerchantCategory(MerchantCategory merchantCategory) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "alternateMerchantId": "521112355854",
  "alternateStoreNumber": "147582547",
  "merchantName": "CLIENT SERVICES TEST",
  "acro": "WALG",
  "merchantTimeZone": "UST",
  "agentBank": "0000",
  "governmentControlledEntity": true,
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

