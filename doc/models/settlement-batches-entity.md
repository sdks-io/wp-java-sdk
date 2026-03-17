
# Settlement Batches Entity

The merchant hierarchy details.

*This model accepts additional fields of type Object.*

## Structure

`SettlementBatchesEntity`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Level` | [`Level2`](../../doc/models/level-2.md) | Optional | **Constraints**: *Maximum Length*: `8` | Level2 getLevel() | setLevel(Level2 level) |
| `Values` | `List<String>` | Optional | The values of hierarchy levels.<br><br>**Constraints**: *Maximum Items*: `2000` | List<String> getValues() | setValues(List<String> values) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "level": "MERCHANT",
  "values": [
    "values4"
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

