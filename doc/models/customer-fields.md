
# Customer Fields

The customer details.

*This model accepts additional fields of type Object.*

## Structure

`CustomerFields`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Field1` | `String` | Optional | Field one for the customer details.<br><br>**Constraints**: *Maximum Length*: `35` | String getField1() | setField1(String field1) |
| `Field2` | `String` | Optional | Field two for the customer details.<br><br>**Constraints**: *Maximum Length*: `20` | String getField2() | setField2(String field2) |
| `Field3` | `String` | Optional | Field three for the customer details.<br><br>**Constraints**: *Maximum Length*: `20` | String getField3() | setField3(String field3) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "field1": "GC",
  "field2": "RealTime",
  "field3": "Report",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

