
# Payment Gateway Details

The details of the payment gateway.

*This model accepts additional fields of type Object.*

## Structure

`PaymentGatewayDetails`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PosApplicationId` | `String` | Optional | The unique identifier for a point-of-sale application used in transactions.<br><br>**Constraints**: *Maximum Length*: `6` | String getPosApplicationId() | setPosApplicationId(String posApplicationId) |
| `PosApplicationName` | `String` | Optional | The name given to a point-of-sale system.<br><br>**Constraints**: *Maximum Length*: `50` | String getPosApplicationName() | setPosApplicationName(String posApplicationName) |
| `PosApplicationVersion` | `String` | Optional | The specific version of the point-of-sale software.<br><br>**Constraints**: *Maximum Length*: `50` | String getPosApplicationVersion() | setPosApplicationVersion(String posApplicationVersion) |
| `GatewayTransactionId` | `String` | Optional | The unique identifier for quick and efficient tracking and processing of a transaction.<br><br>**Constraints**: *Maximum Length*: `20` | String getGatewayTransactionId() | setGatewayTransactionId(String gatewayTransactionId) |
| `PaymentReferenceNumber` | `Object` | Optional | Payment Account Reference (PAR) number is a unique identifier assigned to a cardholder’s payment account. | Object getPaymentReferenceNumber() | setPaymentReferenceNumber(Object paymentReferenceNumber) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "posApplicationId": "1111",
  "posApplicationName": "Express 1",
  "posApplicationVersion": "Express.2.39.0",
  "gatewayTransactionId": "9598394756",
  "paymentReferenceNumber": {
    "key1": "val1",
    "key2": "val2"
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

