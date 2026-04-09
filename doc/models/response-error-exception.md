
# Response Error Exception

## Structure

`ResponseErrorException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | `String` | Optional | Message type | String getType() | setType(String type) |
| `Id` | `String` | Optional | Unique identifier for this API call | String getId() | setId(String id) |
| `StatusCode` | `Integer` | Optional | HTTP status code | Integer getStatusCode() | setStatusCode(Integer statusCode) |
| `Title` | `String` | Optional | Error title | String getTitle() | setTitle(String title) |
| `Detail` | [`Detail1`](../../doc/models/detail-1.md) | Optional | Error details | Detail1 getDetail() | setDetail(Detail1 detail) |
| `Meta` | `Object` | Optional | Object with additional error details | Object getMeta() | setMeta(Object meta) |

## Example (as JSON)

```json
{
  "type": "Error",
  "id": "c7f03d44-c966-4578-93ff-295f3ef6a467",
  "statusCode": 400,
  "title": "Bad Request",
  "detail": {
    "three_ds_server_trans_id": "three_ds_server_trans_id6",
    "acs_trans_id": "acs_trans_id8",
    "ds_trans_id": "ds_trans_id4",
    "error_code": "error_code4",
    "error_component": "error_component2"
  }
}
```

