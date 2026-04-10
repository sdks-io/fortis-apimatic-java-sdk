
# V1 Recurrings Skip Payment Request

*This model accepts additional fields of type Object.*

## Structure

`V1RecurringsSkipPaymentRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `SkipCount` | `int` | Required | Skip Count<br><br>**Constraints**: `>= 1`, `<= 99` | int getSkipCount() | setSkipCount(int skipCount) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "skip_count": 7,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

