
# Sort Results by 2

*This model accepts additional fields of type Object.*

## Structure

`SortResultsBy2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `FieldName` | [`FieldName2`](../../doc/models/field-name-2.md) | Optional | - | FieldName2 getFieldName() | setFieldName(FieldName2 fieldName) |
| `OrderBy` | [`OrderBy`](../../doc/models/order-by.md) | Optional | - | OrderBy getOrderBy() | setOrderBy(OrderBy orderBy) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "fieldName": "PROCESS_DATE",
  "orderBy": "ASC",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

