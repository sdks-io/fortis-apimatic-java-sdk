
# Response Transaction

*This model accepts additional fields of type Object.*

## Structure

`ResponseTransaction`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`Type110`](../../doc/models/type-110.md) | Optional | - | Type110 getType() | setType(Type110 type) |
| `Data` | [`Data27`](../../doc/models/data-27.md) | Optional | - | Data27 getData() | setData(Data27 data) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "type": "Transaction",
  "data": {
    "additional_amounts": [
      {
        "type": {
          "key1": "val1",
          "key2": "val2"
        },
        "amount": 6,
        "account_type": {
          "key1": "val1",
          "key2": "val2"
        },
        "currency": 154.64,
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      {
        "type": {
          "key1": "val1",
          "key2": "val2"
        },
        "amount": 6,
        "account_type": {
          "key1": "val1",
          "key2": "val2"
        },
        "currency": 154.64,
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      }
    ],
    "billing_address": {
      "city": "city2",
      "state": "state6",
      "postal_code": "postal_code0",
      "street": "street8",
      "phone": "phone2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    "checkin_date": "checkin_date2",
    "checkout_date": "checkout_date4",
    "clerk_number": "clerk_number4",
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

