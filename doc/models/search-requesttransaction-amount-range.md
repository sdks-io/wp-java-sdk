
# Search Requesttransaction Amount Range

Used for transaction amount range.

*This model accepts additional fields of type Object.*

## Structure

`SearchRequesttransactionAmountRange`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `FromAmount` | `Double` | Optional | The lowest transaction value in the search range.<br><br>**Constraints**: `>= 0`, `<= 9999999999999.99` | Double getFromAmount() | setFromAmount(Double fromAmount) |
| `ToAmount` | `Double` | Optional | The highest transaction value in the search range.<br><br>**Constraints**: `>= 0`, `<= 9999999999999.99` | Double getToAmount() | setToAmount(Double toAmount) |
| `AuthorizationCurrencyCode` | `String` | Optional | The alpha codes and numeric codes for the representation of currencies and provides information about the relationships between individual currencies and their minor units. ISO Standard country code for United States. <br> Applicable for credit and gift cards.<br><br>**Constraints**: *Maximum Length*: `3` | String getAuthorizationCurrencyCode() | setAuthorizationCurrencyCode(String authorizationCurrencyCode) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "fromAmount": 5000.89,
  "toAmount": 120000.86,
  "authorizationCurrencyCode": "authorizationCurrencyCode6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

