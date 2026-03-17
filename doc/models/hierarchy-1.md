
# Hierarchy 1

*This model accepts additional fields of type Object.*

## Structure

`Hierarchy1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Level` | [`Level1`](../../doc/models/level-1.md) | Optional | **Constraints**: *Maximum Length*: `30` | Level1 getLevel() | setLevel(Level1 level) |
| `Values` | `List<String>` | Optional | The values of the hierarchy levels.<br><br>**Constraints**: *Maximum Items*: `2000`, *Maximum Length*: `2000` | List<String> getValues() | setValues(List<String> values) |
| `ChainCode` | `String` | Optional | The level of the merchant hierarchy that groups merchant identifiers (MIDs) and any related roll-up values under a common identifier for settlement, billing, and reporting. Chain Code is the primary identifier for merchants boarded in MDB (Merchant Database) system. <br> Chain Code is mandatory when the level is store or division.<br><br>**Constraints**: *Maximum Length*: `6` | String getChainCode() | setChainCode(String chainCode) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "chainCode": "PA1234",
  "level": "CHAIN",
  "values": [
    "values2"
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

