
# Device 1

*This model accepts additional fields of type Object.*

## Structure

`Device1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `DeviceBindingStatus` | [`DeviceBindingStatus`](../../doc/models/device-binding-status.md) | Optional | - | DeviceBindingStatus getDeviceBindingStatus() | setDeviceBindingStatus(DeviceBindingStatus deviceBindingStatus) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "device_binding_status": "01",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

