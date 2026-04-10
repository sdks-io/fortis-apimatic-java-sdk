
# Quick Invoice View

*This model accepts additional fields of type Object.*

## Structure

`QuickInvoiceView`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `String` | Optional | Quick Invoice Views Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `QuickInvoiceId` | `String` | Optional | Quick Invoice ID<br><br>**Constraints**: *Maximum Length*: `24` | String getQuickInvoiceId() | setQuickInvoiceId(String quickInvoiceId) |
| `RemoteIp` | `String` | Optional | Remote Ip<br><br>**Constraints**: *Maximum Length*: `45` | String getRemoteIp() | setRemoteIp(String remoteIp) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "quick_invoice_id": "Quick Invoice ID",
  "created_ts": 1422040992,
  "remote_ip": "remote_ip8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

