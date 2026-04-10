
# Data 12

*This model accepts additional fields of type Object.*

## Structure

`Data12`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ThreeDsServerTransId` | `String` | Optional | Universally unique transaction identifier assigned by the 3DS Server to identify a single transaction. It has the same value as the corresponding received authentication request. This value has 36 characters in a format defined in IETF RFC 4122.<br><br>**Constraints**: *Maximum Length*: `36` | String getThreeDsServerTransId() | setThreeDsServerTransId(String threeDsServerTransId) |
| `AcsUrl` | `String` | Optional | Fully qualified URL of the ACS in case the authentication response message indicates that further Cardholder interaction is required to complete the authentication.<br><br>This field is only present in Browser flow. | String getAcsUrl() | setAcsUrl(String acsUrl) |
| `TransactionStatus` | [`TransactionStatus`](../../doc/models/transaction-status.md) | Optional | - | TransactionStatus getTransactionStatus() | setTransactionStatus(TransactionStatus transactionStatus) |
| `AuthenticationValue` | `String` | Optional | Payment System-specific value provided as part of the ACS registration for each supported DS. Authentication Value may be used to provide proof of authentication. | String getAuthenticationValue() | setAuthenticationValue(String authenticationValue) |
| `Eci` | `String` | Optional | Payment System-specific value provided by the ACS to indicate the results of the attempt to authenticate the Cardholder. | String getEci() | setEci(String eci) |
| `DsTransId` | `String` | Optional | Universally unique transaction identifier assigned by the DS to identify a single transaction. | String getDsTransId() | setDsTransId(String dsTransId) |
| `AcsTransId` | `String` | Optional | Universally unique transaction identifier assigned by the ACS to identify a single transaction. | String getAcsTransId() | setAcsTransId(String acsTransId) |
| `MessageVersion` | `String` | Optional | Protocol version identifier This shall be the Protocol Version Number of the specification utilised by the system creating this message.<br>The Message Version Number is set by the 3DS Server which originates the protocol with the AReq message. The Message Version Number does not change during a 3DS transaction. | String getMessageVersion() | setMessageVersion(String messageVersion) |
| `AcsChallengeMandated` | [`AcsChallengeMandated`](../../doc/models/acs-challenge-mandated.md) | Optional | - | AcsChallengeMandated getAcsChallengeMandated() | setAcsChallengeMandated(AcsChallengeMandated acsChallengeMandated) |
| `PurchaseDate` | `String` | Optional | Date and time of the purchase, converted into UTC. The field is limited to 14 characters, formatted as YYYYMMDDHHMMSS.<br><br>**Constraints**: *Maximum Length*: `14` | String getPurchaseDate() | setPurchaseDate(String purchaseDate) |
| `Base64EncodedChallengeRequest` | `String` | Optional | Base64-encoded Challenge Request object in case the authentication response message indicates that further Cardholder interaction is required to complete the authentication. | String getBase64EncodedChallengeRequest() | setBase64EncodedChallengeRequest(String base64EncodedChallengeRequest) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "three_ds_server_trans_id": "ea0c9973-4cd0-4f9f-83b3-609bf22c69e7",
  "acs_url": "https://api.sandbox.fortis.tech/v1/acs/challenge",
  "ds_trans_id": "278c7508-cac6-4233-902d-b90f31f741c6",
  "acs_trans_id": "d7c1ee99-9478-44a6-b1f2-391e29c6b340",
  "message_version": "2.2.0",
  "purchase_date": "20240509111532",
  "base64_encoded_challenge_request": "eyJtZXNzYWdlVHlwZSI6IkNSZXEiLCJ0aHJlZURTU2VydmVyVHJhbnNJRCI6ImVhMGM5OTczLTRjZDAtNGY5Zi04M2IzLTYwOWJmMjJjNjllNyIsImFjc1RyYW5zSUQiOiIwNWViNTE2OS02ZTFkLTQ5NTMtYWQ3NC1hZWU5YmQ4ZTc1YmIiLCJjaGFsbGVuZ2VXaW5kb3dTaXplIjoiMDEiLCJtZXNzYWdlVmVyc2lvbiI6IjIuMi4wIn0=",
  "transaction_status": "R",
  "authentication_value": "authentication_value0",
  "eci": "eci8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

