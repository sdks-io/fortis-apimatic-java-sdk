
# Response User

*This model accepts additional fields of type Object.*

## Structure

`ResponseUser`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type129`](../../doc/models/type-129.md) | Optional | - | Type129 getType() | setType(Type129 type) |
| `Data` | [`Data34`](../../doc/models/data-34.md) | Optional | - | Data34 getData() | setData(Data34 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "User",
  "data": {
    "account_number": "account_number0",
    "branding_domain_url": "branding_domain_url0",
    "cell_phone": "cell_phone6",
    "company_name": "company_name6",
    "contact_id": "contact_id4",
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

