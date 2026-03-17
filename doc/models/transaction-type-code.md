
# Transaction Type Code

The codes for the type of transactions.

*This model accepts additional fields of type Object.*

## Structure

`TransactionTypeCode`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Code` | `String` | Optional | The code of the transaction type.<br><br>**Constraints**: *Maximum Length*: `3` | String getCode() | setCode(String code) |
| `ShortDescription` | `String` | Optional | The short description of the transaction type.<br><br>**Constraints**: *Maximum Length*: `255` | String getShortDescription() | setShortDescription(String shortDescription) |
| `LongDescription` | `String` | Optional | The long description of the transaction type.<br><br>**Constraints**: *Maximum Length*: `255` | String getLongDescription() | setLongDescription(String longDescription) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "code": "GAX",
  "shortDescription": "Actvn Revsl",
  "longDescription": "Activation Reversal",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

