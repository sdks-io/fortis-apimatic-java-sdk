
# Domain 1

*This model accepts additional fields of type Object.*

## Structure

`Domain1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Url` | `String` | Optional | URL<br><br>**Constraints**: *Maximum Length*: `64`, *Pattern*: `^[a-zA-Z0-9]+([\-\.]{1}[a-zA-Z0-9]+)*\.[a-zA-Z]{2,5}$` | String getUrl() | setUrl(String url) |
| `Title` | `String` | Optional | Domain Name<br><br>**Constraints**: *Maximum Length*: `64` | String getTitle() | setTitle(String title) |
| `Logo` | `String` | Optional | Logo<br><br>**Constraints**: *Maximum Length*: `64` | String getLogo() | setLogo(String logo) |
| `SupportEmail` | `String` | Optional | Support Email<br><br>**Constraints**: *Maximum Length*: `64` | String getSupportEmail() | setSupportEmail(String supportEmail) |
| `AllowContactSignup` | `Boolean` | Optional | Allow Contact Signup. | Boolean getAllowContactSignup() | setAllowContactSignup(Boolean allowContactSignup) |
| `AllowContactRegistration` | `Boolean` | Optional | Allow Contact Registration. | Boolean getAllowContactRegistration() | setAllowContactRegistration(Boolean allowContactRegistration) |
| `AllowContactLogin` | `Boolean` | Optional | Allow Contact Login. | Boolean getAllowContactLogin() | setAllowContactLogin(Boolean allowContactLogin) |
| `RegistrationFields` | [`List<RegistrationField>`](../../doc/models/registration-field.md) | Optional | Registration Fields | List<RegistrationField> getRegistrationFields() | setRegistrationFields(List<RegistrationField> registrationFields) |
| `CompanyName` | `String` | Optional | Company Name.<br><br>**Constraints**: *Maximum Length*: `32` | String getCompanyName() | setCompanyName(String companyName) |
| `NavColor` | `String` | Optional | Nav Color.<br><br>**Constraints**: *Maximum Length*: `7` | String getNavColor() | setNavColor(String navColor) |
| `ButtonPrimaryColor` | `String` | Optional | Button Primary Color.<br><br>**Constraints**: *Maximum Length*: `7` | String getButtonPrimaryColor() | setButtonPrimaryColor(String buttonPrimaryColor) |
| `LogoBackgroundColor` | `String` | Optional | Logo Background Color.<br><br>**Constraints**: *Maximum Length*: `7` | String getLogoBackgroundColor() | setLogoBackgroundColor(String logoBackgroundColor) |
| `IconBackgroundColor` | `String` | Optional | Icon Background Color.<br><br>**Constraints**: *Maximum Length*: `7` | String getIconBackgroundColor() | setIconBackgroundColor(String iconBackgroundColor) |
| `MenuTextBackgroundColor` | `String` | Optional | Menu Text Background Color<br><br>**Constraints**: *Maximum Length*: `7` | String getMenuTextBackgroundColor() | setMenuTextBackgroundColor(String menuTextBackgroundColor) |
| `MenuTextColor` | `String` | Optional | Menu Text Color.<br><br>**Constraints**: *Maximum Length*: `7` | String getMenuTextColor() | setMenuTextColor(String menuTextColor) |
| `RightMenuBackgroundColor` | `String` | Optional | Right Menu Background Color.<br><br>**Constraints**: *Maximum Length*: `7` | String getRightMenuBackgroundColor() | setRightMenuBackgroundColor(String rightMenuBackgroundColor) |
| `RightMenuTextColor` | `String` | Optional | Right Menu Text Color.<br><br>**Constraints**: *Maximum Length*: `7` | String getRightMenuTextColor() | setRightMenuTextColor(String rightMenuTextColor) |
| `ButtonPrimaryTextColor` | `String` | Optional | Button Primary Text Color.<br><br>**Constraints**: *Maximum Length*: `7` | String getButtonPrimaryTextColor() | setButtonPrimaryTextColor(String buttonPrimaryTextColor) |
| `NavLogo` | `String` | Optional | Nav Logo.<br><br>**Constraints**: *Maximum Length*: `256` | String getNavLogo() | setNavLogo(String navLogo) |
| `FavIcon` | `String` | Optional | Fav Icon.<br><br>**Constraints**: *Maximum Length*: `256` | String getFavIcon() | setFavIcon(String favIcon) |
| `AesKey` | `String` | Optional | Aes Key.<br><br>**Constraints**: *Maximum Length*: `255` | String getAesKey() | setAesKey(String aesKey) |
| `HelpText` | `String` | Optional | Help Text. | String getHelpText() | setHelpText(String helpText) |
| `EmailReplyTo` | `String` | Optional | Email Reply To. | String getEmailReplyTo() | setEmailReplyTo(String emailReplyTo) |
| `Email` | `String` | Optional | Email. | String getEmail() | setEmail(String email) |
| `CustomJavascript` | `String` | Optional | Custom Javascript.<br><br>**Constraints**: *Maximum Length*: `2048`, *Pattern*: `^<script\b[^>]*>([\s\S]*?)<\/script>$` | String getCustomJavascript() | setCustomJavascript(String customJavascript) |
| `CustomTheme` | `String` | Optional | Custom Theme<br><br>**Constraints**: *Maximum Length*: `48` | String getCustomTheme() | setCustomTheme(String customTheme) |
| `CustomCss` | `String` | Optional | Custom CSS<br><br>**Constraints**: *Maximum Length*: `2048` | String getCustomCss() | setCustomCss(String customCss) |
| `ContactUserDefaultEntryPage` | `Object` | Optional | - | Object getContactUserDefaultEntryPage() | setContactUserDefaultEntryPage(Object contactUserDefaultEntryPage) |
| `ContactUserDefaultAuthRoles` | `List<Object>` | Optional | Contact User Default Auth Role | List<Object> getContactUserDefaultAuthRoles() | setContactUserDefaultAuthRoles(List<Object> contactUserDefaultAuthRoles) |
| `CustomStylesheetUrl` | `String` | Optional | Custom Stylesheet URL<br><br>**Constraints**: *Maximum Length*: `256` | String getCustomStylesheetUrl() | setCustomStylesheetUrl(String customStylesheetUrl) |
| `Id` | `String` | Optional | Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "url": "fortispayrbyn9y.sandbox.zeamster.com",
  "title": "Test Brand Domain Title 2",
  "support_email": "email@domain.com",
  "allow_contact_signup": true,
  "allow_contact_registration": true,
  "allow_contact_login": true,
  "registration_fields": [
    "id",
    "email"
  ],
  "email_reply_to": "email@domain.com",
  "email": "email@domain.com",
  "custom_stylesheet_url": "https://127.0.0.1/receiver",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "logo": "logo2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

