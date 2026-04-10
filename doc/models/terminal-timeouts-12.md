
# Terminal Timeouts 12

The following options outlines some configurable timeout values that can be used to customize the experience at the terminal for the cardholder.

> These timeouts are specific to Ingenico devices only.

*This model accepts additional fields of type Object.*

## Structure

`TerminalTimeouts12`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `CardEntryTimeout` | `Integer` | Optional | How long to wait for input from cardholder.<br><br>> Message on timeout:<br>> Card Entry Timeout<br><br>**Constraints**: `>= 20`, `<= 120` | Integer getCardEntryTimeout() | setCardEntryTimeout(Integer cardEntryTimeout) |
| `DeviceTermsPromptTimeout` | `Integer` | Optional | How long the terms will be displayed on the device.<br><br>> Message on timeout:<br>> Timeout waiting for Customer<br><br>**Constraints**: `>= 5`, `<= 300` | Integer getDeviceTermsPromptTimeout() | setDeviceTermsPromptTimeout(Integer deviceTermsPromptTimeout) |
| `OverallTimeout` | `Integer` | Optional | How long to wait for response from /v2/routertransactions endpoint.<br><br>> Message on timeout:<br>> Overall Request Timeout<br><br>**Constraints**: `>= 30`, `<= 300` | Integer getOverallTimeout() | setOverallTimeout(Integer overallTimeout) |
| `PinEntryTimeout` | `Integer` | Optional | How long to wait for pin entry by cardholder.<br><br>> Message on timeout:<br>> Pin Entry Timeout<br><br>**Constraints**: `>= 20`, `<= 50` | Integer getPinEntryTimeout() | setPinEntryTimeout(Integer pinEntryTimeout) |
| `SignatureInputTimeout` | `Integer` | Optional | How long to wait for first "touch" to signature.<br><br>> Message on timeout:<br>> Signature Input Timeout<br><br>**Constraints**: `>= 10`, `<= 50` | Integer getSignatureInputTimeout() | setSignatureInputTimeout(Integer signatureInputTimeout) |
| `SignatureSubmitTimeout` | `Integer` | Optional | How long to wait for signature to be submitted.<br><br>> Message on timeout:<br>> Signature Storage Timeout<br><br>**Constraints**: `>= 20`, `<= 50` | Integer getSignatureSubmitTimeout() | setSignatureSubmitTimeout(Integer signatureSubmitTimeout) |
| `StatusDisplayTime` | `Integer` | Optional | How long the approve/decline status message stays on screen.<br><br>> Message on timeout:<br>> N/A - Not actually a "timeout".  This is a time to display the status on the screen.<br><br>**Constraints**: `>= 1`, `<= 30` | Integer getStatusDisplayTime() | setStatusDisplayTime(Integer statusDisplayTime) |
| `TipCashbackTimeout` | `Integer` | Optional | How long to wait for input on a tip or cashback screen.<br><br>> Message on timeout:<br>> Tip/Cashback Timeout<br><br>**Constraints**: `>= 20`, `<= 50` | Integer getTipCashbackTimeout() | setTipCashbackTimeout(Integer tipCashbackTimeout) |
| `TransactionTimeout` | `Integer` | Optional | How long to wait for response from the processor.<br><br>> Message on timeout:<br>> Transaction Timeout<br><br>**Constraints**: `>= 10`, `<= 20` | Integer getTransactionTimeout() | setTransactionTimeout(Integer transactionTimeout) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "card_entry_timeout": 47,
  "device_terms_prompt_timeout": 30,
  "overall_timeout": 125,
  "pin_entry_timeout": 40,
  "signature_input_timeout": 35,
  "signature_submit_timeout": 38,
  "status_display_time": 12,
  "tip_cashback_timeout": 25,
  "transaction_timeout": 17,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

