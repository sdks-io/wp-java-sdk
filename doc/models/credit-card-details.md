
# Credit Card Details

Provides card related information.

*This model accepts additional fields of type Object.*

## Structure

`CreditCardDetails`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `CardNumber` | `String` | Optional | The number found on the card used to make a purchase, also referred to as the bank or credit card number. <br>Searches can be done on the full card number, on the first six and last four digits, or on the last four digits."<br><br>**Constraints**: *Maximum Length*: `19` | String getCardNumber() | setCardNumber(String cardNumber) |
| `CardType` | `String` | Optional | The category or classification of a payment card based on the issuing network. <br> Possible values are CREDIT, DEBIT, and GIFT.<br><br>**Constraints**: *Maximum Length*: `6` | String getCardType() | setCardType(String cardType) |
| `ExpirationDate` | `LocalDate` | Optional | The set time when a card will need to be replaced. | LocalDate getExpirationDate() | setExpirationDate(LocalDate expirationDate) |
| `CardNetwork` | [`CardNetwork`](../../doc/models/card-network.md) | Optional | - | CardNetwork getCardNetwork() | setCardNetwork(CardNetwork cardNetwork) |
| `Cvv2ResponseCode` | [`Cvv2ResponseCode`](../../doc/models/cvv-2-response-code.md) | Optional | - | Cvv2ResponseCode getCvv2ResponseCode() | setCvv2ResponseCode(Cvv2ResponseCode cvv2ResponseCode) |
| `Cvv2PresenceIndicator` | [`Cvv2PresenceIndicator`](../../doc/models/cvv-2-presence-indicator.md) | Optional | - | Cvv2PresenceIndicator getCvv2PresenceIndicator() | setCvv2PresenceIndicator(Cvv2PresenceIndicator cvv2PresenceIndicator) |
| `Token` | `String` | Optional | The numeric value that is the same length as the card number and is used as a substitution with proxy data. Max length of the token is 19 characters.<br><br>**Constraints**: *Maximum Length*: `19` | String getToken() | setToken(String token) |
| `TokenId` | `String` | Optional | The host-generated numeric value created during the tokenization process using a token key assigned to a merchant. This value is returned to the point-of-sale when tokenization is requested along with the token for utilization.<br><br>**Constraints**: *Maximum Length*: `6` | String getTokenId() | setTokenId(String tokenId) |
| `TokenAssuranceLevel` | `String` | Optional | A request and response field. The score or confidence level that determines the expected level of assurance associated with the approved token requestor and the identification and verification method performed at the time of token request.<br><br>**Constraints**: *Maximum Length*: `2` | String getTokenAssuranceLevel() | setTokenAssuranceLevel(String tokenAssuranceLevel) |
| `TokenExpirationDate` | `LocalDate` | Optional | The expiration date of the token in the YYYY-MM format with a fixed length of 6. | LocalDate getTokenExpirationDate() | setTokenExpirationDate(LocalDate tokenExpirationDate) |
| `InternationalIndicator` | [`InternationalIndicator`](../../doc/models/international-indicator.md) | Optional | - | InternationalIndicator getInternationalIndicator() | setInternationalIndicator(InternationalIndicator internationalIndicator) |
| `NetworkRejectIndicator` | `Boolean` | Optional | Possible values are true and false. | Boolean getNetworkRejectIndicator() | setNetworkRejectIndicator(Boolean networkRejectIndicator) |
| `NetworkPaymentTokenNumber` | `String` | Optional | Indentifier for digital payment transactions.<br><br>**Constraints**: *Maximum Length*: `20` | String getNetworkPaymentTokenNumber() | setNetworkPaymentTokenNumber(String networkPaymentTokenNumber) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "cardNumber": "123456XXXXXX9876",
  "cardType": "CREDIT",
  "token": "374245111181117",
  "tokenId": "A834GD",
  "tokenAssuranceLevel": "99",
  "networkRejectIndicator": true,
  "networkPaymentTokenNumber": "CD",
  "expirationDate": "2016-03-13",
  "cardNetwork": {
    "code": "code8",
    "shortDescription": "shortDescription6",
    "longDescription": "longDescription0",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "cvv2ResponseCode": {
    "code": "code8",
    "shortDescription": "shortDescription4",
    "longDescription": "longDescription0",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

