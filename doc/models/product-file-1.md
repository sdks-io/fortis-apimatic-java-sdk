
# Product File 1

## Structure

`ProductFile1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Title` | `String` | Optional | Title<br><br>**Constraints**: *Maximum Length*: `64` | String getTitle() | setTitle(String title) |
| `ProductFileCredentialId` | `String` | Optional | Product File Credential Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getProductFileCredentialId() | setProductFileCredentialId(String productFileCredentialId) |
| `FreeBytes` | `Double` | Optional | Free Bytes | Double getFreeBytes() | setFreeBytes(Double freeBytes) |
| `ByteIncrement` | `Double` | Optional | Byte Increment | Double getByteIncrement() | setByteIncrement(Double byteIncrement) |
| `MaxFileSizeBytes` | `Double` | Optional | Max File Size Bytes | Double getMaxFileSizeBytes() | setMaxFileSizeBytes(Double maxFileSizeBytes) |
| `IncrementCost` | `Double` | Optional | Increment Cost | Double getIncrementCost() | setIncrementCost(Double incrementCost) |
| `MonthlyFee` | `Integer` | Optional | Monthly Fee | Integer getMonthlyFee() | setMonthlyFee(Integer monthlyFee) |
| `FileExtAllowed` | `String` | Optional | File Ext Allowed<br><br>**Constraints**: *Maximum Length*: `64` | String getFileExtAllowed() | setFileExtAllowed(String fileExtAllowed) |
| `Container` | `String` | Optional | Container<br><br>**Constraints**: *Maximum Length*: `128` | String getContainer() | setContainer(String container) |
| `Id` | `String` | Optional | Product File Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `Active` | `Boolean` | Optional | Active | Boolean getActive() | setActive(Boolean active) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |

## Example (as JSON)

```json
{
  "title": "My terminal",
  "product_file_credential_id": "11e95f8ec39de8fbdb0a4f1a",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "active": true,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "free_bytes": 13.42,
  "byte_increment": 16.74,
  "max_file_size_bytes": 221.86
}
```

