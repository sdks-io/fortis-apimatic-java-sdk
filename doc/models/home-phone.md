
# Home Phone

The home phone provided by the Cardholder. Refer to ITU-E.164 for additional information on format and length.

This field is required if available, unless market or regional mandate restricts sending this information.

## Structure

`HomePhone`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Cc` | `String` | Optional | Country Code of the phone<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `3` | String getCc() | setCc(String cc) |
| `Subscriber` | `String` | Optional | Subscriber section of the number<br><br>**Constraints**: *Maximum Length*: `15` | String getSubscriber() | setSubscriber(String subscriber) |

## Example (as JSON)

```json
{
  "cc": "cc6",
  "subscriber": "subscriber8"
}
```

