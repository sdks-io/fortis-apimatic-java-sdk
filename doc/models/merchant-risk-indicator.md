
# Merchant Risk Indicator

Contains purchase information

*This model accepts additional fields of type Object.*

## Structure

`MerchantRiskIndicator`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ShipIndicator` | [`ShipIndicator`](../../doc/models/ship-indicator.md) | Optional | - | ShipIndicator getShipIndicator() | setShipIndicator(ShipIndicator shipIndicator) |
| `DeliveryTimeframe` | [`DeliveryTimeframe`](../../doc/models/delivery-timeframe.md) | Optional | - | DeliveryTimeframe getDeliveryTimeframe() | setDeliveryTimeframe(DeliveryTimeframe deliveryTimeframe) |
| `DeliveryEmailAddress` | `String` | Optional | For electronic delivery, the email address to which the merchandise was delivered. | String getDeliveryEmailAddress() | setDeliveryEmailAddress(String deliveryEmailAddress) |
| `ReorderItemsInd` | [`ReorderItemsInd`](../../doc/models/reorder-items-ind.md) | Optional | - | ReorderItemsInd getReorderItemsInd() | setReorderItemsInd(ReorderItemsInd reorderItemsInd) |
| `PreOrderPurchaseInd` | [`PreOrderPurchaseInd`](../../doc/models/pre-order-purchase-ind.md) | Optional | - | PreOrderPurchaseInd getPreOrderPurchaseInd() | setPreOrderPurchaseInd(PreOrderPurchaseInd preOrderPurchaseInd) |
| `PreOrderDate` | `String` | Optional | For a pre-ordered purchase, the expected date that the merchandise will be available. Date format must be YYYYMMDD. | String getPreOrderDate() | setPreOrderDate(String preOrderDate) |
| `GiftCardAmount` | `Integer` | Optional | For prepaid or gift card purchase, the purchase amount total of prepaid or gift card(s) in major units (for example, USD 123.45 is 123). | Integer getGiftCardAmount() | setGiftCardAmount(Integer giftCardAmount) |
| `GiftCardCurr` | `String` | Optional | For prepaid or gift card purchase, the currency code of the card as defined in ISO 4217 except 955 - 964 and 999. | String getGiftCardCurr() | setGiftCardCurr(String giftCardCurr) |
| `GiftCardCount` | `Integer` | Optional | For prepaid or gift card purchase, total count of individual prepaid or gift cards/codes purchased.<br><br>**Constraints**: `>= 0`, `<= 99` | Integer getGiftCardCount() | setGiftCardCount(Integer giftCardCount) |
| `TransChar` | [`List<TransChar>`](../../doc/models/trans-char.md) | Optional | Available starting in EMV 3DS 2.3.1.1.  Indicates to the ACS specific transactions identified by the Merchant.<br><br>> 01 - Cryptocurrency transaction<br>> <br>> 02 - NFT transaction<br><br>**Constraints**: *Minimum Items*: `1`, *Maximum Items*: `2` | List<TransChar> getTransChar() | setTransChar(List<TransChar> transChar) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "delivery_email_address": "fortis@example.com",
  "ship_indicator": "05",
  "delivery_timeframe": "01",
  "reorder_items_ind": "01",
  "pre_order_purchase_ind": "01",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

