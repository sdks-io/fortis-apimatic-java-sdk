
# Home Phone 2

*This model accepts additional fields of type Object.*

## Structure

`HomePhone2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Cc` | `String` | Optional | Country Code of the phone<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `3` | String getCc() | setCc(String cc) |
| `Subscriber` | `String` | Optional | Subscriber section of the number<br><br>**Constraints**: *Maximum Length*: `15` | String getSubscriber() | setSubscriber(String subscriber) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "cc": "cc2",
  "subscriber": "subscriber4",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

