
# Credit Transaction Details

Provides transaction amount related information.

*This model accepts additional fields of type Object.*

## Structure

`CreditTransactionDetails`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TransactionId` | `String` | Optional | The unique 12-19 digit identifier that is generated with every card transaction and from the electronic transfer of funds.<br><br>**Constraints**: *Maximum Length*: `19` | String getTransactionId() | setTransactionId(String transactionId) |
| `ProcessDate` | `LocalDate` | Optional | Refers to the date when the transaction has been processed for settlement between the two parties. | LocalDate getProcessDate() | setProcessDate(LocalDate processDate) |
| `TransactionDateTime` | `LocalDateTime` | Optional | Refers to the date and time when the bank has settled the transaction (deposits or withdraws funds). | LocalDateTime getTransactionDateTime() | setTransactionDateTime(LocalDateTime transactionDateTime) |
| `AuthorizationAmount` | `Double` | Optional | The approved amount of money to be charged.<br><br>**Constraints**: `>= 0`, `<= 99999999.99` | Double getAuthorizationAmount() | setAuthorizationAmount(Double authorizationAmount) |
| `ApprovedAmount` | `Double` | Optional | The agreed upon sum for a transaction after authorization and processing steps.<br><br>**Constraints**: `>= 0`, `<= 99999999.99` | Double getApprovedAmount() | setApprovedAmount(Double approvedAmount) |
| `AuthorizationCode` | `String` | Optional | The six number code from the issuing bank to the vendor that authorizes the sale.<br><br>**Constraints**: *Maximum Length*: `6` | String getAuthorizationCode() | setAuthorizationCode(String authorizationCode) |
| `AuthorizationCurrency` | [`AuthorizationCurrency`](../../doc/models/authorization-currency.md) | Optional | - | AuthorizationCurrency getAuthorizationCurrency() | setAuthorizationCurrency(AuthorizationCurrency authorizationCurrency) |
| `AuthorizationSource` | [`AuthorizationSource`](../../doc/models/authorization-source.md) | Optional | - | AuthorizationSource getAuthorizationSource() | setAuthorizationSource(AuthorizationSource authorizationSource) |
| `TransactionType` | [`TransactionType`](../../doc/models/transaction-type.md) | Optional | - | TransactionType getTransactionType() | setTransactionType(TransactionType transactionType) |
| `TransactionStatus` | [`TransactionStatus`](../../doc/models/transaction-status.md) | Optional | - | TransactionStatus getTransactionStatus() | setTransactionStatus(TransactionStatus transactionStatus) |
| `EntryMode` | [`EntryMode`](../../doc/models/entry-mode.md) | Optional | - | EntryMode getEntryMode() | setEntryMode(EntryMode entryMode) |
| `AvsResponseCode` | [`AvsResponseCode`](../../doc/models/avs-response-code.md) | Optional | - | AvsResponseCode getAvsResponseCode() | setAvsResponseCode(AvsResponseCode avsResponseCode) |
| `CardholderId` | [`CardholderId`](../../doc/models/cardholder-id.md) | Optional | - | CardholderId getCardholderId() | setCardholderId(CardholderId cardholderId) |
| `SequenceNumber` | `String` | Optional | Te unique order identifier indicating the transaction or event sequence.<br><br>**Constraints**: *Maximum Length*: `6` | String getSequenceNumber() | setSequenceNumber(String sequenceNumber) |
| `AuthorizationIdentifier` | `String` | Optional | The ecommerce authorization identifier.<br><br>**Constraints**: *Maximum Length*: `36` | String getAuthorizationIdentifier() | setAuthorizationIdentifier(String authorizationIdentifier) |
| `CustomerIdentifier` | `String` | Optional | The unique identifier of the purchaser associated with the transaction.<br><br>**Constraints**: *Maximum Length*: `50` | String getCustomerIdentifier() | setCustomerIdentifier(String customerIdentifier) |
| `MerchantOrderIdentifier` | `String` | Optional | The merchant-designated identifier for this transaction.<br><br>**Constraints**: *Maximum Length*: `25` | String getMerchantOrderIdentifier() | setMerchantOrderIdentifier(String merchantOrderIdentifier) |
| `Campaign` | `String` | Optional | The merchant-specified identifier used to track transactions associated with specific marketing campaigns.<br><br>**Constraints**: *Maximum Length*: `25` | String getCampaign() | setCampaign(String campaign) |
| `Affiliate` | `String` | Optional | The merchant-specified identifier used to track transactions associated with your affiliate organizations.<br><br>**Constraints**: *Maximum Length*: `25` | String getAffiliate() | setAffiliate(String affiliate) |
| `MerchantGroupingIdentifier` | `String` | Optional | The merchant-specified identifier for grouping transactions by an additional transaction level id outside of affiliate or campaign.<br><br>**Constraints**: *Maximum Length*: `25` | String getMerchantGroupingIdentifier() | setMerchantGroupingIdentifier(String merchantGroupingIdentifier) |
| `ReportGroup` | `String` | Optional | The reporting group category to which the transaction belongs.<br><br>**Constraints**: *Maximum Length*: `25` | String getReportGroup() | setReportGroup(String reportGroup) |
| `Aci` | [`Aci`](../../doc/models/aci.md) | Optional | - | Aci getAci() | setAci(Aci aci) |
| `MailPhoneIndicator` | [`MailPhoneIndicator`](../../doc/models/mail-phone-indicator.md) | Optional | - | MailPhoneIndicator getMailPhoneIndicator() | setMailPhoneIndicator(MailPhoneIndicator mailPhoneIndicator) |
| `OriginType` | [`OriginType`](../../doc/models/origin-type.md) | Optional | - | OriginType getOriginType() | setOriginType(OriginType originType) |
| `ValidationCode` | `String` | Optional | The validation code for Visa card network transactions.<br><br>**Constraints**: *Maximum Length*: `4` | String getValidationCode() | setValidationCode(String validationCode) |
| `PosRegisterNumber` | `String` | Optional | The unique identifier assigned to a point-of-sale terminal for tracking transactions and managing sales data.<br><br>**Constraints**: *Maximum Length*: `4` | String getPosRegisterNumber() | setPosRegisterNumber(String posRegisterNumber) |
| `TerminalNumber` | `String` | Optional | The eight-digit sequence of characters used by financial institutions to monitor which terminal is used to process a transaction.<br><br>**Constraints**: *Maximum Length*: `20` | String getTerminalNumber() | setTerminalNumber(String terminalNumber) |
| `ReferenceNumber` | `String` | Optional | The key to uniquely identify a card transaction based on the ISO 8583 standard.<br><br>**Constraints**: *Maximum Length*: `23` | String getReferenceNumber() | setReferenceNumber(String referenceNumber) |
| `DraftLocator` | `String` | Optional | The merchant reference or draft locator number.<br><br>**Constraints**: *Maximum Length*: `11` | String getDraftLocator() | setDraftLocator(String draftLocator) |
| `TerminalCapability` | [`TerminalCapability`](../../doc/models/terminal-capability.md) | Optional | - | TerminalCapability getTerminalCapability() | setTerminalCapability(TerminalCapability terminalCapability) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "transactionId": "141715459519",
  "processDate": "2022-06-16",
  "authorizationAmount": 100.04,
  "approvedAmount": 29.04,
  "authorizationCode": "73994M",
  "sequenceNumber": "34",
  "authorizationIdentifier": "6T78",
  "customerIdentifier": "G768",
  "merchantOrderIdentifier": "A453",
  "campaign": "D453",
  "affiliate": "G123",
  "merchantGroupingIdentifier": "1098675",
  "reportGroup": "E874",
  "validationCode": "TN2S",
  "posRegisterNumber": "0050",
  "terminalNumber": "D0640450",
  "referenceNumber": "2444677778440029",
  "draftLocator": "65678787979",
  "transactionDateTime": "2016-03-13T12:52:32.123Z",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

