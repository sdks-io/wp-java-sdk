
# Pagination

*This model accepts additional fields of type Object.*

## Structure

`Pagination`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PageNumber` | `Integer` | Optional | The number of the specific page you want to retrieve. <br> The default is page number 0.<br><br>**Default**: `0`<br><br>**Constraints**: `<= 16777215` | Integer getPageNumber() | setPageNumber(Integer pageNumber) |
| `PageSize` | `Integer` | Optional | The number of records that you would want to retrieve per page. <br> The default is 25 items per page.<br><br>**Default**: `25`<br><br>**Constraints**: `<= 2000` | Integer getPageSize() | setPageSize(Integer pageSize) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "pageNumber": 2,
  "pageSize": 10,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

