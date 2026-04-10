
# Meta

*This model accepts additional fields of type Object.*

## Structure

`Meta`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Details` | [`List<Detail>`](../../doc/models/detail.md) | Optional | Error detail | List<Detail> getDetails() | setDetails(List<Detail> details) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "details": [
    {
      "message": "message0",
      "path": [
        "path6"
      ],
      "type": "type0",
      "context": {
        "key": "key2",
        "label": "label2",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

