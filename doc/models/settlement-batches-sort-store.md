
# Settlement Batches Sort Store

Used for sorting.

*This model accepts additional fields of type Object.*

## Structure

`SettlementBatchesSortStore`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `FieldName` | [`FieldName2`](../../doc/models/field-name-2.md) | Optional | - | FieldName2 getFieldName() | setFieldName(FieldName2 fieldName) |
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

