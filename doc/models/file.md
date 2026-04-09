
# File

## Structure

`File`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `File` | `Object` | Optional | File Object | Object getFile() | setFile(Object file) |
| `ResourceId` | `String` | Optional | Resource Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getResourceId() | setResourceId(String resourceId) |
| `Resource` | [`Resource2Enum`](../../doc/models/resource-2-enum.md) | Optional | Resource | Resource2Enum getResource() | setResource(Resource2Enum resource) |
| `ProductFileId` | `String` | Optional | Product File Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getProductFileId() | setProductFileId(String productFileId) |
| `FileCategoryId` | `String` | Optional | File Category Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getFileCategoryId() | setFileCategoryId(String fileCategoryId) |
| `VisibilityGroupId` | `String` | Optional | Visibility Group Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getVisibilityGroupId() | setVisibilityGroupId(String visibilityGroupId) |
| `FileDescription` | `String` | Optional | File Description<br><br>**Constraints**: *Maximum Length*: `128` | String getFileDescription() | setFileDescription(String fileDescription) |
| `Id` | `String` | Optional | Resource<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `FileName` | `String` | Optional | File Name | String getFileName() | setFileName(String fileName) |
| `FileExtension` | `String` | Optional | File Extension<br><br>**Constraints**: *Maximum Length*: `4` | String getFileExtension() | setFileExtension(String fileExtension) |
| `FileSizeBytes` | `Integer` | Optional | File Size Bytes | Integer getFileSizeBytes() | setFileSizeBytes(Integer fileSizeBytes) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |

## Example (as JSON)

```json
{
  "resource_id": "11e95f8ec39de8fbdb0a4f1a",
  "resource": "Contact",
  "product_file_id": "11e95f8ec39de8fbdb0a4f1a",
  "file_category_id": "11e95f8ec39de8fbdb0a4f1a",
  "visibility_group_id": "11e95f8ec39de8fbdb0a4f1a",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "file": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

