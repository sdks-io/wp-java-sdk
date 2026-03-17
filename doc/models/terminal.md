
# Terminal

*This model accepts additional fields of type Object.*

## Structure

`Terminal`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Number` | `String` | Optional | The eight-digit sequence of characters used by financial institutions to monitor which terminal is used to process a transaction.<br><br>**Constraints**: *Maximum Length*: `20` | String getNumber() | setNumber(String number) |
| `Address` | `String` | Optional | The location identifier or address for the physical point-of-sale device or processing equipment.<br><br>**Constraints**: *Maximum Length*: `25` | String getAddress() | setAddress(String address) |
| `City` | `String` | Optional | The city where the physical point-of-sale device or processing equipment is located.<br><br>**Constraints**: *Maximum Length*: `13` | String getCity() | setCity(String city) |
| `State` | `String` | Optional | The state where the physical point-of-sale device or processing equipment is located.<br><br>**Constraints**: *Maximum Length*: `2` | String getState() | setState(String state) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "number": "D0640450",
  "address": "210 11TH ST",
  "city": "HUNTINGTON",
  "state": "WV",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

