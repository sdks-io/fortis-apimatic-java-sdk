
# V1 Recurrings Defer Payment Request

*This model accepts additional fields of type Object.*

## Structure

`V1RecurringsDeferPaymentRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `DeferCount` | `int` | Required | Defer Count<br><br>**Constraints**: `>= 1`, `<= 99` | int getDeferCount() | setDeferCount(int deferCount) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "defer_count": 5,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

