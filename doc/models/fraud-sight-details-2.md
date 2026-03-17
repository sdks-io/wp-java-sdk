
# Fraud Sight Details 2

*This model accepts additional fields of type Object.*

## Structure

`FraudSightDetails2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `FraudScore` | `Double` | Optional | The measure that helps gauge risk involved with orders before processing.<br><br>**Constraints**: `>= 0`, `<= 1` | Double getFraudScore() | setFraudScore(Double fraudScore) |
| `FraudRule` | `String` | Optional | The condition that helps you decide whether an activity is fraudulent or not.<br><br>**Constraints**: *Maximum Length*: `30` | String getFraudRule() | setFraudRule(String fraudRule) |
| `FraudResponseCode` | [`FraudResponseCode2`](../../doc/models/fraud-response-code-2.md) | Optional | - | FraudResponseCode2 getFraudResponseCode() | setFraudResponseCode(FraudResponseCode2 fraudResponseCode) |
| `FraudRuleResult` | [`FraudRuleResult2`](../../doc/models/fraud-rule-result-2.md) | Optional | - | FraudRuleResult2 getFraudRuleResult() | setFraudRuleResult(FraudRuleResult2 fraudRuleResult) |
| `FraudResponseTime` | `String` | Optional | The time taken to verify if the transaction was fraudulent.<br><br>**Constraints**: *Maximum Length*: `4`, *Pattern*: `[0-9]{4}` | String getFraudResponseTime() | setFraudResponseTime(String fraudResponseTime) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "fraudScore": 0.13,
  "fraudRule": "CaR",
  "fraudResponseCode": {
    "code": "code6",
    "shortDescription": "shortDescription4",
    "longDescription": "longDescription8",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "fraudRuleResult": {
    "code": "code2",
    "shortDescription": "shortDescription0",
    "longDescription": "longDescription4",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "fraudResponseTime": "fraudResponseTime6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

