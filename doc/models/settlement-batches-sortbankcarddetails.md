
# Settlement Batches Sortbankcarddetails

Used for sorting.

*This model accepts additional fields of type Object.*

## Structure

`SettlementBatchesSortbankcarddetails`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `FieldName` | [`FieldName3`](../../doc/models/field-name-3.md) | Optional | - | FieldName3 getFieldName() | setFieldName(FieldName3 fieldName) |
| `OrderBy` | [`OrderBy`](../../doc/models/order-by.md) | Optional | - | OrderBy getOrderBy() | setOrderBy(OrderBy orderBy) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "fieldName": "SALE_AMOUNT",
  "orderBy": "ASC",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

