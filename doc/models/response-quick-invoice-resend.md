
# Response Quick Invoice Resend

## Structure

`ResponseQuickInvoiceResend`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type61Enum`](../../doc/models/type-61-enum.md) | Optional | Resource Type<br><br>**Default**: `Type61Enum.QUICKINVOICERESEND` | Type61Enum getType() | setType(Type61Enum type) |
| `Data` | [`Data19`](../../doc/models/data-19.md) | Optional | - | Data19 getData() | setData(Data19 data) |

## Example (as JSON)

```json
{
  "type": "QuickInvoiceResend",
  "data": {
    "id": "id0",
    "email_log_id": "email_log_id2",
    "sms_log_id": "sms_log_id4",
    "success": false,
    "sms_success": false
  }
}
```

