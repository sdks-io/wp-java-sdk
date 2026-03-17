
# Signifyd Detail

Provides information on the signify details.

*This model accepts additional fields of type Object.*

## Structure

`SignifydDetail`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `FraudVendorId` | `String` | Optional | An vendor identification used in fraudulent schemes to deceive and exploit unsuspecting individuals or organizations.<br><br>**Constraints**: *Maximum Length*: `22` | String getFraudVendorId() | setFraudVendorId(String fraudVendorId) |
| `FraudCoverageType` | [`FraudCoverageType`](../../doc/models/fraud-coverage-type.md) | Optional | - | FraudCoverageType getFraudCoverageType() | setFraudCoverageType(FraudCoverageType fraudCoverageType) |
| `FraudDetectionStage` | [`FraudDetectionStage`](../../doc/models/fraud-detection-stage.md) | Optional | - | FraudDetectionStage getFraudDetectionStage() | setFraudDetectionStage(FraudDetectionStage fraudDetectionStage) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "fraudVendorId": "34455",
  "fraudCoverageType": {
    "code": "code2",
    "shortDescription": "shortDescription0",
    "longDescription": "longDescription4",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "fraudDetectionStage": {
    "code": "code8",
    "shortDescription": "shortDescription6",
    "longDescription": "longDescription0",
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

