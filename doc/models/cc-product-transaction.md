
# Cc Product Transaction

Cc Product Transaction Information on `expand`

## Structure

`CcProductTransaction`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ProcessorVersion` | `String` | Optional | Processor Version | String getProcessorVersion() | setProcessorVersion(String processorVersion) |
| `IndustryType` | [`IndustryTypeEnum`](../../doc/models/industry-type-enum.md) | Optional | Industry Type<br><br>**Constraints**: *Maximum Length*: `45` | IndustryTypeEnum getIndustryType() | setIndustryType(IndustryTypeEnum industryType) |
| `Title` | `String` | Optional | Title<br><br>**Constraints**: *Maximum Length*: `64` | String getTitle() | setTitle(String title) |
| `PaymentMethod` | [`PaymentMethodEnum`](../../doc/models/payment-method-enum.md) | Optional | Payment method | PaymentMethodEnum getPaymentMethod() | setPaymentMethod(PaymentMethodEnum paymentMethod) |
| `Processor` | [`ProcessorEnum`](../../doc/models/processor-enum.md) | Optional | Processor | ProcessorEnum getProcessor() | setProcessor(ProcessorEnum processor) |
| `Mcc` | `String` | Optional | MCC<br><br>**Constraints**: *Maximum Length*: `4`, *Pattern*: `^\d+$` | String getMcc() | setMcc(String mcc) |
| `TaxSurchargeConfig` | [`TaxSurchargeConfigEnum`](../../doc/models/tax-surcharge-config-enum.md) | Optional | Tax Surcharge Config<br><br>**Default**: `TaxSurchargeConfigEnum.ENUM_2` | TaxSurchargeConfigEnum getTaxSurchargeConfig() | setTaxSurchargeConfig(TaxSurchargeConfigEnum taxSurchargeConfig) |
| `TerminalId` | `String` | Optional | Terminal ID<br><br>**Constraints**: *Maximum Length*: `24` | String getTerminalId() | setTerminalId(String terminalId) |
| `Partner` | [`PartnerEnum`](../../doc/models/partner-enum.md) | Optional | Partner<br><br>**Constraints**: *Maximum Length*: `24` | PartnerEnum getPartner() | setPartner(PartnerEnum partner) |
| `ProductAchPvStoreId` | `String` | Optional | Product Ach Pv Store ID | String getProductAchPvStoreId() | setProductAchPvStoreId(String productAchPvStoreId) |
| `InvoiceAdjustmentTitle` | `String` | Optional | Invoice Adjustment Title | String getInvoiceAdjustmentTitle() | setInvoiceAdjustmentTitle(String invoiceAdjustmentTitle) |
| `LocationId` | `String` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `LocationApiId` | `String` | Optional | Location Api ID | String getLocationApiId() | setLocationApiId(String locationApiId) |
| `BillingLocationApiId` | `String` | Optional | Billing Location API ID | String getBillingLocationApiId() | setBillingLocationApiId(String billingLocationApiId) |
| `PortfolioId` | `String` | Optional | Portfolio ID | String getPortfolioId() | setPortfolioId(String portfolioId) |
| `PortfolioValidationRule` | `String` | Optional | Product Validation Rule | String getPortfolioValidationRule() | setPortfolioValidationRule(String portfolioValidationRule) |
| `SubProcessor` | `String` | Optional | Sub Processor<br><br>**Constraints**: *Maximum Length*: `48` | String getSubProcessor() | setSubProcessor(String subProcessor) |
| `Surcharge` | `Object` | Optional | Surcharge | Object getSurcharge() | setSurcharge(Object surcharge) |
| `ProcessorData` | `Object` | Optional | - | Object getProcessorData() | setProcessorData(Object processorData) |
| `VtClerkNumber` | `Boolean` | Optional | Vt Clerk Number | Boolean getVtClerkNumber() | setVtClerkNumber(Boolean vtClerkNumber) |
| `VtBillingPhone` | `Boolean` | Optional | Card Type JCB | Boolean getVtBillingPhone() | setVtBillingPhone(Boolean vtBillingPhone) |
| `VtEnableTip` | `Boolean` | Optional | VT Enable Tip | Boolean getVtEnableTip() | setVtEnableTip(Boolean vtEnableTip) |
| `AchAllowDebit` | `Boolean` | Optional | Ach Allow Debit | Boolean getAchAllowDebit() | setAchAllowDebit(Boolean achAllowDebit) |
| `AchAllowCredit` | `Boolean` | Optional | Ach Allow Credit | Boolean getAchAllowCredit() | setAchAllowCredit(Boolean achAllowCredit) |
| `AchAllowRefund` | `Boolean` | Optional | Ach Allow Refund | Boolean getAchAllowRefund() | setAchAllowRefund(Boolean achAllowRefund) |
| `VtCvv` | `Boolean` | Optional | VT CVV | Boolean getVtCvv() | setVtCvv(Boolean vtCvv) |
| `VtStreet` | `Boolean` | Optional | VT Street | Boolean getVtStreet() | setVtStreet(Boolean vtStreet) |
| `VtZip` | `Boolean` | Optional | VT Zip | Boolean getVtZip() | setVtZip(Boolean vtZip) |
| `VtOrderNum` | `Boolean` | Optional | VT Order Num | Boolean getVtOrderNum() | setVtOrderNum(Boolean vtOrderNum) |
| `VtEnable` | `Boolean` | Optional | VT Enable | Boolean getVtEnable() | setVtEnable(Boolean vtEnable) |
| `ReceiptShowContactName` | `Boolean` | Optional | Receipt Show Contact Name | Boolean getReceiptShowContactName() | setReceiptShowContactName(Boolean receiptShowContactName) |
| `DisplayAvs` | `Boolean` | Optional | Display Avs | Boolean getDisplayAvs() | setDisplayAvs(Boolean displayAvs) |
| `CardTypeVisa` | `Boolean` | Optional | Card Type Visa | Boolean getCardTypeVisa() | setCardTypeVisa(Boolean cardTypeVisa) |
| `CardTypeMc` | `Boolean` | Optional | Card Type Mc | Boolean getCardTypeMc() | setCardTypeMc(Boolean cardTypeMc) |
| `CardTypeDisc` | `Boolean` | Optional | Card Type Disc | Boolean getCardTypeDisc() | setCardTypeDisc(Boolean cardTypeDisc) |
| `CardTypeAmex` | `Boolean` | Optional | Card Type Amex | Boolean getCardTypeAmex() | setCardTypeAmex(Boolean cardTypeAmex) |
| `CardTypeDiners` | `Boolean` | Optional | Card Type Dinners | Boolean getCardTypeDiners() | setCardTypeDiners(Boolean cardTypeDiners) |
| `CardTypeJcb` | `Boolean` | Optional | - | Boolean getCardTypeJcb() | setCardTypeJcb(Boolean cardTypeJcb) |
| `CardTypeEbt` | `Boolean` | Optional | Card Type EBT | Boolean getCardTypeEbt() | setCardTypeEbt(Boolean cardTypeEbt) |
| `AllowEbtCashBenefit` | `Boolean` | Optional | Allow EBT Cash Benefit | Boolean getAllowEbtCashBenefit() | setAllowEbtCashBenefit(Boolean allowEbtCashBenefit) |
| `AllowEbtFoodStamp` | `Boolean` | Optional | Allow EBT Food Stamp | Boolean getAllowEbtFoodStamp() | setAllowEbtFoodStamp(Boolean allowEbtFoodStamp) |
| `InvoiceLocation` | `Boolean` | Optional | Invoice Location | Boolean getInvoiceLocation() | setInvoiceLocation(Boolean invoiceLocation) |
| `AllowPartialAuthorization` | `Boolean` | Optional | Allow Partial Authorization | Boolean getAllowPartialAuthorization() | setAllowPartialAuthorization(Boolean allowPartialAuthorization) |
| `AllowRecurringPartialAuthorization` | `Boolean` | Optional | Allow Recurring Partial Authorization | Boolean getAllowRecurringPartialAuthorization() | setAllowRecurringPartialAuthorization(Boolean allowRecurringPartialAuthorization) |
| `AutoDeclineCvv` | `Boolean` | Optional | Auto Decline Cvv | Boolean getAutoDeclineCvv() | setAutoDeclineCvv(Boolean autoDeclineCvv) |
| `AutoDeclineStreet` | `Boolean` | Optional | Auto Decline Street | Boolean getAutoDeclineStreet() | setAutoDeclineStreet(Boolean autoDeclineStreet) |
| `AutoDeclineZip` | `Boolean` | Optional | Auto Decline ZIP | Boolean getAutoDeclineZip() | setAutoDeclineZip(Boolean autoDeclineZip) |
| `SplitPaymentsAllow` | `Boolean` | Optional | Split Payments Allow | Boolean getSplitPaymentsAllow() | setSplitPaymentsAllow(Boolean splitPaymentsAllow) |
| `VtShowCustomFields` | `Boolean` | Optional | Vt Show Custom Fields | Boolean getVtShowCustomFields() | setVtShowCustomFields(Boolean vtShowCustomFields) |
| `ReceiptShowCustomFields` | `Boolean` | Optional | Receipt Show Custom Fields | Boolean getReceiptShowCustomFields() | setReceiptShowCustomFields(Boolean receiptShowCustomFields) |
| `VtOverrideSalesTaxAllowed` | `Boolean` | Optional | Vt Override Sales Tax Allowed | Boolean getVtOverrideSalesTaxAllowed() | setVtOverrideSalesTaxAllowed(Boolean vtOverrideSalesTaxAllowed) |
| `VtEnableSalesTax` | `Boolean` | Optional | Vt Enable Sales Tax | Boolean getVtEnableSalesTax() | setVtEnableSalesTax(Boolean vtEnableSalesTax) |
| `VtRequireZip` | `Boolean` | Optional | Vt Require ZIP | Boolean getVtRequireZip() | setVtRequireZip(Boolean vtRequireZip) |
| `VtRequireStreet` | `Boolean` | Optional | Vt Require Street | Boolean getVtRequireStreet() | setVtRequireStreet(Boolean vtRequireStreet) |
| `AutoDeclineCavv` | `Boolean` | Optional | Auto Decline Cavv | Boolean getAutoDeclineCavv() | setAutoDeclineCavv(Boolean autoDeclineCavv) |
| `MerchantId` | `String` | Optional | Merchant ID<br><br>**Constraints**: *Maximum Length*: `24` | String getMerchantId() | setMerchantId(String merchantId) |
| `ReceiptHeader` | `String` | Optional | Receipt Header<br><br>**Constraints**: *Maximum Length*: `255` | String getReceiptHeader() | setReceiptHeader(String receiptHeader) |
| `ReceiptFooter` | `String` | Optional | Receipt Footer<br><br>**Constraints**: *Maximum Length*: `255` | String getReceiptFooter() | setReceiptFooter(String receiptFooter) |
| `ReceiptAddAccountAboveSignature` | `String` | Optional | Receipt Add Account Above Signature<br><br>**Constraints**: *Maximum Length*: `1032` | String getReceiptAddAccountAboveSignature() | setReceiptAddAccountAboveSignature(String receiptAddAccountAboveSignature) |
| `ReceiptAddRecurringAboveSignature` | `String` | Optional | Receipt Add Recurring Above Signature<br><br>**Constraints**: *Maximum Length*: `1032` | String getReceiptAddRecurringAboveSignature() | setReceiptAddRecurringAboveSignature(String receiptAddRecurringAboveSignature) |
| `ReceiptVtAboveSignature` | `String` | Optional | Receipt VT Above Signature<br><br>**Constraints**: *Maximum Length*: `1032` | String getReceiptVtAboveSignature() | setReceiptVtAboveSignature(String receiptVtAboveSignature) |
| `DefaultTransactionType` | [`DefaultTransactionTypeEnum`](../../doc/models/default-transaction-type-enum.md) | Optional | Default Transaction Type | DefaultTransactionTypeEnum getDefaultTransactionType() | setDefaultTransactionType(DefaultTransactionTypeEnum defaultTransactionType) |
| `Username` | `String` | Optional | Username<br><br>**Constraints**: *Maximum Length*: `512` | String getUsername() | setUsername(String username) |
| `Password` | `String` | Optional | Passowrd<br><br>**Constraints**: *Maximum Length*: `512` | String getPassword() | setPassword(String password) |
| `CurrentBatch` | `Double` | Optional | Current Batch<br><br>**Default**: `1d`<br><br>**Constraints**: `>= 1`, `<= 9999` | Double getCurrentBatch() | setCurrentBatch(Double currentBatch) |
| `DupCheckPerBatch` | `String` | Optional | Dup Check Per Batch<br><br>**Constraints**: *Maximum Length*: `500` | String getDupCheckPerBatch() | setDupCheckPerBatch(String dupCheckPerBatch) |
| `AgentCode` | `String` | Optional | Agent Code<br><br>**Constraints**: *Maximum Length*: `16`, *Pattern*: `^[\w\-]+$` | String getAgentCode() | setAgentCode(String agentCode) |
| `PaylinkAllow` | `Boolean` | Optional | Paylink Allow | Boolean getPaylinkAllow() | setPaylinkAllow(Boolean paylinkAllow) |
| `QuickInvoiceAllow` | `Boolean` | Optional | Quick Invoice Allow | Boolean getQuickInvoiceAllow() | setQuickInvoiceAllow(Boolean quickInvoiceAllow) |
| `Level3Allow` | `Boolean` | Optional | Level3 Allow | Boolean getLevel3Allow() | setLevel3Allow(Boolean level3Allow) |
| `PayfacEnable` | `Boolean` | Optional | Payfac Enable | Boolean getPayfacEnable() | setPayfacEnable(Boolean payfacEnable) |
| `Enable3ds` | `Boolean` | Optional | Enable 3DS | Boolean getEnable3ds() | setEnable3ds(Boolean enable3ds) |
| `SalesOfficeId` | `String` | Optional | Sales Office ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getSalesOfficeId() | setSalesOfficeId(String salesOfficeId) |
| `HostedPaymentPageMaxAllowed` | `Double` | Optional | Hosted Payment Page Max Allowed<br><br>**Default**: `5d`<br><br>**Constraints**: `>= 1`, `<= 999` | Double getHostedPaymentPageMaxAllowed() | setHostedPaymentPageMaxAllowed(Double hostedPaymentPageMaxAllowed) |
| `HostedPaymentPageAllow` | `Boolean` | Optional | Hosted Payment Page Allow | Boolean getHostedPaymentPageAllow() | setHostedPaymentPageAllow(Boolean hostedPaymentPageAllow) |
| `SurchargeId` | `String` | Optional | Surcharge ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getSurchargeId() | setSurchargeId(String surchargeId) |
| `AllowBigCommerce` | `Boolean` | Optional | Allow Big Commerce | Boolean getAllowBigCommerce() | setAllowBigCommerce(Boolean allowBigCommerce) |
| `Level3Default` | [`Level3Default`](../../doc/models/level-3-default.md) | Optional | Level3 Default | Level3Default getLevel3Default() | setLevel3Default(Level3Default level3Default) |
| `CauSubscribeTypeId` | [`CauSubscribeTypeIdEnum`](../../doc/models/cau-subscribe-type-id-enum.md) | Optional | Cau Subscribe Type ID | CauSubscribeTypeIdEnum getCauSubscribeTypeId() | setCauSubscribeTypeId(CauSubscribeTypeIdEnum cauSubscribeTypeId) |
| `CauAccountNumber` | `String` | Optional | Cau Account Number<br><br>**Constraints**: *Minimum Length*: `32`, *Maximum Length*: `32`, *Pattern*: `^[a-zA-Z0-9\-]+$` | String getCauAccountNumber() | setCauAccountNumber(String cauAccountNumber) |
| `LocationBillingAccountId` | `String` | Optional | Location Billing Account ID | String getLocationBillingAccountId() | setLocationBillingAccountId(String locationBillingAccountId) |
| `ProductBillingGroupId` | `String` | Optional | Product Billing Group ID | String getProductBillingGroupId() | setProductBillingGroupId(String productBillingGroupId) |
| `AccountNumber` | `String` | Optional | Account number<br><br>**Constraints**: *Maximum Length*: `32`, *Pattern*: `^[a-zA-Z0-9\-_]+$` | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `RunAvsOnAccountvaultCreate` | `Boolean` | Optional | Run Avs On Accountvault Create | Boolean getRunAvsOnAccountvaultCreate() | setRunAvsOnAccountvaultCreate(Boolean runAvsOnAccountvaultCreate) |
| `AccountvaultExpireNotificationEmailEnable` | `Boolean` | Optional | Accountvault Expire Notification Email Enable | Boolean getAccountvaultExpireNotificationEmailEnable() | setAccountvaultExpireNotificationEmailEnable(Boolean accountvaultExpireNotificationEmailEnable) |
| `DebitAllowVoid` | `Boolean` | Optional | Debit Allow Void | Boolean getDebitAllowVoid() | setDebitAllowVoid(Boolean debitAllowVoid) |
| `QuickInvoiceTextToPay` | `Boolean` | Optional | Quick Invoice Text To Pay | Boolean getQuickInvoiceTextToPay() | setQuickInvoiceTextToPay(Boolean quickInvoiceTextToPay) |
| `AuthenticationCode` | `String` | Optional | Authentication Code | String getAuthenticationCode() | setAuthenticationCode(String authenticationCode) |
| `SmsEnable` | `Boolean` | Optional | SMS Enable | Boolean getSmsEnable() | setSmsEnable(Boolean smsEnable) |
| `VtShowCurrency` | `Boolean` | Optional | Vt Show Currency | Boolean getVtShowCurrency() | setVtShowCurrency(Boolean vtShowCurrency) |
| `ReceiptShowCurrency` | `Boolean` | Optional | Receipt Show Currency | Boolean getReceiptShowCurrency() | setReceiptShowCurrency(Boolean receiptShowCurrency) |
| `AllowBlindRefund` | `Boolean` | Optional | Allow Blind Refund | Boolean getAllowBlindRefund() | setAllowBlindRefund(Boolean allowBlindRefund) |
| `VtShowCompanyName` | `Boolean` | Optional | Vt Show Company Name | Boolean getVtShowCompanyName() | setVtShowCompanyName(Boolean vtShowCompanyName) |
| `ReceiptShowCompanyName` | `Boolean` | Optional | Receipt Show Company Name | Boolean getReceiptShowCompanyName() | setReceiptShowCompanyName(Boolean receiptShowCompanyName) |
| `BankFundedOnly` | `Boolean` | Optional | Bank Funded Only | Boolean getBankFundedOnly() | setBankFundedOnly(Boolean bankFundedOnly) |
| `RequireCvvOnKeyedCnp` | `Boolean` | Optional | Require CVV on keyed CNP | Boolean getRequireCvvOnKeyedCnp() | setRequireCvvOnKeyedCnp(Boolean requireCvvOnKeyedCnp) |
| `RequireCvvOnTokenizedCnp` | `Boolean` | Optional | Require CVV on tokenized CNP | Boolean getRequireCvvOnTokenizedCnp() | setRequireCvvOnTokenizedCnp(Boolean requireCvvOnTokenizedCnp) |
| `ShowSecondaryAmount` | `Boolean` | Optional | Show Retained Amount | Boolean getShowSecondaryAmount() | setShowSecondaryAmount(Boolean showSecondaryAmount) |
| `AllowSecondaryAmount` | `Boolean` | Optional | Allow Retained Amount | Boolean getAllowSecondaryAmount() | setAllowSecondaryAmount(Boolean allowSecondaryAmount) |
| `ShowGooglePay` | `Boolean` | Optional | Vt Require Street | Boolean getShowGooglePay() | setShowGooglePay(Boolean showGooglePay) |
| `ShowApplePay` | `Boolean` | Optional | Vt Require Street | Boolean getShowApplePay() | setShowApplePay(Boolean showApplePay) |
| `BatchRiskConfig` | [`BatchRiskConfig`](../../doc/models/batch-risk-config.md) | Optional | Batch Risk Config | BatchRiskConfig getBatchRiskConfig() | setBatchRiskConfig(BatchRiskConfig batchRiskConfig) |
| `CurrencyCode` | `Double` | Optional | Currency Code | Double getCurrencyCode() | setCurrencyCode(Double currencyCode) |
| `EnableAchValidation` | `Boolean` | Optional | Enable ACH Validation | Boolean getEnableAchValidation() | setEnableAchValidation(Boolean enableAchValidation) |
| `EnableAchRetry` | `Boolean` | Optional | Enable ACH Retry | Boolean getEnableAchRetry() | setEnableAchRetry(Boolean enableAchRetry) |
| `AllowSoftpos` | `Boolean` | Optional | Allow Soft POS | Boolean getAllowSoftpos() | setAllowSoftpos(Boolean allowSoftpos) |
| `Id` | `String` | Optional | User Reports ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `ReceiptLogo` | `String` | Optional | Receipt Logo | String getReceiptLogo() | setReceiptLogo(String receiptLogo) |
| `Active` | `Boolean` | Optional | Active | Boolean getActive() | setActive(Boolean active) |
| `Tz` | `String` | Optional | TZ | String getTz() | setTz(String tz) |
| `CurrentStan` | `Double` | Optional | Current Stan<br><br>**Default**: `1d` | Double getCurrentStan() | setCurrentStan(Double currentStan) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `ModifiedUserId` | `String` | Optional | Last User ID that updated the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getModifiedUserId() | setModifiedUserId(String modifiedUserId) |
| `ProductTransactionApiId` | `String` | Optional | Product Transaction API ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getProductTransactionApiId() | setProductTransactionApiId(String productTransactionApiId) |
| `TransactionAmountNotificationThreshold` | `Integer` | Optional | Transaction Amount Notification Treshold | Integer getTransactionAmountNotificationThreshold() | setTransactionAmountNotificationThreshold(Integer transactionAmountNotificationThreshold) |
| `IsSecondaryAmountAllowed` | `Boolean` | Optional | Allow Retained Amount | Boolean getIsSecondaryAmountAllowed() | setIsSecondaryAmountAllowed(Boolean isSecondaryAmountAllowed) |
| `FortisId` | `String` | Optional | - | String getFortisId() | setFortisId(String fortisId) |
| `ProductBillingGroupCode` | `String` | Optional | Product Billing Group Code | String getProductBillingGroupCode() | setProductBillingGroupCode(String productBillingGroupCode) |
| `CauSubscribeTypeCode` | [`CauSubscribeTypeCodeEnum`](../../doc/models/cau-subscribe-type-code-enum.md) | Optional | Cau Subscribe Type Code | CauSubscribeTypeCodeEnum getCauSubscribeTypeCode() | setCauSubscribeTypeCode(CauSubscribeTypeCodeEnum cauSubscribeTypeCode) |
| `MerchantCode` | `String` | Optional | Merchant Code<br><br>**Constraints**: *Maximum Length*: `24` | String getMerchantCode() | setMerchantCode(String merchantCode) |

## Example (as JSON)

```json
{
  "processor_version": "1_0_0",
  "title": "My terminal",
  "payment_method": "cc",
  "processor": "zgate",
  "mcc": "1111",
  "tax_surcharge_config": 2,
  "partner": "standalone",
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "vt_clerk_number": true,
  "vt_billing_phone": true,
  "vt_enable_tip": true,
  "ach_allow_debit": true,
  "ach_allow_credit": true,
  "ach_allow_refund": true,
  "vt_cvv": true,
  "vt_street": true,
  "vt_zip": true,
  "vt_order_num": true,
  "vt_enable": true,
  "receipt_show_contact_name": true,
  "display_avs": true,
  "card_type_visa": true,
  "card_type_mc": true,
  "card_type_disc": true,
  "card_type_amex": true,
  "card_type_diners": true,
  "card_type_jcb": true,
  "card_type_ebt": true,
  "allow_ebt_cash_benefit": true,
  "allow_ebt_food_stamp": true,
  "invoice_location": true,
  "allow_partial_authorization": true,
  "allow_recurring_partial_authorization": true,
  "auto_decline_cvv": true,
  "auto_decline_street": true,
  "auto_decline_zip": true,
  "split_payments_allow": true,
  "vt_show_custom_fields": true,
  "receipt_show_custom_fields": true,
  "vt_override_sales_tax_allowed": true,
  "vt_enable_sales_tax": true,
  "vt_require_zip": true,
  "vt_require_street": true,
  "auto_decline_cavv": true,
  "current_batch": 34,
  "paylink_allow": false,
  "quick_invoice_allow": false,
  "level3_allow": false,
  "payfac_enable": false,
  "enable_3ds": false,
  "sales_office_id": "11e95f8ec39de8fbdb0a4f1a",
  "hosted_payment_page_max_allowed": 5,
  "hosted_payment_page_allow": false,
  "surcharge_id": "11e95f8ec39de8fbdb0a4f1a",
  "allow_big_commerce": false,
  "cau_subscribe_type_id": 0,
  "location_billing_account_id": "11eb88b873980c64a21e5fd2",
  "product_billing_group_id": "nofees",
  "account_number": "12345678",
  "run_avs_on_accountvault_create": false,
  "accountvault_expire_notification_email_enable": false,
  "debit_allow_void": false,
  "quick_invoice_text_to_pay": false,
  "sms_enable": false,
  "vt_show_currency": true,
  "receipt_show_currency": false,
  "allow_blind_refund": false,
  "vt_show_company_name": false,
  "receipt_show_company_name": false,
  "bank_funded_only": false,
  "require_cvv_on_keyed_cnp": true,
  "require_cvv_on_tokenized_cnp": true,
  "show_secondary_amount": false,
  "allow_secondary_amount": false,
  "show_google_pay": true,
  "show_apple_pay": true,
  "currency_code": 840,
  "enable_ach_validation": false,
  "enable_ach_retry": false,
  "allow_softpos": false,
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "active": true,
  "current_stan": 1,
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "modified_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "product_transaction_api_id": "11e95f8ec39de8fbdb0a4f1a",
  "is_secondary_amount_allowed": false,
  "fortis_id": "8149742",
  "product_billing_group_code": "nofees",
  "cau_subscribe_type_code": 0,
  "industry_type": "lodging"
}
```

