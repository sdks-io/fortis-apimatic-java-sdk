
# Forecast

Forecast Information on `expand`

*This model accepts additional fields of type Object.*

## Structure

`Forecast`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `String` | Optional | ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `RecurringId` | `String` | Optional | Recurring ID | String getRecurringId() | setRecurringId(String recurringId) |
| `RecurringType` | `Double` | Optional | Recurring Type | Double getRecurringType() | setRecurringType(Double recurringType) |
| `Amount` | `Double` | Optional | Amount | Double getAmount() | setAmount(Double amount) |
| `Month` | `String` | Optional | Month | String getMonth() | setMonth(String month) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "recurring_id": "Recurring ID",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "recurring_type": 118.0,
  "amount": 7.04,
  "month": "month2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

