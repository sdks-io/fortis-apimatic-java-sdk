
# List 14

*This model accepts additional fields of type Object.*

## Structure

`List14`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `LocationId` | `String` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getLocationId() | setLocationId(String locationId) |
| `DefaultProductTransactionId` | `String` | Optional | Product Transaction ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getDefaultProductTransactionId() | setDefaultProductTransactionId(String defaultProductTransactionId) |
| `TerminalApplicationId` | `String` | Optional | Terminal Application ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getTerminalApplicationId() | setTerminalApplicationId(String terminalApplicationId) |
| `TerminalCvmId` | `String` | Optional | Terminal CVM ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getTerminalCvmId() | setTerminalCvmId(String terminalCvmId) |
| `TerminalManufacturerCode` | [`TerminalManufacturerCode`](../../doc/models/terminal-manufacturer-code.md) | Optional | - | TerminalManufacturerCode getTerminalManufacturerCode() | setTerminalManufacturerCode(TerminalManufacturerCode terminalManufacturerCode) |
| `Title` | `String` | Optional | Terminal Name<br><br>**Constraints**: *Maximum Length*: `64` | String getTitle() | setTitle(String title) |
| `MacAddress` | `String` | Optional | Terminal MAC Address<br><br>**Constraints**: *Pattern*: `^([0-9a-fA-F]{2}[:-]?){5}([0-9a-fA-F]{2})$` | String getMacAddress() | setMacAddress(String macAddress) |
| `LocalIpAddress` | `String` | Optional | Terminal Local IP Address | String getLocalIpAddress() | setLocalIpAddress(String localIpAddress) |
| `Port` | `Integer` | Optional | Terminal Port<br><br>**Default**: `10009`<br><br>**Constraints**: `>= 0`, `<= 65535` | Integer getPort() | setPort(Integer port) |
| `SerialNumber` | `String` | Optional | Terminal Serial Number<br><br>**Constraints**: *Maximum Length*: `24`, *Pattern*: `^[a-zA-Z0-9]*$` | String getSerialNumber() | setSerialNumber(String serialNumber) |
| `TerminalNumber` | `String` | Optional | Terminal Number<br><br>**Constraints**: *Minimum Length*: `15`, *Maximum Length*: `15` | String getTerminalNumber() | setTerminalNumber(String terminalNumber) |
| `TerminalTimeouts` | [`TerminalTimeouts1`](../../doc/models/terminal-timeouts-1.md) | Optional | - | TerminalTimeouts1 getTerminalTimeouts() | setTerminalTimeouts(TerminalTimeouts1 terminalTimeouts) |
| `TipPercents` | [`TipPercents1`](../../doc/models/tip-percents-1.md) | Optional | - | TipPercents1 getTipPercents() | setTipPercents(TipPercents1 tipPercents) |
| `LocationApiId` | `String` | Optional | Location Api ID<br><br>**Constraints**: *Maximum Length*: `64` | String getLocationApiId() | setLocationApiId(String locationApiId) |
| `TerminalApiId` | `String` | Optional | Terminal Api ID<br><br>**Constraints**: *Maximum Length*: `64` | String getTerminalApiId() | setTerminalApiId(String terminalApiId) |
| `HeaderLine1` | `String` | Optional | Header Line 1<br><br>**Constraints**: *Maximum Length*: `32` | String getHeaderLine1() | setHeaderLine1(String headerLine1) |
| `HeaderLine2` | `String` | Optional | Header Line 2<br><br>**Constraints**: *Maximum Length*: `32` | String getHeaderLine2() | setHeaderLine2(String headerLine2) |
| `HeaderLine3` | `String` | Optional | Header Line 3<br><br>**Constraints**: *Maximum Length*: `32` | String getHeaderLine3() | setHeaderLine3(String headerLine3) |
| `HeaderLine4` | `String` | Optional | Header Line 4<br><br>**Constraints**: *Maximum Length*: `32` | String getHeaderLine4() | setHeaderLine4(String headerLine4) |
| `HeaderLine5` | `String` | Optional | Header Line 5<br><br>**Constraints**: *Maximum Length*: `32` | String getHeaderLine5() | setHeaderLine5(String headerLine5) |
| `TrailerLine1` | `String` | Optional | Trailer Line 1<br><br>**Constraints**: *Maximum Length*: `32` | String getTrailerLine1() | setTrailerLine1(String trailerLine1) |
| `TrailerLine2` | `String` | Optional | Trailer Line 2<br><br>**Constraints**: *Maximum Length*: `32` | String getTrailerLine2() | setTrailerLine2(String trailerLine2) |
| `TrailerLine3` | `String` | Optional | Trailer Line 3<br><br>**Constraints**: *Maximum Length*: `32` | String getTrailerLine3() | setTrailerLine3(String trailerLine3) |
| `TrailerLine4` | `String` | Optional | Trailer Line 4<br><br>**Constraints**: *Maximum Length*: `32` | String getTrailerLine4() | setTrailerLine4(String trailerLine4) |
| `TrailerLine5` | `String` | Optional | Trailer Line 5<br><br>**Constraints**: *Maximum Length*: `32` | String getTrailerLine5() | setTrailerLine5(String trailerLine5) |
| `DefaultCheckin` | `String` | Optional | Default Checkin<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getDefaultCheckin() | setDefaultCheckin(String defaultCheckin) |
| `DefaultCheckout` | `String` | Optional | Default Checkout<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | String getDefaultCheckout() | setDefaultCheckout(String defaultCheckout) |
| `DefaultRoomRate` | `Integer` | Optional | Default Room Rate<br><br>**Constraints**: `>= 0`, `<= 100` | Integer getDefaultRoomRate() | setDefaultRoomRate(Integer defaultRoomRate) |
| `DefaultRoomNumber` | `String` | Optional | Default Room Number<br><br>**Constraints**: *Maximum Length*: `12` | String getDefaultRoomNumber() | setDefaultRoomNumber(String defaultRoomNumber) |
| `Debit` | `Boolean` | Optional | Debit | Boolean getDebit() | setDebit(Boolean debit) |
| `Emv` | `Boolean` | Optional | EMV | Boolean getEmv() | setEmv(Boolean emv) |
| `CashbackEnable` | `Boolean` | Optional | Cashback Enable | Boolean getCashbackEnable() | setCashbackEnable(Boolean cashbackEnable) |
| `PrintEnable` | `Boolean` | Optional | Print Enable | Boolean getPrintEnable() | setPrintEnable(Boolean printEnable) |
| `SigCaptureEnable` | `Boolean` | Optional | Sig Capture Enable | Boolean getSigCaptureEnable() | setSigCaptureEnable(Boolean sigCaptureEnable) |
| `IsProvisioned` | `Boolean` | Optional | Is Provisioned | Boolean getIsProvisioned() | setIsProvisioned(Boolean isProvisioned) |
| `TipEnable` | `Boolean` | Optional | Tip Enable | Boolean getTipEnable() | setTipEnable(Boolean tipEnable) |
| `ValidatedDecryption` | `Boolean` | Optional | Validated Decryption | Boolean getValidatedDecryption() | setValidatedDecryption(Boolean validatedDecryption) |
| `CommunicationType` | `Object` | Optional | - | Object getCommunicationType() | setCommunicationType(Object communicationType) |
| `Active` | `Boolean` | Optional | Active | Boolean getActive() | setActive(Boolean active) |
| `Id` | `String` | Optional | Terminal ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `LastRegistrationTs` | `Integer` | Optional | Modified Time Stamp | Integer getLastRegistrationTs() | setLastRegistrationTs(Integer lastRegistrationTs) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `ModifiedUserId` | `String` | Optional | Last User ID that updated the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getModifiedUserId() | setModifiedUserId(String modifiedUserId) |
| `Location` | [`Location18`](../../doc/models/location-18.md) | Optional | - | Location18 getLocation() | setLocation(Location18 location) |
| `CreatedUser` | [`User9`](../../doc/models/user-9.md) | Optional | - | User9 getCreatedUser() | setCreatedUser(User9 createdUser) |
| `TerminalApplication` | [`TerminalApplication1`](../../doc/models/terminal-application-1.md) | Optional | - | TerminalApplication1 getTerminalApplication() | setTerminalApplication(TerminalApplication1 terminalApplication) |
| `Changelogs` | [`List<Changelog>`](../../doc/models/changelog.md) | Optional | Changelog Information on `expand` | List<Changelog> getChangelogs() | setChangelogs(List<Changelog> changelogs) |
| `TerminalRouters` | [`List<TerminalRouter>`](../../doc/models/terminal-router.md) | Optional | Terminal Router Information on `expand` | List<TerminalRouter> getTerminalRouters() | setTerminalRouters(List<TerminalRouter> terminalRouters) |
| `HasTerminalRouters` | `Boolean` | Optional | Has Terminal Router Information on `expand` | Boolean getHasTerminalRouters() | setHasTerminalRouters(Boolean hasTerminalRouters) |
| `TerminalCvm` | [`TerminalCvm1`](../../doc/models/terminal-cvm-1.md) | Optional | - | TerminalCvm1 getTerminalCvm() | setTerminalCvm(TerminalCvm1 terminalCvm) |
| `TerminalManufacturer` | [`TerminalManufacturer1`](../../doc/models/terminal-manufacturer-1.md) | Optional | - | TerminalManufacturer1 getTerminalManufacturer() | setTerminalManufacturer(TerminalManufacturer1 terminalManufacturer) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "default_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "terminal_application_id": "11e95f8ec39de8fbdb0a4f1a",
  "terminal_cvm_id": "11e95f8ec39de8fbdb0a4f1a",
  "title": "My terminal",
  "mac_address": "3D:F2:C9:A6:B3:4F",
  "local_ip_address": "192.168.0.10",
  "port": 10009,
  "serial_number": "1234567890",
  "terminal_number": "973456789012367",
  "header_line_1": "line 1 sample",
  "header_line_2": "line 2 sample",
  "header_line_3": "line 3 sample",
  "header_line_4": "line 4 sample",
  "header_line_5": "line 5 sample",
  "trailer_line_1": "trailer 1 sample",
  "trailer_line_2": "trailer 2 sample",
  "trailer_line_3": "trailer 3 sample",
  "trailer_line_4": "trailer 4 sample",
  "trailer_line_5": "trailer 5 sample",
  "default_checkin": "2021-12-01",
  "default_checkout": "2021-12-01",
  "default_room_rate": 56,
  "default_room_number": "303",
  "debit": false,
  "emv": false,
  "cashback_enable": false,
  "print_enable": false,
  "sig_capture_enable": false,
  "is_provisioned": false,
  "tip_enable": false,
  "validated_decryption": false,
  "active": true,
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "last_registration_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "modified_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "has_terminal_routers": true,
  "terminal_manufacturer_code": "4",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

