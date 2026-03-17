
# Premium Payback

*This model accepts additional fields of type Object.*

## Structure

`PremiumPayback`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `IndicatorPassed` | `Boolean` | Optional | Possible values are True or False. | Boolean getIndicatorPassed() | setIndicatorPassed(Boolean indicatorPassed) |
| `EligibleBin` | `Boolean` | Optional | Possible values are True or False. | Boolean getEligibleBin() | setEligibleBin(Boolean eligibleBin) |
| `Eligible` | `Boolean` | Optional | Possible values are True or False. | Boolean getEligible() | setEligible(Boolean eligible) |
| `RedemptionAccepted` | `Boolean` | Optional | Possible values are True or False. | Boolean getRedemptionAccepted() | setRedemptionAccepted(Boolean redemptionAccepted) |
| `RedemptionAmount` | `Double` | Optional | Indicates the early repayment charges.<br><br>**Constraints**: `>= 0`, `<= 999999999.99` | Double getRedemptionAmount() | setRedemptionAmount(Double redemptionAmount) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "indicatorPassed": false,
  "eligibleBIN": false,
  "eligible": false,
  "redemptionAccepted": false,
  "redemptionAmount": 200.56,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

