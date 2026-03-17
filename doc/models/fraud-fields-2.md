
# Fraud Fields 2

*This model accepts additional fields of type Object.*

## Structure

`FraudFields2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `FraudScore` | [`FraudScore`](../../doc/models/fraud-score.md) | Optional | - | FraudScore getFraudScore() | setFraudScore(FraudScore fraudScore) |
| `FraudResponseCode` | [`FraudResponseCode`](../../doc/models/fraud-response-code.md) | Optional | **Constraints**: *Maximum Length*: `256` | FraudResponseCode getFraudResponseCode() | setFraudResponseCode(FraudResponseCode fraudResponseCode) |
| `FraudRuleResult` | [`FraudRuleResult`](../../doc/models/fraud-rule-result.md) | Optional | **Constraints**: *Maximum Length*: `256` | FraudRuleResult getFraudRuleResult() | setFraudRuleResult(FraudRuleResult fraudRuleResult) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "fraudScore": {
    "fromScore": 1.0,
    "toScore": 1.0,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "fraudResponseCode": "NO_RESPONSE_FRAUD_SYSTEM_TIMEOUT",
  "fraudRuleResult": "FRAUD_SIGHT_NOT_INVOKED",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

