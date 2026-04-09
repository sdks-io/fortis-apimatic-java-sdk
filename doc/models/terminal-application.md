
# Terminal Application

Terminal Application Information on `expand`

## Structure

`TerminalApplication`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Standalone` | `Boolean` | Optional | Standalone | Boolean getStandalone() | setStandalone(Boolean standalone) |
| `EmvCapable` | `Boolean` | Optional | Emv Capable | Boolean getEmvCapable() | setEmvCapable(Boolean emvCapable) |
| `NfcCapable` | `Boolean` | Optional | Nfc Capable | Boolean getNfcCapable() | setNfcCapable(Boolean nfcCapable) |
| `PinCapable` | `Boolean` | Optional | Pin Capable | Boolean getPinCapable() | setPinCapable(Boolean pinCapable) |
| `PrintCapable` | `Boolean` | Optional | Print Capable | Boolean getPrintCapable() | setPrintCapable(Boolean printCapable) |
| `MsrCapable` | `Boolean` | Optional | Msr Capable | Boolean getMsrCapable() | setMsrCapable(Boolean msrCapable) |
| `SigCaptureCapable` | `Boolean` | Optional | Sig Capture Capable | Boolean getSigCaptureCapable() | setSigCaptureCapable(Boolean sigCaptureCapable) |
| `MposTerminal` | `Boolean` | Optional | Mpos Terminal | Boolean getMposTerminal() | setMposTerminal(Boolean mposTerminal) |
| `Title` | `String` | Optional | Title<br><br>**Constraints**: *Maximum Length*: `48` | String getTitle() | setTitle(String title) |
| `Description` | `String` | Optional | Description<br><br>**Constraints**: *Maximum Length*: `256` | String getDescription() | setDescription(String description) |
| `Id` | `String` | Optional | Terminal Application Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |

## Example (as JSON)

```json
{
  "standalone": true,
  "emv_capable": true,
  "nfc_capable": false,
  "pin_capable": true,
  "print_capable": false,
  "msr_capable": true,
  "sig_capture_capable": false,
  "mpos_terminal": false,
  "title": "Ingenico Link2500",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a"
}
```

