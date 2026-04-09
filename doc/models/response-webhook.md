
# Response Webhook

## Structure

`ResponseWebhook`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type138Enum`](../../doc/models/type-138-enum.md) | Optional | Resource Type<br><br>**Default**: `Type138Enum.WEBHOOK` | Type138Enum getType() | setType(Type138Enum type) |
| `Data` | [`Data39`](../../doc/models/data-39.md) | Optional | - | Data39 getData() | setData(Data39 data) |

## Example (as JSON)

```json
{
  "type": "Webhook",
  "data": {
    "attempt_interval": 300,
    "basic_auth_username": "basic_auth_username8",
    "basic_auth_password": "basic_auth_password0",
    "expands": "expands2",
    "format": "api-default"
  }
}
```

