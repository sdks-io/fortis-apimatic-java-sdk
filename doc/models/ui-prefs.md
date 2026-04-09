
# Ui Prefs

Ui Prefs

## Structure

`UiPrefs`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `EntryPage` | `String` | Optional | Ui Prefs Entry Page | String getEntryPage() | setEntryPage(String entryPage) |
| `PageSize` | `Integer` | Optional | Ui Prefs Page Size<br><br>**Constraints**: `>= 0`, `<= 99` | Integer getPageSize() | setPageSize(Integer pageSize) |
| `ReportExportType` | [`ReportExportTypeEnum`](../../doc/models/report-export-type-enum.md) | Optional | Ui Prefs Export Type | ReportExportTypeEnum getReportExportType() | setReportExportType(ReportExportTypeEnum reportExportType) |
| `ProcessMethod` | [`ProcessMethodEnum`](../../doc/models/process-method-enum.md) | Optional | Ui Prefs Process Method | ProcessMethodEnum getProcessMethod() | setProcessMethod(ProcessMethodEnum processMethod) |
| `DefaultTerminal` | `String` | Optional | Ui Prefs Default Termianl<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getDefaultTerminal() | setDefaultTerminal(String defaultTerminal) |

## Example (as JSON)

```json
{
  "entry_page": "dashboard",
  "page_size": 2,
  "report_export_type": "csv",
  "process_method": "virtual_terminal",
  "default_terminal": "11e95f8ec39de8fbdb0a4f1a"
}
```

