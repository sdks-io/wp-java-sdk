
# Rejection Reason

*This model accepts additional fields of type Object.*

## Structure

`RejectionReason`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Code` | `String` | Optional | The identifier code.<br><br>**Constraints**: *Maximum Length*: `3` | String getCode() | setCode(String code) |
| `ShortDescription` | `String` | Optional | The short description of the code.<br><br>**Constraints**: *Maximum Length*: `15` | String getShortDescription() | setShortDescription(String shortDescription) |
| `LongDescription` | `String` | Optional | The long description of the code.<br><br>**Constraints**: *Maximum Length*: `255` | String getLongDescription() | setLongDescription(String longDescription) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "code": "BD",
  "longDescription": "long description",
  "shortDescription": "shortDescription2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

