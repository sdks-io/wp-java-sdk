
# Date Range 1

*This model accepts additional fields of type Object.*

## Structure

`DateRange1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `FromDate` | `LocalDate` | Optional | The starting date of the particular time period. | LocalDate getFromDate() | setFromDate(LocalDate fromDate) |
| `ToDate` | `LocalDate` | Optional | The end date of the particular time period. | LocalDate getToDate() | setToDate(LocalDate toDate) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "fromDate": "2021-12-01",
  "toDate": "2021-12-01",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

