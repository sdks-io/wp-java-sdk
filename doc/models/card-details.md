
# Card Details

The details of card used for the transaction.

*This model accepts additional fields of type Object.*

## Structure

`CardDetails`

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
| `CardAccountTerm` | [`CardAccountTerm`](../../doc/models/card-account-term.md) | Optional | - | CardAccountTerm getCardAccountTerm() | setCardAccountTerm(CardAccountTerm cardAccountTerm) |
| `CardholderBankAcro` | `String` | Optional | The acronym for the primary user of a payment card.<br><br>**Constraints**: *Maximum Length*: `4` | String getCardholderBankAcro() | setCardholderBankAcro(String cardholderBankAcro) |
| `TokenRequestorId` | `String` | Optional | The unique identifier used to request network tokens from the card networks.<br><br>**Constraints**: *Maximum Length*: `11` | String getTokenRequestorId() | setTokenRequestorId(String tokenRequestorId) |
| `BankNetDate` | `LocalDate` | Optional | The payments network operated by Mastercard. The value is present only if the transaction is Mastercard, otherwise it's null. | LocalDate getBankNetDate() | setBankNetDate(LocalDate bankNetDate) |
| `BankNetReferenceNumber` | `String` | Optional | The unique identifier for transactions processed through banknet systems.<br><br>**Constraints**: *Maximum Length*: `9` | String getBankNetReferenceNumber() | setBankNetReferenceNumber(String bankNetReferenceNumber) |
| `MarketSpecificDataIndicator` | [`MarketSpecificDataIndicator`](../../doc/models/market-specific-data-indicator.md) | Optional | - | MarketSpecificDataIndicator getMarketSpecificDataIndicator() | setMarketSpecificDataIndicator(MarketSpecificDataIndicator marketSpecificDataIndicator) |
| `DccMcpIndicator` | `String` | Optional | Provides dynamic currency conversion information to the merchant. Applicable for credit (master credit card).<br><br>**Constraints**: *Maximum Length*: `1` | String getDccMcpIndicator() | setDccMcpIndicator(String dccMcpIndicator) |
| `LastFourOfPan` | `String` | Optional | The last four digits of the PAN on the receipt.<br><br>**Constraints**: *Maximum Length*: `4` | String getLastFourOfPan() | setLastFourOfPan(String lastFourOfPan) |
| `VisaReversed` | `Boolean` | Optional | Indicates funds without corresponding transaction records in accounts. Possible values are true or false. | Boolean getVisaReversed() | setVisaReversed(Boolean visaReversed) |
| `VisaReversedDate` | `LocalDate` | Optional | The Visa transaction's reversed authorization date. | LocalDate getVisaReversedDate() | setVisaReversedDate(LocalDate visaReversedDate) |
| `MastercardWalletId` | `String` | Optional | The Mastercard wallet identifier.<br><br>**Constraints**: *Maximum Length*: `3` | String getMastercardWalletId() | setMastercardWalletId(String mastercardWalletId) |
| `MastercardTicIndicator` | [`MastercardTicIndicator`](../../doc/models/mastercard-tic-indicator.md) | Optional | - | MastercardTicIndicator getMastercardTicIndicator() | setMastercardTicIndicator(MastercardTicIndicator mastercardTicIndicator) |
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
  "cardholderBankAcro": "MAE1",
  "tokenRequestorId": "AZDAJAKAYHE",
  "dccMcpIndicator": "Y",
  "lastFourOfPAN": "3245",
  "visaReversed": false,
  "visaReversedDate": "2022-06-16",
  "mastercardWalletId": "DR1",
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

