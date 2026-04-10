
# Merchant List

*This model accepts additional fields of type Object.*

## Structure

`MerchantList`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `MerchantNameListed` | `String` | Required | Name of the listed merchant as used in the authorization message as defined in ISO 8583.<br><br>**Constraints**: *Maximum Length*: `40` | String getMerchantNameListed() | setMerchantNameListed(String merchantNameListed) |
| `AcquirerMerchantIdListed` | `String` | Optional | Acquirer-assigned Merchant Listed Identifier.<br>This may be the same value that is used in authorisation requests sent on behalf of the 3DS Requestor and is represented in ISO 8583 formatting requirements.<br><br>**Constraints**: *Maximum Length*: `15` | String getAcquirerMerchantIdListed() | setAcquirerMerchantIdListed(String acquirerMerchantIdListed) |
| `MerchantAmount` | `String` | Optional | Purchase amount for the merchant in minor units of currency with all punctuation removed.<br>When used in conjunction with the Purchase Currency Exponent field, proper punctuation can be calculated.<br><br>**Constraints**: *Maximum Length*: `48` | String getMerchantAmount() | setMerchantAmount(String merchantAmount) |
| `MerchantCurrency` | `String` | Optional | Currency Code in which purchase Merchant Amount is expressed. Must be provided as ISO 4217 three-digit currency code except values 955-964 and 999.<br><br>**Constraints**: *Minimum Length*: `3`, *Maximum Length*: `3` | String getMerchantCurrency() | setMerchantCurrency(String merchantCurrency) |
| `MerchantExponent` | `String` | Optional | Minor units of Merchant Currency as specified in the ISO 4217 currency exponent.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `1` | String getMerchantExponent() | setMerchantExponent(String merchantExponent) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "merchant_name_listed": "merchant_name_listed4",
  "acquirer_merchant_id_listed": "acquirer_merchant_id_listed4",
  "merchant_amount": "merchant_amount2",
  "merchant_currency": "merchant_currency0",
  "merchant_exponent": "merchant_exponent4",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

