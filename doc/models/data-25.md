
# Data 25

## Structure

`Data25`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AccountHolderName` | `String` | Optional | Account holder name<br><br>> For CC, this is the 'Name (as it appears) on Card'. For ACH, this is the 'Name on Account'.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `32` | String getAccountHolderName() | setAccountHolderName(String accountHolderName) |
| `AccountVaultApiId` | `String` | Optional | This field can be used to correlate Tokens in our system to data within an outside software integration<br><br>> Must be unique per location. When running a transaction and using a stored token, this field can be used in place of account_vault_id.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `64` | String getAccountVaultApiId() | setAccountVaultApiId(String accountVaultApiId) |
| `TokenApiId` | `String` | Optional | This field can be used to correlate Tokens in our system to data within an outside software integration<br><br>> Must be unique per location. When running a transaction and using a stored token, this field can be used in place of token_id.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `64` | String getTokenApiId() | setTokenApiId(String tokenApiId) |
| `AccountvaultC1` | `String` | Optional | DEPRECATED (Use token_c1 instead)<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `128` | String getAccountvaultC1() | setAccountvaultC1(String accountvaultC1) |
| `AccountvaultC2` | `String` | Optional | DEPRECATED (Use token_c2 instead)<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `128` | String getAccountvaultC2() | setAccountvaultC2(String accountvaultC2) |
| `AccountvaultC3` | `String` | Optional | DEPRECATED (Use token_c3 instead)<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `128` | String getAccountvaultC3() | setAccountvaultC3(String accountvaultC3) |
| `TokenC1` | `String` | Optional | Custom field 1 for API users to store custom data<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `128` | String getTokenC1() | setTokenC1(String tokenC1) |
| `TokenC2` | `String` | Optional | Custom field 2 for API users to store custom data<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `128` | String getTokenC2() | setTokenC2(String tokenC2) |
| `TokenC3` | `String` | Optional | Custom field 3 for API users to store custom data<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `128` | String getTokenC3() | setTokenC3(String tokenC3) |
| `AchSecCode` | [`AchSecCode3Enum`](../../doc/models/ach-sec-code-3-enum.md) | Optional | SEC code for the account | AchSecCode3Enum getAchSecCode() | setAchSecCode(AchSecCode3Enum achSecCode) |
| `BillingAddress` | [`BillingAddress`](../../doc/models/billing-address.md) | Optional | Billing Address Object | BillingAddress getBillingAddress() | setBillingAddress(BillingAddress billingAddress) |
| `ContactId` | `String` | Optional | Used to associate the Token with a Contact.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getContactId() | setContactId(String contactId) |
| `CustomerId` | `String` | Optional | Used to store a customer identification number.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `50` | String getCustomerId() | setCustomerId(String customerId) |
| `IdentityVerification` | [`IdentityVerification2`](../../doc/models/identity-verification-2.md) | Optional | Identity verification | IdentityVerification2 getIdentityVerification() | setIdentityVerification(IdentityVerification2 identityVerification) |
| `LocationId` | `String` | Optional | A valid Location Id associated with the Contact for this Token<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `PreviousAccountVaultApiId` | `String` | Optional | Can be used to pull payment info from a previous token api id.<br><br>**Constraints**: *Maximum Length*: `64` | String getPreviousAccountVaultApiId() | setPreviousAccountVaultApiId(String previousAccountVaultApiId) |
| `PreviousTokenApiId` | `String` | Optional | Can be used to pull payment info from a previous token api id.<br><br>**Constraints**: *Maximum Length*: `64` | String getPreviousTokenApiId() | setPreviousTokenApiId(String previousTokenApiId) |
| `PreviousAccountVaultId` | `String` | Optional | Can be used to pull payment info from a previous token.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getPreviousAccountVaultId() | setPreviousAccountVaultId(String previousAccountVaultId) |
| `PreviousTokenId` | `String` | Optional | Can be used to pull payment info from a previous token.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getPreviousTokenId() | setPreviousTokenId(String previousTokenId) |
| `PreviousTransactionId` | `String` | Optional | Can be used to pull payment info from a previous transaction.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getPreviousTransactionId() | setPreviousTransactionId(String previousTransactionId) |
| `AccountNumber` | `String` | Optional | Account number<br><br>> For CC transactions, a credit card number. For ACH transactions, a bank account number. String lengths are conditional, CC should be 13-19 and ACH should be 4-19.<br><br>**Constraints**: *Minimum Length*: `4`, *Maximum Length*: `19`, *Pattern*: `^[\d]+$` | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `TermsAgree` | `Boolean` | Optional | Terms agreement. | Boolean getTermsAgree() | setTermsAgree(Boolean termsAgree) |
| `TermsAgreeIp` | `String` | Optional | The ip address of the client that agreed to terms. | String getTermsAgreeIp() | setTermsAgreeIp(String termsAgreeIp) |
| `Title` | `String` | Optional | Used to describe the Token for easier identification within our UI.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `16` | String getTitle() | setTitle(String title) |
| `TokenImportId` | `String` | Optional | Token Import Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getTokenImportId() | setTokenImportId(String tokenImportId) |
| `SecureDirectoryServerTransactionId` | `String` | Optional | (ECOMM) Directory Server Transaction ID (Such as XID, TAVV) | String getSecureDirectoryServerTransactionId() | setSecureDirectoryServerTransactionId(String secureDirectoryServerTransactionId) |
| `SecureProtocolVersion` | `Integer` | Optional | (ECOMM)  Secure Program Protocol Version | Integer getSecureProtocolVersion() | setSecureProtocolVersion(Integer secureProtocolVersion) |
| `SecureAuthData` | `String` | Optional | (ECOMM) The token authentication value associated with 3D secure transactions (Such as CAVV, UCAF auth data) | String getSecureAuthData() | setSecureAuthData(String secureAuthData) |
| `SecureCollectionIndicator` | `Integer` | Optional | (ECOMM) Used for UCAF collection indicator or Discover Autentication type | Integer getSecureCollectionIndicator() | setSecureCollectionIndicator(Integer secureCollectionIndicator) |
| `ThreeDsServerTransId` | `String` | Optional | 3DS Server Transaction ID.  If this field is sent and 3DS authentication was done with Fortis, the 3DS fields secure_directory_server_transaction_id, secure_protocol_version, and secure_collection_indicator will be pre-populated. | String getThreeDsServerTransId() | setThreeDsServerTransId(String threeDsServerTransId) |
| `AcsTransactionId` | `String` | Optional | ACS Transaction ID<br><br>**Constraints**: *Maximum Length*: `36` | String getAcsTransactionId() | setAcsTransactionId(String acsTransactionId) |
| `Joi` | [`Joi4`](../../doc/models/joi-4.md) | Optional | - | Joi4 getJoi() | setJoi(Joi4 joi) |
| `Id` | `String` | Optional | A unique, system-generated identifier for the Token.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `AccountType` | `String` | Optional | Account type<br><br>> For ACH, must be provided as either 'checking' or 'savings'. For CC, field is read only. System will identify card_type and generate a value for this field automatically. i.e. visa, mc, disc, amex, jcb, diners.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `32` | String getAccountType() | setAccountType(String accountType) |
| `Active` | `Boolean` | Optional | Register is Active | Boolean getActive() | setActive(Boolean active) |
| `CauSummaryStatusId` | [`CauSummaryStatusIdEnum`](../../doc/models/cau-summary-status-id-enum.md) | Optional | CAU Summary Status ID. | CauSummaryStatusIdEnum getCauSummaryStatusId() | setCauSummaryStatusId(CauSummaryStatusIdEnum cauSummaryStatusId) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ESerialNumber` | `String` | Optional | E Serial Number<br><br>**Constraints**: *Maximum Length*: `36`, *Pattern*: `^[a-zA-Z0-9]*$` | String getESerialNumber() | setESerialNumber(String eSerialNumber) |
| `ETrackData` | `String` | Optional | E Track Data | String getETrackData() | setETrackData(String eTrackData) |
| `EFormat` | `String` | Optional | E Format | String getEFormat() | setEFormat(String eFormat) |
| `EKeyedData` | `String` | Optional | E Keyed Data | String getEKeyedData() | setEKeyedData(String eKeyedData) |
| `ExpiringInMonths` | `Integer` | Optional | Determined by API based on card exp_date. | Integer getExpiringInMonths() | setExpiringInMonths(Integer expiringInMonths) |
| `ExpDate` | `String` | Optional | Required for CC. The Expiration Date for the credit card. (MMYY format).<br><br>**Constraints**: *Maximum Length*: `4` | String getExpDate() | setExpDate(String expDate) |
| `FirstSix` | `String` | Optional | The first six numbers of an account number.  System will generate a value for this field automatically.<br><br>**Constraints**: *Maximum Length*: `6` | String getFirstSix() | setFirstSix(String firstSix) |
| `HasRecurring` | `Boolean` | Optional | True indicates that this token is tied to a Recurring Payment | Boolean getHasRecurring() | setHasRecurring(Boolean hasRecurring) |
| `LastFour` | `String` | Optional | The last four numbers of an account number.  System will generate a value for this field automatically.<br><br>**Constraints**: *Maximum Length*: `4` | String getLastFour() | setLastFour(String lastFour) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `PaymentMethod` | [`PaymentMethod16Enum`](../../doc/models/payment-method-16-enum.md) | Optional | Must be provided as either 'cc' or 'ach'. | PaymentMethod16Enum getPaymentMethod() | setPaymentMethod(PaymentMethod16Enum paymentMethod) |
| `Ticket` | `String` | Optional | A valid ticket that was created to store the token.<br><br>**Constraints**: *Maximum Length*: `36` | String getTicket() | setTicket(String ticket) |
| `TrackData` | `String` | Optional | Track Data from a magnetic card swipe.<br><br>**Constraints**: *Maximum Length*: `256` | String getTrackData() | setTrackData(String trackData) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `CauLastUpdatedTs` | `Integer` | Optional | CAU Last Updated Timestamp | Integer getCauLastUpdatedTs() | setCauLastUpdatedTs(Integer cauLastUpdatedTs) |
| `CardBin` | `String` | Optional | Card bin | String getCardBin() | setCardBin(String cardBin) |
| `RoutingNumber` | `String` | Optional | Required for ACH. The Routing Number for the bank account being used. | String getRoutingNumber() | setRoutingNumber(String routingNumber) |
| `Location` | [`Location`](../../doc/models/location.md) | Optional | Location Information on `expand` | Location getLocation() | setLocation(Location location) |
| `Contact` | [`Contact1`](../../doc/models/contact-1.md) | Optional | Contact Information on `expand` | Contact1 getContact() | setContact(Contact1 contact) |
| `Transactions` | [`List<Transaction>`](../../doc/models/transaction.md) | Optional | Transaction Information on `expand` | List<Transaction> getTransactions() | setTransactions(List<Transaction> transactions) |
| `ActiveRecurrings` | [`List<ActiveRecurring>`](../../doc/models/active-recurring.md) | Optional | ActiveRecurring Information on `expand` | List<ActiveRecurring> getActiveRecurrings() | setActiveRecurrings(List<ActiveRecurring> activeRecurrings) |
| `IsDeletable` | `Boolean` | Optional | Is Deletable Information on `expand` | Boolean getIsDeletable() | setIsDeletable(Boolean isDeletable) |
| `Signature` | [`Signature`](../../doc/models/signature.md) | Optional | Signature Information on `expand` | Signature getSignature() | setSignature(Signature signature) |
| `CreatedUser` | [`CreatedUser`](../../doc/models/created-user.md) | Optional | User Information on `expand` | CreatedUser getCreatedUser() | setCreatedUser(CreatedUser createdUser) |
| `Changelogs` | [`List<Changelog>`](../../doc/models/changelog.md) | Optional | Changelog Information on `expand` | List<Changelog> getChangelogs() | setChangelogs(List<Changelog> changelogs) |
| `AccountVaultCauLogs` | [`List<AccountVaultCauLog>`](../../doc/models/account-vault-cau-log.md) | Optional | Token Cau Log Information on `expand` | List<AccountVaultCauLog> getAccountVaultCauLogs() | setAccountVaultCauLogs(List<AccountVaultCauLog> accountVaultCauLogs) |
| `AccountVaultCauProductTransactions` | [`List<AccountVaultCauProductTransaction>`](../../doc/models/account-vault-cau-product-transaction.md) | Optional | Token Cau Product Transaction Information on `expand` | List<AccountVaultCauProductTransaction> getAccountVaultCauProductTransactions() | setAccountVaultCauProductTransactions(List<AccountVaultCauProductTransaction> accountVaultCauProductTransactions) |

