
# Document

Array of document objects.

## Structure

`Document`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `DocumentName` | `String` | Required | Array of bank account objects.<br><br>**Constraints**: *Maximum Length*: `32` | String getDocumentName() | setDocumentName(String documentName) |
| `DocumentData` | `String` | Required | Base64 encoded document content.<br><br>> Base64 encoded document content. | String getDocumentData() | setDocumentData(String documentData) |
| `MimeType` | `String` | Required | Mime type of document.<br><br>**Constraints**: *Maximum Length*: `20` | String getMimeType() | setMimeType(String mimeType) |

## Example (as JSON)

```json
{
  "document_name": "ImportantDoc.txt",
  "document_data": "alskj;asijia;eiom;weirj;iomj",
  "mime_type": "application/json"
}
```

