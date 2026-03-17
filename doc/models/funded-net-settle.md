
# Funded Net Settle

Funded transaction reconciliation process for net balance finalization.

*This model accepts additional fields of type Object.*

## Structure

`FundedNetSettle`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ProcessorAmount` | `Double` | Optional | The final funds transferred to merchant accounts after processing fees deductions.<br><br>**Constraints**: `>= 0`, `<= 9999999999999.99` | Double getProcessorAmount() | setProcessorAmount(Double processorAmount) |
| `ProcessorCount` | `Integer` | Optional | The payment method based on processing capacity for settlements.<br><br>**Constraints**: `<= 9999` | Integer getProcessorCount() | setProcessorCount(Integer processorCount) |
| `OtherAmount` | `Double` | Optional | The final transaction balance after deducting external funding sources.<br><br>**Constraints**: `>= 0`, `<= 9999999999999.99` | Double getOtherAmount() | setOtherAmount(Double otherAmount) |
| `OtherCount` | `Integer` | Optional | The amount of financial transactions settled through external sources.<br><br>**Constraints**: `<= 9999` | Integer getOtherCount() | setOtherCount(Integer otherCount) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "processorAmount": 29.04,
  "processorCount": 2,
  "otherAmount": 29.04,
  "otherCount": 14,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

