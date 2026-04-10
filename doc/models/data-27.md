
# Data 27

*This model accepts additional fields of type Object.*

## Structure

`Data27`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AdditionalAmounts` | [`List<AdditionalAmount>`](../../doc/models/additional-amount.md) | Optional | Additional amounts | List<AdditionalAmount> getAdditionalAmounts() | setAdditionalAmounts(List<AdditionalAmount> additionalAmounts) |
| `BillingAddress` | [`BillingAddress2`](../../doc/models/billing-address-2.md) | Optional | - | BillingAddress2 getBillingAddress() | setBillingAddress(BillingAddress2 billingAddress) |
| `CheckinDate` | `String` | Optional | Checkin Date - The time difference between checkin_date and checkout_date must be less than or equal to 99 days. NOTE: if checkin_date is in the future, set the advance_deposit to 1<br><br>> Required if merchant industry type is lodging.<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getCheckinDate() | setCheckinDate(String checkinDate) |
| `CheckoutDate` | `String` | Optional | Checkout Date - The time difference between checkin_date and checkout_date must be less than or equal to 99 days.<br><br>> Required if merchant industry type is lodging.<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getCheckoutDate() | setCheckoutDate(String checkoutDate) |
| `ClerkNumber` | `String` | Optional | Clerk or Employee Identifier<br><br>**Constraints**: *Maximum Length*: `16` | String getClerkNumber() | setClerkNumber(String clerkNumber) |
| `ContactApiId` | `String` | Optional | This can be supplied in place of contact_id if you would like to use a contact for the transaction and are using your own custom api_id's to track contacts in the system.<br><br>**Constraints**: *Maximum Length*: `36` | String getContactApiId() | setContactApiId(String contactApiId) |
| `ContactId` | `String` | Optional | If contact_id is provided, ensure it belongs to the same location as the transaction. You cannot move transaction across locations.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getContactId() | setContactId(String contactId) |
| `CustomData` | `Object` | Optional | A field that allows custom JSON to be entered to store extra data. | Object getCustomData() | setCustomData(Object customData) |
| `CustomerId` | `String` | Optional | Can be used by Merchants to identify Contacts in our system by an ID from another system.<br><br>**Constraints**: *Maximum Length*: `64` | String getCustomerId() | setCustomerId(String customerId) |
| `Description` | `String` | Optional | Description<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `64` | String getDescription() | setDescription(String description) |
| `IiasInd` | `Object` | Optional | - | Object getIiasInd() | setIiasInd(Object iiasInd) |
| `ImageFront` | `String` | Optional | A base64 encoded string for the image.  Used with Check21 ACH transactions. | String getImageFront() | setImageFront(String imageFront) |
| `ImageBack` | `String` | Optional | A base64 encoded string for the image.  Used with Check21 ACH transactions. | String getImageBack() | setImageBack(String imageBack) |
| `Installment` | `Boolean` | Optional | Flag that is allowed to be passed on card not present industries to signify the transaction is a fixed installment plan transaction. | Boolean getInstallment() | setInstallment(Boolean installment) |
| `InstallmentNumber` | `Integer` | Optional | If this is a fixed installment plan and installment field is being passed as 1, then this field must have a vlue of 1-999 specifying the current installment number that is running.<br><br>**Constraints**: `>= 1`, `<= 999` | Integer getInstallmentNumber() | setInstallmentNumber(Integer installmentNumber) |
| `InstallmentCount` | `Integer` | Optional | If this is a fixed installment plan and installment field is being passed as 1, then this field must have a vlue of 1-999 specifying the total number of installments on the plan. This number must be grater than or equal to installment_number.<br><br>**Constraints**: `>= 1`, `<= 999` | Integer getInstallmentCount() | setInstallmentCount(Integer installmentCount) |
| `RecurringFlag` | `Object` | Optional | - | Object getRecurringFlag() | setRecurringFlag(Object recurringFlag) |
| `InstallmentCounter` | `Integer` | Optional | Installment Counter<br><br>**Constraints**: `>= 1`, `<= 999` | Integer getInstallmentCounter() | setInstallmentCounter(Integer installmentCounter) |
| `InstallmentTotal` | `Integer` | Optional | Installment Total<br><br>**Constraints**: `>= 1`, `<= 999` | Integer getInstallmentTotal() | setInstallmentTotal(Integer installmentTotal) |
| `Subscription` | `Boolean` | Optional | Subscription | Boolean getSubscription() | setSubscription(Boolean subscription) |
| `StandingOrder` | `Boolean` | Optional | Standing Order | Boolean getStandingOrder() | setStandingOrder(Boolean standingOrder) |
| `LocationApiId` | `String` | Optional | This can be supplied in place of location_id for the transaction if you are using your own custom api_id's for your locations.<br><br>**Constraints**: *Maximum Length*: `36` | String getLocationApiId() | setLocationApiId(String locationApiId) |
| `LocationId` | `String` | Optional | A valid Location Id to associate the transaction with.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `ProductTransactionId` | `String` | Optional | The Product's method (cc/ach) has to match the action. If not provided, the API will use the default configured for the Location.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getProductTransactionId() | setProductTransactionId(String productTransactionId) |
| `AdvanceDeposit` | `Boolean` | Optional | Advance Deposit | Boolean getAdvanceDeposit() | setAdvanceDeposit(Boolean advanceDeposit) |
| `NoShow` | `Boolean` | Optional | Used in Lodging | Boolean getNoShow() | setNoShow(Boolean noShow) |
| `NotificationEmailAddress` | `String` | Optional | If email is supplied then receipt will be emailed | String getNotificationEmailAddress() | setNotificationEmailAddress(String notificationEmailAddress) |
| `OrderNumber` | `String` | Optional | Required for CC transactions , if merchant's deposit account's duplicate check per batch has 'order_number' field<br><br>**Constraints**: *Maximum Length*: `32` | String getOrderNumber() | setOrderNumber(String orderNumber) |
| `PoNumber` | `String` | Optional | Purchase Order number<br><br>**Constraints**: *Maximum Length*: `64` | String getPoNumber() | setPoNumber(String poNumber) |
| `QuickInvoiceId` | `String` | Optional | Can be used to associate a transaction to a Quick Invoice.  Quick Invoice transactions will have a value for this field automatically.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getQuickInvoiceId() | setQuickInvoiceId(String quickInvoiceId) |
| `Recurring` | [`Recurring`](../../doc/models/recurring.md) | Optional | - | Recurring getRecurring() | setRecurring(Recurring recurring) |
| `RecurringNumber` | `Integer` | Optional | If this is an ongoing recurring and recurring field is being passed as 1, then this field must have a vlue of 1-999 specifying the current recurring number that is running.<br><br>**Constraints**: `>= 1`, `<= 999` | Integer getRecurringNumber() | setRecurringNumber(Integer recurringNumber) |
| `RoomNum` | `String` | Optional | Used in Lodging<br><br>**Constraints**: *Maximum Length*: `12` | String getRoomNum() | setRoomNum(String roomNum) |
| `RoomRate` | `Integer` | Optional | Required if merchant industry type is lodging. | Integer getRoomRate() | setRoomRate(Integer roomRate) |
| `SaveAccount` | `Boolean` | Optional | Specifies to save account to contacts profile if account_number/track_data is present with either contact_id or contact_api_id in params. | Boolean getSaveAccount() | setSaveAccount(Boolean saveAccount) |
| `SaveAccountTitle` | `String` | Optional | If saving token while running a transaction, this will be the title of the token.<br><br>**Constraints**: *Maximum Length*: `16` | String getSaveAccountTitle() | setSaveAccountTitle(String saveAccountTitle) |
| `SubtotalAmount` | `Integer` | Optional | This field is allowed and required for transactions that have a product where surcharge is configured. Use only integer numbers, so $10.99 will be 1099.<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getSubtotalAmount() | setSubtotalAmount(Integer subtotalAmount) |
| `SurchargeAmount` | `Integer` | Optional | This field is allowed and required for transactions that have a product where surcharge is configured. Use only integer numbers, so $10.99 will be 1099.<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getSurchargeAmount() | setSurchargeAmount(Integer surchargeAmount) |
| `Tags` | [`List<Tag>`](../../doc/models/tag.md) | Optional | Tag Information on `expand` | List<Tag> getTags() | setTags(List<Tag> tags) |
| `Tax` | `Integer` | Optional | Amount of Sales tax - If supplied, this amount should be included in the total transaction_amount field. Use only integer numbers, so $10.99 will be 1099.<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getTax() | setTax(Integer tax) |
| `TipAmount` | `Integer` | Optional | Optional tip amount. Tip is not supported for lodging and ecommerce merchants. Use only integer numbers, so $10.99 will be 1099.<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getTipAmount() | setTipAmount(Integer tipAmount) |
| `TransactionAmount` | `Integer` | Optional | Amount of the transaction. This should always be the desired settle amount of the transaction. Use only integer numbers, so $10.99 will be 1099.<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getTransactionAmount() | setTransactionAmount(Integer transactionAmount) |
| `SecondaryAmount` | `Integer` | Optional | Retained Amount of the transaction. This should always be less than transaction amount. Use only integer numbers, so $10.99 will be 1099<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getSecondaryAmount() | setSecondaryAmount(Integer secondaryAmount) |
| `TransactionApiId` | `String` | Optional | See api_id page for more details<br><br>**Constraints**: *Maximum Length*: `64` | String getTransactionApiId() | setTransactionApiId(String transactionApiId) |
| `TransactionC1` | `String` | Optional | Custom field 1 for api users to store custom data<br><br>**Constraints**: *Maximum Length*: `128` | String getTransactionC1() | setTransactionC1(String transactionC1) |
| `TransactionC2` | `String` | Optional | Custom field 2 for api users to store custom data<br><br>**Constraints**: *Maximum Length*: `128` | String getTransactionC2() | setTransactionC2(String transactionC2) |
| `TransactionC3` | `String` | Optional | Custom field 3 for api users to store custom data<br><br>**Constraints**: *Maximum Length*: `128` | String getTransactionC3() | setTransactionC3(String transactionC3) |
| `BankFundedOnlyOverride` | `Boolean` | Optional | Bank Funded Only Override | Boolean getBankFundedOnlyOverride() | setBankFundedOnlyOverride(Boolean bankFundedOnlyOverride) |
| `AllowPartialAuthorizationOverride` | `Boolean` | Optional | Allow Partial Authorization Override | Boolean getAllowPartialAuthorizationOverride() | setAllowPartialAuthorizationOverride(Boolean allowPartialAuthorizationOverride) |
| `AutoDeclineCvvOverride` | `Boolean` | Optional | Auto Decline CVV Override | Boolean getAutoDeclineCvvOverride() | setAutoDeclineCvvOverride(Boolean autoDeclineCvvOverride) |
| `AutoDeclineStreetOverride` | `Boolean` | Optional | Auto Decline Street Override | Boolean getAutoDeclineStreetOverride() | setAutoDeclineStreetOverride(Boolean autoDeclineStreetOverride) |
| `AutoDeclineZipOverride` | `Boolean` | Optional | Auto Decline Zip Override | Boolean getAutoDeclineZipOverride() | setAutoDeclineZipOverride(Boolean autoDeclineZipOverride) |
| `EbtType` | `Object` | Optional | - | Object getEbtType() | setEbtType(Object ebtType) |
| `Id` | `String` | Optional | Transaction ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `TerminalId` | `String` | Optional | Terminal ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getTerminalId() | setTerminalId(String terminalId) |
| `AccountHolderName` | `String` | Optional | For CC, this is the 'Name (as it appears) on Card'. For ACH, this is the 'Name on Account'.<br><br>> Required for ACH transactions if account_vault_id is not provided. For CC transactions that are run through a terminal, this field may be overwritten by data acquired from the credit card track data.<br><br>**Constraints**: *Maximum Length*: `32` | String getAccountHolderName() | setAccountHolderName(String accountHolderName) |
| `AccountType` | `String` | Optional | Required for ACH transactions if account_vault_id is not provided.<br><br>> For ACH, allowed values are 'checking' or 'savings'. For CC, this field is read only. The system will identify card type and generate a value for this field automatically. possible values are: visa, mc, disc, amex, jcb, diners, and debit.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `32` | String getAccountType() | setAccountType(String accountType) |
| `TokenApiId` | `String` | Optional | This can be supplied in place of account_vault_id if you would like to use an token for the transaction and are using your own custom api_id's to track accountvaults in the system.<br><br>**Constraints**: *Maximum Length*: `36` | String getTokenApiId() | setTokenApiId(String tokenApiId) |
| `TokenId` | `String` | Optional | Required if account_number,  track_data, micr_data is not provided.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getTokenId() | setTokenId(String tokenId) |
| `AchIdentifier` | `String` | Optional | Required for ACH transactions in certain scenarios.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `1` | String getAchIdentifier() | setAchIdentifier(String achIdentifier) |
| `AchSecCode` | `Object` | Optional | - | Object getAchSecCode() | setAchSecCode(Object achSecCode) |
| `AuthAmount` | `Integer` | Optional | Authorization Amount<br><br>**Constraints**: `<= 999999999` | Integer getAuthAmount() | setAuthAmount(Integer authAmount) |
| `AuthCode` | `String` | Optional | Required on force transactions and EBT voucher clear sale/refund. Ignored for all other actions.<br><br>**Constraints**: *Minimum Length*: `6`, *Maximum Length*: `6` | String getAuthCode() | setAuthCode(String authCode) |
| `Avs` | `Object` | Optional | - | Object getAvs() | setAvs(Object avs) |
| `AvsEnhanced` | `String` | Optional | AVS Enhanced<br><br>**Constraints**: *Minimum Length*: `1` | String getAvsEnhanced() | setAvsEnhanced(String avsEnhanced) |
| `CardholderPresent` | `Boolean` | Optional | If the cardholder is present at the point of service | Boolean getCardholderPresent() | setCardholderPresent(Boolean cardholderPresent) |
| `CardPresent` | `Boolean` | Optional | A POST only field to specify whether or not the card is present.<br><br>> This field will be defaulted to '1' for all card present industries (retail, lodging, restaurant) and '0' for card not present industries (MOTO/e-commerce).<br>> For lodging, if the no_show flag is set to '1', this field will automatically be set to '0'.<br>> For transactions where account_vault_id is used, this filed will be set to '0'. | Boolean getCardPresent() | setCardPresent(Boolean cardPresent) |
| `CheckNumber` | `String` | Optional | Required for transactions using TEL SEC code.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `15` | String getCheckNumber() | setCheckNumber(String checkNumber) |
| `CustomerIp` | `String` | Optional | Can be used to store customer IP Address | String getCustomerIp() | setCustomerIp(String customerIp) |
| `CvvResponse` | `String` | Optional | Obfuscated CVV<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `1` | String getCvvResponse() | setCvvResponse(String cvvResponse) |
| `EntryModeId` | `Object` | Optional | - | Object getEntryModeId() | setEntryModeId(Object entryModeId) |
| `EmvReceiptData` | `Object` | Optional | - | Object getEmvReceiptData() | setEmvReceiptData(Object emvReceiptData) |
| `FirstSix` | `String` | Optional | First six numbers of account_number.  Automatically generated by system.<br><br>**Constraints**: *Minimum Length*: `6`, *Maximum Length*: `6` | String getFirstSix() | setFirstSix(String firstSix) |
| `LastFour` | `String` | Optional | Last four numbers of account_number.  Automatically generated by the system.<br><br>**Constraints**: *Minimum Length*: `4`, *Maximum Length*: `4` | String getLastFour() | setLastFour(String lastFour) |
| `PaymentMethod` | [`PaymentMethod9`](../../doc/models/payment-method-9.md) | Optional | - | PaymentMethod9 getPaymentMethod() | setPaymentMethod(PaymentMethod9 paymentMethod) |
| `TerminalSerialNumber` | `String` | Optional | If transaction was processed using a terminal, this field would contain the terminal's serial number<br><br>**Constraints**: *Maximum Length*: `36`, *Pattern*: `^[a-zA-Z0-9]*$` | String getTerminalSerialNumber() | setTerminalSerialNumber(String terminalSerialNumber) |
| `TransactionSettlementStatus` | `String` | Optional | (Deprecated field)<br><br>**Constraints**: *Maximum Length*: `32` | String getTransactionSettlementStatus() | setTransactionSettlementStatus(String transactionSettlementStatus) |
| `ChargeBackDate` | `String` | Optional | Charge Back Date (ACH Trxs)<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getChargeBackDate() | setChargeBackDate(String chargeBackDate) |
| `IsRecurring` | `Boolean` | Optional | Flag that is allowed to be passed on card not present industries to signify the transaction is a fixed installment plan transaction. | Boolean getIsRecurring() | setIsRecurring(Boolean isRecurring) |
| `NotificationEmailSent` | `Boolean` | Optional | Indicates if email receipt has been sent | Boolean getNotificationEmailSent() | setNotificationEmailSent(Boolean notificationEmailSent) |
| `Par` | `String` | Optional | A field usually returned form the processor to uniquely identifier a specific cardholder's credit card.<br><br>**Constraints**: *Maximum Length*: `36` | String getPar() | setPar(String par) |
| `ReasonCodeId` | `Object` | Optional | - | Object getReasonCodeId() | setReasonCodeId(Object reasonCodeId) |
| `RecurringId` | `String` | Optional | A unique identifer used to associate a transaction with a Recurring.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getRecurringId() | setRecurringId(String recurringId) |
| `SettleDate` | `String` | Optional | Settle date<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getSettleDate() | setSettleDate(String settleDate) |
| `StatusCode` | `Object` | Optional | - | Object getStatusCode() | setStatusCode(Object statusCode) |
| `TransactionBatchId` | `String` | Optional | For cc transactions, this is the id of the batch the transaction belongs to (not to be confused with batch number). This will be null for transactions that do not settle (void and authonly).<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getTransactionBatchId() | setTransactionBatchId(String transactionBatchId) |
| `TypeId` | `Object` | Optional | - | Object getTypeId() | setTypeId(Object typeId) |
| `Verbiage` | `String` | Optional | Verbiage -Do not use verbiage to see if the transaction was approved, use status_id | String getVerbiage() | setVerbiage(String verbiage) |
| `VoucherNumber` | `String` | Optional | Voucher Number | String getVoucherNumber() | setVoucherNumber(String voucherNumber) |
| `VoidDate` | `String` | Optional | void date<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getVoidDate() | setVoidDate(String voidDate) |
| `Batch` | `String` | Optional | Batch | String getBatch() | setBatch(String batch) |
| `TermsAgree` | `Boolean` | Optional | Terms Agreement | Boolean getTermsAgree() | setTermsAgree(Boolean termsAgree) |
| `ResponseMessage` | `String` | Optional | Response Message<br><br>**Constraints**: *Maximum Length*: `255` | String getResponseMessage() | setResponseMessage(String responseMessage) |
| `ReturnDate` | `String` | Optional | Return Date<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getReturnDate() | setReturnDate(String returnDate) |
| `TrxSourceId` | `Object` | Optional | - | Object getTrxSourceId() | setTrxSourceId(Object trxSourceId) |
| `RoutingNumber` | `String` | Optional | This field is read only for ach on transactions. Must be supplied if account_vault_id is not provided. | String getRoutingNumber() | setRoutingNumber(String routingNumber) |
| `TrxSourceCode` | `Object` | Optional | - | Object getTrxSourceCode() | setTrxSourceCode(Object trxSourceCode) |
| `PaylinkId` | `String` | Optional | Paylink Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getPaylinkId() | setPaylinkId(String paylinkId) |
| `CurrencyCode` | `Double` | Optional | Currency Code<br><br>**Default**: `840d` | Double getCurrencyCode() | setCurrencyCode(Double currencyCode) |
| `IsAccountvault` | `Boolean` | Optional | Is Token Transaction | Boolean getIsAccountvault() | setIsAccountvault(Boolean isAccountvault) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `ModifiedUserId` | `String` | Optional | Last User ID that updated the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getModifiedUserId() | setModifiedUserId(String modifiedUserId) |
| `TransactionCode` | `String` | Optional | Transaction Code | String getTransactionCode() | setTransactionCode(String transactionCode) |
| `EffectiveDate` | `String` | Optional | For ACH only, this is optional and defaults to current day.<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getEffectiveDate() | setEffectiveDate(String effectiveDate) |
| `NotificationPhone` | `String` | Optional | Notification Phone. Country code not included | String getNotificationPhone() | setNotificationPhone(String notificationPhone) |
| `CavvResult` | `String` | Optional | Cavv Result | String getCavvResult() | setCavvResult(String cavvResult) |
| `IsToken` | `Boolean` | Optional | Is Token Transaction | Boolean getIsToken() | setIsToken(Boolean isToken) |
| `AccountVaultId` | `String` | Optional | Token ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getAccountVaultId() | setAccountVaultId(String accountVaultId) |
| `HostedPaymentPageId` | `String` | Optional | Hosted Payment Page Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getHostedPaymentPageId() | setHostedPaymentPageId(String hostedPaymentPageId) |
| `Stan` | `String` | Optional | - | String getStan() | setStan(String stan) |
| `Currency` | `String` | Optional | Currency | String getCurrency() | setCurrency(String currency) |
| `CardBin` | `String` | Optional | Card Bin | String getCardBin() | setCardBin(String cardBin) |
| `WalletType` | `String` | Optional | This value provides information from where the transaction was initialized (Such as In-App provider) | String getWalletType() | setWalletType(String walletType) |
| `AccountVault` | [`AccountVault1`](../../doc/models/account-vault-1.md) | Optional | - | AccountVault1 getAccountVault() | setAccountVault(AccountVault1 accountVault) |
| `QuickInvoice` | [`QuickInvoice1`](../../doc/models/quick-invoice-1.md) | Optional | - | QuickInvoice1 getQuickInvoice() | setQuickInvoice(QuickInvoice1 quickInvoice) |
| `LogEmails` | [`List<LogEmail>`](../../doc/models/log-email.md) | Optional | Log Email Information on `expand` | List<LogEmail> getLogEmails() | setLogEmails(List<LogEmail> logEmails) |
| `IsVoidable` | `Boolean` | Optional | Is Voidable Information on `expand` | Boolean getIsVoidable() | setIsVoidable(Boolean isVoidable) |
| `IsReversible` | `Boolean` | Optional | Is Reversible Information on `expand` | Boolean getIsReversible() | setIsReversible(Boolean isReversible) |
| `IsRefundable` | `Boolean` | Optional | Is Refundable Information on `expand` | Boolean getIsRefundable() | setIsRefundable(Boolean isRefundable) |
| `IsCompletable` | `Boolean` | Optional | Is Competable Information on `expand` | Boolean getIsCompletable() | setIsCompletable(Boolean isCompletable) |
| `IsSettled` | `Boolean` | Optional | Is Settled Information on `expand` | Boolean getIsSettled() | setIsSettled(Boolean isSettled) |
| `CreatedUser` | [`User9`](../../doc/models/user-9.md) | Optional | - | User9 getCreatedUser() | setCreatedUser(User9 createdUser) |
| `Location` | [`Location18`](../../doc/models/location-18.md) | Optional | - | Location18 getLocation() | setLocation(Location18 location) |
| `Contact` | [`Contact3`](../../doc/models/contact-3.md) | Optional | - | Contact3 getContact() | setContact(Contact3 contact) |
| `Changelogs` | [`List<Changelog>`](../../doc/models/changelog.md) | Optional | Changelog Information on `expand` | List<Changelog> getChangelogs() | setChangelogs(List<Changelog> changelogs) |
| `ProductTransaction` | [`ProductTransaction1`](../../doc/models/product-transaction-1.md) | Optional | - | ProductTransaction1 getProductTransaction() | setProductTransaction(ProductTransaction1 productTransaction) |
| `AllTags` | [`List<AllTag>`](../../doc/models/all-tag.md) | Optional | All Tag Information on `expand` | List<AllTag> getAllTags() | setAllTags(List<AllTag> allTags) |
| `TagTransactions` | [`List<TagTransaction>`](../../doc/models/tag-transaction.md) | Optional | TagTransaction Information on `expand` | List<TagTransaction> getTagTransactions() | setTagTransactions(List<TagTransaction> tagTransactions) |
| `DeclinedRecurringNotification` | [`DeclinedRecurringNotification1`](../../doc/models/declined-recurring-notification-1.md) | Optional | - | DeclinedRecurringNotification1 getDeclinedRecurringNotification() | setDeclinedRecurringNotification(DeclinedRecurringNotification1 declinedRecurringNotification) |
| `PaymentRecurringNotification` | [`PaymentRecurringNotification1`](../../doc/models/payment-recurring-notification-1.md) | Optional | - | PaymentRecurringNotification1 getPaymentRecurringNotification() | setPaymentRecurringNotification(PaymentRecurringNotification1 paymentRecurringNotification) |
| `DeveloperCompany` | [`DeveloperCompany1`](../../doc/models/developer-company-1.md) | Optional | - | DeveloperCompany1 getDeveloperCompany() | setDeveloperCompany(DeveloperCompany1 developerCompany) |
| `Terminal` | [`Terminal2`](../../doc/models/terminal-2.md) | Optional | - | Terminal2 getTerminal() | setTerminal(Terminal2 terminal) |
| `HostedPaymentPage` | [`HostedPaymentPage1`](../../doc/models/hosted-payment-page-1.md) | Optional | - | HostedPaymentPage1 getHostedPaymentPage() | setHostedPaymentPage(HostedPaymentPage1 hostedPaymentPage) |
| `TransactionLevel3` | [`Data29`](../../doc/models/data-29.md) | Optional | - | Data29 getTransactionLevel3() | setTransactionLevel3(Data29 transactionLevel3) |
| `DeveloperCompanyId` | `String` | Optional | Developer Company Id Information on `expand` | String getDeveloperCompanyId() | setDeveloperCompanyId(String developerCompanyId) |
| `TransactionHistories` | [`List<TransactionHistory>`](../../doc/models/transaction-history.md) | Optional | Transaction History Information on `expand` | List<TransactionHistory> getTransactionHistories() | setTransactionHistories(List<TransactionHistory> transactionHistories) |
| `SurchargeTransaction` | [`SurchargeTransaction1`](../../doc/models/surcharge-transaction-1.md) | Optional | - | SurchargeTransaction1 getSurchargeTransaction() | setSurchargeTransaction(SurchargeTransaction1 surchargeTransaction) |
| `Surcharge` | [`Surcharge1`](../../doc/models/surcharge-1.md) | Optional | - | Surcharge1 getSurcharge() | setSurcharge(Surcharge1 surcharge) |
| `Signature` | [`Signature1`](../../doc/models/signature-1.md) | Optional | - | Signature1 getSignature() | setSignature(Signature1 signature) |
| `ReasonCode` | [`ReasonCode1`](../../doc/models/reason-code-1.md) | Optional | - | ReasonCode1 getReasonCode() | setReasonCode(ReasonCode1 reasonCode) |
| `Type` | [`Type7`](../../doc/models/type-7.md) | Optional | - | Type7 getType() | setType(Type7 type) |
| `Status` | [`Status7`](../../doc/models/status-7.md) | Optional | - | Status7 getStatus() | setStatus(Status7 status) |
| `TransactionBatch` | [`TransactionBatch1`](../../doc/models/transaction-batch-1.md) | Optional | - | TransactionBatch1 getTransactionBatch() | setTransactionBatch(TransactionBatch1 transactionBatch) |
| `TransactionSplits` | [`List<TransactionSplit>`](../../doc/models/transaction-split.md) | Optional | Transaction Split Information on `expand` | List<TransactionSplit> getTransactionSplits() | setTransactionSplits(List<TransactionSplit> transactionSplits) |
| `PostbackLogs` | [`List<PostbackLog>`](../../doc/models/postback-log.md) | Optional | Postback Log Information on `expand` | List<PostbackLog> getPostbackLogs() | setPostbackLogs(List<PostbackLog> postbackLogs) |
| `CurrencyType` | [`CurrencyType1`](../../doc/models/currency-type-1.md) | Optional | - | CurrencyType1 getCurrencyType() | setCurrencyType(CurrencyType1 currencyType) |
| `TransactionReferences` | [`List<TransactionReference>`](../../doc/models/transaction-reference.md) | Optional | Transaction Reference Information on `expand` | List<TransactionReference> getTransactionReferences() | setTransactionReferences(List<TransactionReference> transactionReferences) |
| `RejectedTransactionAchRetries` | [`List<RejectedTransactionAchRetry>`](../../doc/models/rejected-transaction-ach-retry.md) | Optional | [object Object] | List<RejectedTransactionAchRetry> getRejectedTransactionAchRetries() | setRejectedTransactionAchRetries(List<RejectedTransactionAchRetry> rejectedTransactionAchRetries) |
| `ReturnFeeTransactionAchRetry` | [`RejectedTransactionAchRetry`](../../doc/models/rejected-transaction-ach-retry.md) | Optional | - | RejectedTransactionAchRetry getReturnFeeTransactionAchRetry() | setReturnFeeTransactionAchRetry(RejectedTransactionAchRetry returnFeeTransactionAchRetry) |
| `RetryTransactionAchRetry` | [`RejectedTransactionAchRetry`](../../doc/models/rejected-transaction-ach-retry.md) | Optional | - | RejectedTransactionAchRetry getRetryTransactionAchRetry() | setRetryTransactionAchRetry(RejectedTransactionAchRetry retryTransactionAchRetry) |
| `IsRetriable` | `Boolean` | Optional | [object Object] | Boolean getIsRetriable() | setIsRetriable(Boolean isRetriable) |
| `SavedAccount` | [`SavedAccount1`](../../doc/models/saved-account-1.md) | Optional | - | SavedAccount1 getSavedAccount() | setSavedAccount(SavedAccount1 savedAccount) |
| `Balances` | [`List<Balance>`](../../doc/models/balance.md) | Optional | Additional amounts | List<Balance> getBalances() | setBalances(List<Balance> balances) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "checkin_date": "2021-12-01",
  "checkout_date": "2021-12-01",
  "clerk_number": "AE1234",
  "contact_id": "11e95f8ec39de8fbdb0a4f1a",
  "custom_data": {
    "data1": "custom1",
    "data2": "custom2"
  },
  "customer_id": "customerid",
  "description": "some description",
  "image_front": "U29tZVN0cmluZ09idmlvdXNseU5vdEJhc2U2NEVuY29kZWQ=",
  "image_back": "U29tZVN0cmluZ09idmlvdXNseU5vdEJhc2U2NEVuY29kZWQ=",
  "installment": true,
  "installment_number": 1,
  "installment_count": 1,
  "installment_counter": 1,
  "installment_total": 1,
  "subscription": false,
  "standing_order": false,
  "location_api_id": "location-api-id-florida-2",
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "advance_deposit": false,
  "no_show": false,
  "notification_email_address": "johnsmith@smiths.com",
  "order_number": "433659378839",
  "po_number": "555555553123",
  "quick_invoice_id": "11e95f8ec39de8fbdb0a4f1a",
  "recurring_number": 1,
  "room_num": "303",
  "room_rate": 95,
  "save_account": false,
  "save_account_title": "John Account",
  "subtotal_amount": 599,
  "surcharge_amount": 100,
  "tax": 0,
  "tip_amount": 0,
  "transaction_amount": 0,
  "secondary_amount": 0,
  "transaction_api_id": "transaction-payment-abcd123",
  "transaction_c1": "custom-data-1",
  "transaction_c2": "custom-data-2",
  "transaction_c3": "custom-data-3",
  "bank_funded_only_override": false,
  "allow_partial_authorization_override": false,
  "auto_decline_cvv_override": false,
  "auto_decline_street_override": false,
  "auto_decline_zip_override": false,
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "terminal_id": "11e95f8ec39de8fbdb0a4f1a",
  "account_holder_name": "smith",
  "account_type": "checking",
  "token_id": "11e95f8ec39de8fbdb0a4f1a",
  "ach_identifier": "P",
  "auth_amount": 1,
  "auth_code": "BR349K",
  "avs_enhanced": "N",
  "cardholder_present": true,
  "card_present": true,
  "check_number": "8520748520963",
  "customer_ip": "192.168.0.10",
  "cvv_response": "N",
  "first_six": "545454",
  "last_four": "5454",
  "terminal_serial_number": "1234567890",
  "charge_back_date": "2021-12-01",
  "is_recurring": true,
  "notification_email_sent": true,
  "par": "Q1J4Z28RKA1EBL470G9XYG90R5D3E",
  "recurring_id": "11e95f8ec39de8fbdb0a4f1a",
  "settle_date": "2021-12-01",
  "transaction_batch_id": "11e95f8ec39de8fbdb0a4f1a",
  "verbiage": "APPROVED",
  "voucher_number": "1234",
  "void_date": "2021-12-01",
  "batch": "2",
  "terms_agree": true,
  "return_date": "2021-12-01",
  "routing_number": "051904524",
  "paylink_id": "11e95f8ec39de8fbdb0a4f1a",
  "currency_code": 840,
  "is_accountvault": true,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "modified_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "effective_date": "2021-12-01",
  "is_token": true,
  "account_vault_id": "11e95f8ec39de8fbdb0a4f1a",
  "hosted_payment_page_id": "11e95f8ec39de8fbdb0a4f1a",
  "is_voidable": true,
  "is_reversible": true,
  "is_refundable": true,
  "is_completable": true,
  "is_settled": true,
  "developer_company_id": "Sample Developer Company ID",
  "additional_amounts": [
    {
      "type": {
        "key1": "val1",
        "key2": "val2"
      },
      "amount": 6,
      "account_type": {
        "key1": "val1",
        "key2": "val2"
      },
      "currency": 154.64,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "billing_address": {
    "city": "city2",
    "state": "state6",
    "postal_code": "postal_code0",
    "street": "street8",
    "phone": "phone2",
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

