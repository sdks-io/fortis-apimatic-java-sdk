
# V1 Wallet Provider Apple Pay Validate Merchant Request

## Structure

`V1WalletProviderApplePayValidateMerchantRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Url` | `String` | Required | Url obtained in the ApplePay button click event. Apple's URL that needs to be called to validate merchant. | String getUrl() | setUrl(String url) |
| `MerchantId` | `String` | Required | Merchant ID | String getMerchantId() | setMerchantId(String merchantId) |
| `DomainName` | `String` | Required | Domain Name | String getDomainName() | setDomainName(String domainName) |
| `DisplayName` | `String` | Required | Title | String getDisplayName() | setDisplayName(String displayName) |

## Example (as JSON)

```json
{
  "url": "https://apple-pay-gateway-cert.apple.com/paymentservices/startSession",
  "merchantId": "abc1234",
  "domainName": "website.domain.com",
  "displayName": "Sandwich Market"
}
```

