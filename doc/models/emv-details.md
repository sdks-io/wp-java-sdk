
# Emv Details

Provides information on the EMV details.

*This model accepts additional fields of type Object.*

## Structure

`EmvDetails`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Transaction` | `Boolean` | Optional | True means the transaction is EMV. <br> False means the transaction is EMV fallback. | Boolean getTransaction() | setTransaction(Boolean transaction) |
| `OfflineTransaction` | `Boolean` | Optional | True means the transaction didn't go out to the network for authorization. <br> False means the transaction did go out to the network for authorization. | Boolean getOfflineTransaction() | setOfflineTransaction(Boolean offlineTransaction) |
| `CardCapable` | `Boolean` | Optional | True means the card is an EMV capable card. <br> False means the card is not an EMV capable card. | Boolean getCardCapable() | setCardCapable(Boolean cardCapable) |
| `TermCapable` | `Boolean` | Optional | True means the terminal is EMV capable. <br> False means the terminal is not EMV capable. | Boolean getTermCapable() | setTermCapable(Boolean termCapable) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "transaction": true,
  "offlineTransaction": true,
  "cardCapable": true,
  "termCapable": true,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

