
# Quick Invoice Setting

Quick Invoice Setting Information on `expand`

## Structure

`QuickInvoiceSetting`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `LocationApiId` | `String` | Optional | Location API ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationApiId() | setLocationApiId(String locationApiId) |
| `LocationId` | `String` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `QuickInvoiceTemplate` | `String` | Optional | Quick Invoice Template<br><br>**Constraints**: *Maximum Length*: `5000` | String getQuickInvoiceTemplate() | setQuickInvoiceTemplate(String quickInvoiceTemplate) |
| `DefaultAllowPartialPay` | `Boolean` | Optional | Default Quick Invoice Allow Partial Pay | Boolean getDefaultAllowPartialPay() | setDefaultAllowPartialPay(Boolean defaultAllowPartialPay) |
| `DefaultNotificationOnDueDate` | `Boolean` | Optional | Default Quick Invoice Notification On Due Date | Boolean getDefaultNotificationOnDueDate() | setDefaultNotificationOnDueDate(Boolean defaultNotificationOnDueDate) |
| `DefaultNotificationDaysAfterDueDate` | `Double` | Optional | Default Quick Invoice Notification Days After Due Date<br><br>**Constraints**: `>= 0`, `<= 60` | Double getDefaultNotificationDaysAfterDueDate() | setDefaultNotificationDaysAfterDueDate(Double defaultNotificationDaysAfterDueDate) |
| `DefaultNotificationDaysBeforeDueDate` | `Double` | Optional | Default Quick Invoice Notification Days Before Due Date<br><br>**Constraints**: `>= 0`, `<= 60` | Double getDefaultNotificationDaysBeforeDueDate() | setDefaultNotificationDaysBeforeDueDate(Double defaultNotificationDaysBeforeDueDate) |
| `ShowCustomFields` | `Boolean` | Optional | Show Custom Fields | Boolean getShowCustomFields() | setShowCustomFields(Boolean showCustomFields) |
| `Id` | `String` | Optional | Quick Invoice Settings ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |

## Example (as JSON)

```json
{
  "location_api_id": "11e95f8ec39de8fbdb0a4f1a",
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "quick_invoice_template": "<html>Template<html>",
  "default_allow_partial_pay": true,
  "default_notification_on_due_date": true,
  "default_notification_days_after_due_date": 7,
  "default_notification_days_before_due_date": 3,
  "show_custom_fields": false,
  "id": "11e95f8ec39de8fbdb0a4f1a"
}
```

