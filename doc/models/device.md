
# Device

Contains device information.

Available for supporting EMV 3DS 2.3.1 and later versions.

*This model accepts additional fields of type Object.*

## Structure

`Device`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `DeviceBindingStatus` | [`DeviceBindingStatus`](../../doc/models/device-binding-status.md) | Optional | - | DeviceBindingStatus getDeviceBindingStatus() | setDeviceBindingStatus(DeviceBindingStatus deviceBindingStatus) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "device_binding_status": "38",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

