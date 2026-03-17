
# Fraud Score

*This model accepts additional fields of type Object.*

## Structure

`FraudScore`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `FromScore` | `Double` | Optional | The starting score for the range for fraud.<br><br>**Constraints**: `>= 0`, `<= 1` | Double getFromScore() | setFromScore(Double fromScore) |
| `ToScore` | `Double` | Optional | The ending score for the range for fraud.<br><br>**Constraints**: `>= 0`, `<= 1` | Double getToScore() | setToScore(Double toScore) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "fromScore": 0.13,
  "toScore": 0.84,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

