
# V1 Transactions Cc Auth Only Terminal Request

*This model accepts additional fields of type Object.*

## Structure

`V1TransactionsCcAuthOnlyTerminalRequest`

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
| `IdentityVerification` | [`IdentityVerification1`](../../doc/models/identity-verification-1.md) | Optional | - | IdentityVerification1 getIdentityVerification() | setIdentityVerification(IdentityVerification1 identityVerification) |
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
| `LocationId` | `String` | Required | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `ProductTransactionId` | `String` | Optional | The Product's method (cc/ach) has to match the action. If not provided, the API will use the default configured for the Location.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getProductTransactionId() | setProductTransactionId(String productTransactionId) |
| `AdvanceDeposit` | `Boolean` | Optional | Advance Deposit | Boolean getAdvanceDeposit() | setAdvanceDeposit(Boolean advanceDeposit) |
| `NoShow` | `Boolean` | Optional | Used in Lodging | Boolean getNoShow() | setNoShow(Boolean noShow) |
| `NotificationEmailAddress` | `String` | Optional | If email is supplied then receipt will be emailed | String getNotificationEmailAddress() | setNotificationEmailAddress(String notificationEmailAddress) |
| `OrderNumber` | `String` | Optional | Required for CC transactions , if merchant's deposit account's duplicate check per batch has 'order_number' field<br><br>**Constraints**: *Maximum Length*: `32` | String getOrderNumber() | setOrderNumber(String orderNumber) |
| `PoNumber` | `String` | Optional | Purchase Order number<br><br>**Constraints**: *Maximum Length*: `64` | String getPoNumber() | setPoNumber(String poNumber) |
| `QuickInvoiceId` | `String` | Optional | Can be used to associate a transaction to a Quick Invoice.  Quick Invoice transactions will have a value for this field automatically.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getQuickInvoiceId() | setQuickInvoiceId(String quickInvoiceId) |
| `Recurring` | `Boolean` | Optional | Flag that is allowed to be passed on card not present industries to signify the transaction is an ongoing recurring transaction. Possible values to send are 0 or 1. This field must be 0 or not present if installment is sent as 1. | Boolean getRecurring() | setRecurring(Boolean recurring) |
| `RecurringNumber` | `Integer` | Optional | If this is an ongoing recurring and recurring field is being passed as 1, then this field must have a vlue of 1-999 specifying the current recurring number that is running.<br><br>**Constraints**: `>= 1`, `<= 999` | Integer getRecurringNumber() | setRecurringNumber(Integer recurringNumber) |
| `RoomNum` | `String` | Optional | Used in Lodging<br><br>**Constraints**: *Maximum Length*: `12` | String getRoomNum() | setRoomNum(String roomNum) |
| `RoomRate` | `Integer` | Optional | Required if merchant industry type is lodging. | Integer getRoomRate() | setRoomRate(Integer roomRate) |
| `SaveAccount` | `Boolean` | Optional | Specifies to save account to contacts profile if account_number/track_data is present with either contact_id or contact_api_id in params. | Boolean getSaveAccount() | setSaveAccount(Boolean saveAccount) |
| `SaveAccountTitle` | `String` | Optional | If saving token while running a transaction, this will be the title of the token.<br><br>**Constraints**: *Maximum Length*: `16` | String getSaveAccountTitle() | setSaveAccountTitle(String saveAccountTitle) |
| `SubtotalAmount` | `Integer` | Optional | This field is allowed and required for transactions that have a product where surcharge is configured. Use only integer numbers, so $10.99 will be 1099.<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getSubtotalAmount() | setSubtotalAmount(Integer subtotalAmount) |
| `SurchargeAmount` | `Integer` | Optional | This field is allowed and required for transactions that have a product where surcharge is configured. Use only integer numbers, so $10.99 will be 1099.<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getSurchargeAmount() | setSurchargeAmount(Integer surchargeAmount) |
| `Tags` | `List<String>` | Optional | Tags | List<String> getTags() | setTags(List<String> tags) |
| `Tax` | `Integer` | Optional | Amount of Sales tax - If supplied, this amount should be included in the total transaction_amount field. Use only integer numbers, so $10.99 will be 1099.<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getTax() | setTax(Integer tax) |
| `TipAmount` | `Integer` | Optional | Optional tip amount. Tip is not supported for lodging and ecommerce merchants. Use only integer numbers, so $10.99 will be 1099.<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getTipAmount() | setTipAmount(Integer tipAmount) |
| `TransactionAmount` | `int` | Required | Amount of the transaction. This should always be the desired settle amount of the transaction. Use only integer numbers, so $10.99 will be 1099.<br><br>**Constraints**: `>= 1`, `<= 999999999` | int getTransactionAmount() | setTransactionAmount(int transactionAmount) |
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
| `CardholderPresent` | `Boolean` | Optional | If the cardholder is present at the point of service | Boolean getCardholderPresent() | setCardholderPresent(Boolean cardholderPresent) |
| `CardPresent` | `Boolean` | Optional | A POST only field to specify whether or not the card is present.<br><br>> This field will be defaulted to '1' for all card present industries (retail, lodging, restaurant) and '0' for card not present industries (MOTO/e-commerce).<br>> For lodging, if the no_show flag is set to '1', this field will automatically be set to '0'.<br>> For transactions where account_vault_id is used, this filed will be set to '0'. | Boolean getCardPresent() | setCardPresent(Boolean cardPresent) |
| `SecureAuthData` | `String` | Optional | (ECOMM) The token authentication value associated with 3D secure transactions (Such as CAVV, UCAF auth data) | String getSecureAuthData() | setSecureAuthData(String secureAuthData) |
| `SecureProtocolVersion` | `Integer` | Optional | (ECOMM)  Secure Program Protocol Version | Integer getSecureProtocolVersion() | setSecureProtocolVersion(Integer secureProtocolVersion) |
| `SecureCollectionIndicator` | `Integer` | Optional | (ECOMM) Used for UCAF collection indicator or Discover Autentication type | Integer getSecureCollectionIndicator() | setSecureCollectionIndicator(Integer secureCollectionIndicator) |
| `SecureCryptogram` | `String` | Optional | (ECOMM) Used to supply the Digital Payment Cryptogram obtained from a Digital Secure Remote Payment (DSRP) transaction | String getSecureCryptogram() | setSecureCryptogram(String secureCryptogram) |
| `SecureDirectoryServerTransactionId` | `String` | Optional | (ECOMM) Directory Server Transaction ID (Such as XID, TAVV) | String getSecureDirectoryServerTransactionId() | setSecureDirectoryServerTransactionId(String secureDirectoryServerTransactionId) |
| `SecureEcommUrl` | `String` | Optional | (ECOMM) This field is used to enter a merchant identifier such as the Merchant URL or reverse domain name as presented to the consumer during the checkout process for a Digital Secure Remote payment transaction | String getSecureEcommUrl() | setSecureEcommUrl(String secureEcommUrl) |
| `TerminalSerialNumber` | `String` | Optional | If transaction was processed using a terminal, this field would contain the terminal's serial number<br><br>**Constraints**: *Maximum Length*: `36`, *Pattern*: `^[a-zA-Z0-9]*$` | String getTerminalSerialNumber() | setTerminalSerialNumber(String terminalSerialNumber) |
| `Threedsecure` | `Boolean` | Optional | (ECOMM) Specify if the transaction is obtained by 3DSecure. | Boolean getThreedsecure() | setThreedsecure(Boolean threedsecure) |
| `ThreeDsServerTransId` | `String` | Optional | 3DS Server Transaction ID.  If this field is sent and 3DS authentication was done with Fortis, the 3DS fields secure_directory_server_transaction_id, secure_protocol_version, and secure_collection_indicator will be pre-populated. | String getThreeDsServerTransId() | setThreeDsServerTransId(String threeDsServerTransId) |
| `WalletType` | `Object` | Optional | - | Object getWalletType() | setWalletType(Object walletType) |
| `ClerkId` | `String` | Optional | Clerk ID | String getClerkId() | setClerkId(String clerkId) |
| `VoucherNumber` | `String` | Optional | Voucher Number | String getVoucherNumber() | setVoucherNumber(String voucherNumber) |
| `InitiationType` | `Object` | Optional | - | Object getInitiationType() | setInitiationType(Object initiationType) |
| `BillPayment` | `Boolean` | Optional | If transaction is a bill payment | Boolean getBillPayment() | setBillPayment(Boolean billPayment) |
| `DelayCharge` | `Boolean` | Optional | Delay Charge | Boolean getDelayCharge() | setDelayCharge(Boolean delayCharge) |
| `DeferredAuth` | `Boolean` | Optional | Deferred Auth | Boolean getDeferredAuth() | setDeferredAuth(Boolean deferredAuth) |
| `MiniBar` | `Boolean` | Optional | Mini Bar | Boolean getMiniBar() | setMiniBar(Boolean miniBar) |
| `EbtFoodEligibleAmount` | `Integer` | Optional | EBT Food Eligible Amount<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getEbtFoodEligibleAmount() | setEbtFoodEligibleAmount(Integer ebtFoodEligibleAmount) |
| `EbtCashEligibleAmount` | `Integer` | Optional | EBT Cash Eligible Amount<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getEbtCashEligibleAmount() | setEbtCashEligibleAmount(Integer ebtCashEligibleAmount) |
| `TerminalId` | `String` | Required | Terminal ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getTerminalId() | setTerminalId(String terminalId) |
| `TerminalApiId` | `String` | Optional | Advance Deposit<br><br>**Constraints**: *Maximum Length*: `36` | String getTerminalApiId() | setTerminalApiId(String terminalApiId) |
| `EFormat` | `Object` | Optional | - | Object getEFormat() | setEFormat(Object eFormat) |
| `ETrackData` | `String` | Optional | Encrypted Track Data | String getETrackData() | setETrackData(String eTrackData) |
| `ESerialNumber` | `String` | Optional | Encrypted Track Data KSN<br><br>**Constraints**: *Maximum Length*: `20` | String getESerialNumber() | setESerialNumber(String eSerialNumber) |
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
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "advance_deposit": false,
  "no_show": false,
  "notification_email_address": "johnsmith@smiths.com",
  "order_number": "433659378839",
  "po_number": "555555553123",
  "quick_invoice_id": "11e95f8ec39de8fbdb0a4f1a",
  "recurring": false,
  "recurring_number": 1,
  "room_num": "303",
  "room_rate": 95,
  "save_account": false,
  "save_account_title": "John Account",
  "subtotal_amount": 599,
  "surcharge_amount": 100,
  "tax": 0,
  "tip_amount": 0,
  "transaction_amount": 1,
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
  "secure_auth_data": "vVwL7UNHCf8W8M2LAfvRChNHN7c%3D",
  "secure_protocol_version": 2,
  "secure_cryptogram": "ZVVEVDJITHpTNE9yNlNHMUh0R0E=",
  "secure_directory_server_transaction_id": "d65e93c3-35ab-41ba-b307-767bfc19eae",
  "terminal_serial_number": "1234567890",
  "threedsecure": true,
  "three_ds_server_trans_id": "d65e93c3-35ab-41ba-b307-767bfc19eae",
  "clerk_id": "1234",
  "voucher_number": "1234",
  "bill_payment": true,
  "delay_charge": true,
  "deferred_auth": true,
  "ebt_food_eligible_amount": 0,
  "ebt_cash_eligible_amount": 0,
  "terminal_id": "11e95f8ec39de8fbdb0a4f1a",
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

