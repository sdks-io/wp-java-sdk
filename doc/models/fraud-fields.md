
# Fraud Fields

Metric indicating a transaction's potential fraudulent activity level.

*This model accepts additional fields of type Object.*

## Structure

`FraudFields`

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
  "fraudResponseCode": "NO_RESPONSE_FRAUD_SYSTEM_ERROR",
  "fraudRuleResult": "DECLINE",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

