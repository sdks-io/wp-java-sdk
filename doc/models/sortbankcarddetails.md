
# Sortbankcarddetails

Used for sorting results.

*This model accepts additional fields of type Object.*

## Structure

`Sortbankcarddetails`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `FieldName` | [`FieldName5`](../../doc/models/field-name-5.md) | Optional | - | FieldName5 getFieldName() | setFieldName(FieldName5 fieldName) |
| `OrderBy` | [`OrderBy`](../../doc/models/order-by.md) | Optional | - | OrderBy getOrderBy() | setOrderBy(OrderBy orderBy) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "fieldName": "BATCH_HOLD_STATUS",
  "orderBy": "ASC",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

