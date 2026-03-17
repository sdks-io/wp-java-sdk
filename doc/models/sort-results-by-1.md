
# Sort Results by 1

*This model accepts additional fields of type Object.*

## Structure

`SortResultsBy1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `FieldName` | [`FieldName1`](../../doc/models/field-name-1.md) | Optional | **Constraints**: *Maximum Length*: `21` | FieldName1 getFieldName() | setFieldName(FieldName1 fieldName) |
| `OrderBy` | [`OrderBy`](../../doc/models/order-by.md) | Optional | **Constraints**: *Maximum Length*: `4` | OrderBy getOrderBy() | setOrderBy(OrderBy orderBy) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "fieldName": "BATCH_NUMBER",
  "orderBy": "ASC",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

