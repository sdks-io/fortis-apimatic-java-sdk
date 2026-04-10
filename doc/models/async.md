
# Async

Do not store the Async Code for long term use, it expires after 30 days.

*This model accepts additional fields of type Object.*

## Structure

`Async`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Code` | `UUID` | Optional | A [UUID v4](https://datatracker.ietf.org/doc/html/rfc4122) that's unique for the Async Request | UUID getCode() | setCode(UUID code) |
| `Link` | `String` | Optional | Link to the status check endpoint | String getLink() | setLink(String link) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "code": "406c66c3-21cb-47fb-80fc-843bc42507fb",
  "link": "/v1/async/status/406c66c3-21cb-47fb-80fc-843bc42507fb",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

