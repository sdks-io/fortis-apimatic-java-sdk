
# Pricing Element

Array of pricing items from template to be changed.

*This model accepts additional fields of type Object.*

## Structure

`PricingElement`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ItemId` | `int` | Required | Item ID.<br><br>**Constraints**: `>= 0` | int getItemId() | setItemId(int itemId) |
| `ItemValue` | `double` | Required | Item value.<br><br>**Constraints**: `>= 0` | double getItemValue() | setItemValue(double itemValue) |
| `ItemTerm` | `int` | Required | Item term.<br><br>**Constraints**: `>= 0` | int getItemTerm() | setItemTerm(int itemTerm) |
| `ItemDescription` | `String` | Optional | Item desciption.<br><br>**Constraints**: *Maximum Length*: `100` | String getItemDescription() | setItemDescription(String itemDescription) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "item_id": 5,
  "item_value": 1.5,
  "item_term": 2,
  "item_description": "AVS fee.",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

