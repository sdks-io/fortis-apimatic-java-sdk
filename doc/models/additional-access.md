
# Additional Access

*This model accepts additional fields of type Object.*

## Structure

`AdditionalAccess`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `MerchantIcOptimization` | `Boolean` | Optional | - | Boolean getMerchantIcOptimization() | setMerchantIcOptimization(Boolean merchantIcOptimization) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "merchant_ic_optimization": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

