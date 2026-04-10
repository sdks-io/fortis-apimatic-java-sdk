
# Mobile Phone

The mobile phone provided by the Cardholder. Refer to ITU-E.164 for additional information on format and length.

This field is required if available, unless market or regional mandate restricts sending this information.

*This model accepts additional fields of type Object.*

## Structure

`MobilePhone`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Cc` | `String` | Optional | Country Code of the phone<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `3` | String getCc() | setCc(String cc) |
| `Subscriber` | `String` | Optional | Subscriber section of the number<br><br>**Constraints**: *Maximum Length*: `15` | String getSubscriber() | setSubscriber(String subscriber) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "cc": "1",
  "subscriber": "5555555",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