## Example (as JSON)

```json
{
  "account_holder_name": "John Smith",
  "account_vault_api_id": "accountvaultabcd",
  "token_api_id": "tokenabcd",
  "accountvault_c1": "accountvault custom 1",
  "accountvault_c2": "accountvault custom 2",
  "accountvault_c3": "accountvault custom 3",
  "token_c1": "token custom 1",
  "token_c2": "token custom 2",
  "token_c3": "token custom 3",
  "ach_sec_code": "WEB",
  "contact_id": "11e95f8ec39de8fbdb0a4f1a",
  "customer_id": "123456",
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "previous_account_vault_api_id": "previousaccountvault123456",
  "previous_token_api_id": "previousaccountvault123456",
  "previous_account_vault_id": "11e95f8ec39de8fbdb0a4f1a",
  "previous_token_id": "11e95f8ec39de8fbdb0a4f1a",
  "previous_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "account_number": "545454545454545",
  "terms_agree": true,
  "terms_agree_ip": "192.168.0.10",
  "title": "Test CC Account",
  "token_import_id": "11e95f8ec39de8fbdb0a4f1a",
  "secure_directory_server_transaction_id": "d65e93c3-35ab-41ba-b307-767bfc19eae",
  "secure_protocol_version": 2,
  "secure_auth_data": "vVwL7UNHCf8W8M2LAfvRChNHN7c%3D",
  "three_ds_server_trans_id": "d65e93c3-35ab-41ba-b307-767bfc19eae",
  "acs_transaction_id": "13c701a3-5a88-4c45-89e9-ef65e50a8bf9",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "account_type": "checking",
  "active": true,
  "cau_summary_status_id": 1,
  "created_ts": 1422040992,
  "e_serial_number": "1234567890",
  "exp_date": "0722",
  "first_six": "700953",
  "has_recurring": false,
  "last_four": "3657",
  "modified_ts": 1422040992,
  "payment_method": "cc",
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "cau_last_updated_ts": 1422040992,
  "routing_number": "051904524",
  "is_deletable": true
}
```

