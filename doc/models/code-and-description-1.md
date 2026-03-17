
# Code and Description 1

The unique identifier and the brief description.

*This model accepts additional fields of type Object.*

## Structure

`CodeAndDescription1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Code` | `String` | Optional | The identifier code.<br><br>**Constraints**: *Maximum Length*: `6` | String getCode() | setCode(String code) |
| `Description` | `String` | Optional | The description of the code.<br><br>**Constraints**: *Maximum Length*: `255` | String getDescription() | setDescription(String description) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "code": "BD",
  "description": "Description",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

