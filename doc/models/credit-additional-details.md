
# Credit Additional Details

Provides additional details on the credit transaction.

*This model accepts additional fields of type Object.*

## Structure

`CreditAdditionalDetails`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `HasAdjustmentRecords` | `String` | Optional | Refers to any adjustment made in the records.<br><br>**Constraints**: *Maximum Length*: `1` | String getHasAdjustmentRecords() | setHasAdjustmentRecords(String hasAdjustmentRecords) |
| `ForcePost` | `Boolean` | Optional | Possible values are True or False. | Boolean getForcePost() | setForcePost(Boolean forcePost) |
| `AirlineInvoiceNumber` | `String` | Optional | Unique identifier for the airline invoice billing transactions.<br><br>**Constraints**: *Maximum Length*: `14` | String getAirlineInvoiceNumber() | setAirlineInvoiceNumber(String airlineInvoiceNumber) |
| `AirlineTicketNumber` | `String` | Optional | Unique identifier for the airline ticket billing transactions.<br><br>**Constraints**: *Maximum Length*: `25` | String getAirlineTicketNumber() | setAirlineTicketNumber(String airlineTicketNumber) |
| `AirlineDepartureDate` | `LocalDate` | Optional | The scheduled day a flight leaves. | LocalDate getAirlineDepartureDate() | setAirlineDepartureDate(LocalDate airlineDepartureDate) |
| `UnmatchedCredit` | `Boolean` | Optional | Indicates funds without corresponding transaction records in the accounts. Possible values are true or false. | Boolean getUnmatchedCredit() | setUnmatchedCredit(Boolean unmatchedCredit) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "forcePost": true,
  "airlineInvoiceNumber": "A12GB2314234G1",
  "airlineTicketNumber": "IN9854GBFDTA12GB2314234G1",
  "airlineDepartureDate": "2024-03-16",
  "unmatchedCredit": true,
  "hasAdjustmentRecords": "hasAdjustmentRecords2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

