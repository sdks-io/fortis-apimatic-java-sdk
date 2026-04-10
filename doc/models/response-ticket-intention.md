
# Response Ticket Intention

*This model accepts additional fields of type Object.*

## Structure

`ResponseTicketIntention`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type27`](../../doc/models/type-27.md) | Optional | - | Type27 getType() | setType(Type27 type) |
| `Data` | [`Data7`](../../doc/models/data-7.md) | Optional | - | Data7 getData() | setData(Data7 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "TicketIntention",
  "data": {
    "contact_id": "contact_id4",
    "contact_api_id": "contact_api_id4",
    "location_id": "location_id4",
    "product_transaction_id": "product_transaction_id4",
    "message": "message0",
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
```

