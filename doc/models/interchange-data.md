
# Interchange Data

Refers to interchange data.

*This model accepts additional fields of type Object.*

## Structure

`InterchangeData`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TieBreaker` | `String` | Optional | Mechanism to resolve disputes or conflicts in settlements.<br><br>**Constraints**: *Maximum Length*: `6` | String getTieBreaker() | setTieBreaker(String tieBreaker) |
| `InterchangeFees` | `Double` | Optional | Fees between banks for processing credit and debit transactions interchangeably.<br><br>**Constraints**: `>= 0`, `<= 1000000000` | Double getInterchangeFees() | setInterchangeFees(Double interchangeFees) |
| `SurchargeAmount` | `Double` | Optional | An additional fee added to the original cost or payment.<br><br>**Constraints**: `>= 0`, `<= 999999.999999999` | Double getSurchargeAmount() | setSurchargeAmount(Double surchargeAmount) |
| `MerchantSurchargeAmount` | `Double` | Optional | An additional fee imposed by a merchant for using a particular payment method or service.<br><br>**Constraints**: `>= 0`, `<= 999999.999999999` | Double getMerchantSurchargeAmount() | setMerchantSurchargeAmount(Double merchantSurchargeAmount) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "tieBreaker": "AB3645",
  "interchangeFees": 14857.49,
  "surchargeAmount": 893.56,
  "merchantSurchargeAmount": 9845.87,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

