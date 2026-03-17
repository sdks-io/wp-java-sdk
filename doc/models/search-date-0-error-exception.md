
# Search Date 0 Error Exception

*This model accepts additional fields of type Object.*

## Structure

`SearchDate0ErrorException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ErrorCode` | `String` | Optional | Code of error<br><br>**Constraints**: *Maximum Length*: `256` | String getErrorCode() | setErrorCode(String errorCode) |
| `ErrorMessage` | `String` | Optional | Error Message<br><br>**Constraints**: *Maximum Length*: `256` | String getErrorMessage() | setErrorMessage(String errorMessage) |
| `Target` | `String` | Optional | Error Target<br><br>**Constraints**: *Maximum Length*: `256` | String getTarget() | setTarget(String target) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "errorCode": "ERROR_CODE",
  "errorMessage": "Error message here.",
  "target": "Target field name.",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

