
# Other Services 2

*This model accepts additional fields of type Object.*

## Structure

`OtherServices2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `LevelIndicator` | [`LevelIndicator`](../../doc/models/level-indicator.md) | Optional | - | LevelIndicator getLevelIndicator() | setLevelIndicator(LevelIndicator levelIndicator) |
| `ReAuthorizationAttemptsCount` | `String` | Optional | The number of times reauthorization has been attempted.<br><br>**Constraints**: *Maximum Length*: `4` | String getReAuthorizationAttemptsCount() | setReAuthorizationAttemptsCount(String reAuthorizationAttemptsCount) |
| `SignatureCapabilitiesIndicator` | [`SignatureCapabilitiesIndicator`](../../doc/models/signature-capabilities-indicator.md) | Optional | - | SignatureCapabilitiesIndicator getSignatureCapabilitiesIndicator() | setSignatureCapabilitiesIndicator(SignatureCapabilitiesIndicator signatureCapabilitiesIndicator) |
| `SignatureCompression` | [`SignatureCompression`](../../doc/models/signature-compression.md) | Optional | - | SignatureCompression getSignatureCompression() | setSignatureCompression(SignatureCompression signatureCompression) |
| `SignatureEncryptKey` | `String` | Optional | Indicates the encryption key of the signature.<br><br>**Constraints**: *Maximum Length*: `4` | String getSignatureEncryptKey() | setSignatureEncryptKey(String signatureEncryptKey) |
| `SignatureEncryptMethod` | `String` | Optional | Used to verify the encryption method.<br><br>**Constraints**: *Maximum Length*: `2` | String getSignatureEncryptMethod() | setSignatureEncryptMethod(String signatureEncryptMethod) |
| `SignaturePen` | [`SignaturePen`](../../doc/models/signature-pen.md) | Optional | - | SignaturePen getSignaturePen() | setSignaturePen(SignaturePen signaturePen) |
| `StandInIndicator` | [`StandInIndicator`](../../doc/models/stand-in-indicator.md) | Optional | - | StandInIndicator getStandInIndicator() | setStandInIndicator(StandInIndicator standInIndicator) |
| `StandInLevel` | [`StandInLevel`](../../doc/models/stand-in-level.md) | Optional | - | StandInLevel getStandInLevel() | setStandInLevel(StandInLevel standInLevel) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "reAuthorizationAttemptsCount": "6",
  "levelIndicator": {
    "code": "code4",
    "shortDescription": "shortDescription8",
    "longDescription": "longDescription6",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "signatureCapabilitiesIndicator": {
    "code": "code8",
    "shortDescription": "shortDescription6",
    "longDescription": "longDescription0",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "signatureCompression": {
    "code": "code8",
    "shortDescription": "shortDescription4",
    "longDescription": "longDescription0",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "signatureEncryptKey": "signatureEncryptKey0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

