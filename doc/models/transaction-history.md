
# Transaction History

*This model accepts additional fields of type Object.*

## Structure

`TransactionHistory`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TransactionId` | `String` | Optional | Transaction ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getTransactionId() | setTransactionId(String transactionId) |
| `Id` | `String` | Optional | Transaction Histories ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `StatusId` | `Integer` | Optional | Status ID | Integer getStatusId() | setStatusId(Integer statusId) |
| `EventDateTs` | `Integer` | Optional | Event Date TS | Integer getEventDateTs() | setEventDateTs(Integer eventDateTs) |
| `LocationId` | `String` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "status_id": 101,
  "event_date_ts": 1422040992,
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

