
# Addon

## Structure

`Addon`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Title` | `String` | Optional | Title<br><br>**Constraints**: *Maximum Length*: `24` | String getTitle() | setTitle(String title) |
| `Secret` | `String` | Optional | Secret<br><br>**Constraints**: *Maximum Length*: `36` | String getSecret() | setSecret(String secret) |
| `IframeUrl` | `String` | Optional | Iframe URL<br><br>**Constraints**: *Maximum Length*: `512` | String getIframeUrl() | setIframeUrl(String iframeUrl) |
| `LocationSetupUrl` | `String` | Optional | Location Setup URL<br><br>**Constraints**: *Maximum Length*: `512` | String getLocationSetupUrl() | setLocationSetupUrl(String locationSetupUrl) |
| `UserSetupUrl` | `String` | Optional | User Setup URL<br><br>**Constraints**: *Maximum Length*: `512` | String getUserSetupUrl() | setUserSetupUrl(String userSetupUrl) |
| `EncryptUrlParams` | `Boolean` | Optional | Encrypt URL Params | Boolean getEncryptUrlParams() | setEncryptUrlParams(Boolean encryptUrlParams) |

## Example (as JSON)

```json
{
  "encrypt_url_params": true,
  "title": "title4",
  "secret": "secret4",
  "iframe_url": "iframe_url4",
  "location_setup_url": "location_setup_url0",
  "user_setup_url": "user_setup_url6"
}
```

