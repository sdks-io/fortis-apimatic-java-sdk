
# Billing Address 5

Billing Address Object

## Structure

`BillingAddress5`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PostalCode` | `String` | Optional | The Zip or 'Postal Code' portion of the address associated with the Credit Card.<br><br>**Constraints**: *Minimum Length*: `3`, *Maximum Length*: `10`, *Pattern*: `^[a-zA-Z0-9\-\s]+$` | String getPostalCode() | setPostalCode(String postalCode) |
| `Street` | `String` | Optional | The Street portion of the address associated with the Credit Card.<br><br>**Constraints**: *Maximum Length*: `32`, *Pattern*: `^[\w\#\,\.\-\'\&\s\/]+$` | String getStreet() | setStreet(String street) |

## Example (as JSON)

```json
{
  "postal_code": "48375",
  "street": "street4"
}
```

