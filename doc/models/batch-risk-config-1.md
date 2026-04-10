
# Batch Risk Config 1

*This model accepts additional fields of type Object.*

## Structure

`BatchRiskConfig1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `BlindRefundTotalCount` | `Integer` | Optional | Blind Refund Total Count<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getBlindRefundTotalCount() | setBlindRefundTotalCount(Integer blindRefundTotalCount) |
| `BlindRefundMaxAmount` | `Integer` | Optional | Blind Refund Max Amount<br><br>**Constraints**: `>= 0`, `<= 999999999` | Integer getBlindRefundMaxAmount() | setBlindRefundMaxAmount(Integer blindRefundMaxAmount) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "blind_refund_total_count": 66,
  "blind_refund_max_amount": 128,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

