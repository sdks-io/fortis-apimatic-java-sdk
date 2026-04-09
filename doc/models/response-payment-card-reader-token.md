
# Response Payment Card Reader Token

## Structure

`ResponsePaymentCardReaderToken`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type58Enum`](../../doc/models/type-58-enum.md) | Optional | Resource Type<br><br>**Default**: `Type58Enum.PAYMENTCARDREADERTOKEN` | Type58Enum getType() | setType(Type58Enum type) |
| `Data` | [`Data17`](../../doc/models/data-17.md) | Optional | - | Data17 getData() | setData(Data17 data) |

## Example (as JSON)

```json
{
  "type": "PaymentCardReaderToken",
  "data": {
    "token": "token4"
  }
}
```

