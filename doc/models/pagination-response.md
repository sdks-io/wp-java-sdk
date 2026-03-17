
# Pagination Response

The format used to display your resources.

*This model accepts additional fields of type Object.*

## Structure

`PaginationResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PageNumber` | `Integer` | Optional | The current page number returned.<br><br>**Default**: `0`<br><br>**Constraints**: `<= 16777215` | Integer getPageNumber() | setPageNumber(Integer pageNumber) |
| `PageSize` | `Integer` | Optional | The number of records that you would want to retrieve per page.<br><br>**Default**: `25`<br><br>**Constraints**: `<= 2000` | Integer getPageSize() | setPageSize(Integer pageSize) |
| `TotalRowCount` | `Integer` | Optional | The total number of result rows returned.<br><br>**Constraints**: `<= 9999` | Integer getTotalRowCount() | setTotalRowCount(Integer totalRowCount) |
| `TotalReturnedCount` | `Integer` | Optional | The total number of records returned.<br><br>**Constraints**: `<= 2000` | Integer getTotalReturnedCount() | setTotalReturnedCount(Integer totalReturnedCount) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "pageNumber": 0,
  "pageSize": 50,
  "totalRowCount": 45,
  "totalReturnedCount": 25,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

