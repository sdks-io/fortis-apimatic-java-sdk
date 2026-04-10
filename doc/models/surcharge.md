
# Surcharge

Surcharge Information on `expand`

*This model accepts additional fields of type Object.*

## Structure

`Surcharge`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `SurchargeFee` | `Integer` | Optional | Surcharge Fee | Integer getSurchargeFee() | setSurchargeFee(Integer surchargeFee) |
| `SurchargeRate` | `Integer` | Optional | Surcharge Rate | Integer getSurchargeRate() | setSurchargeRate(Integer surchargeRate) |
| `MaxTransactionAmount` | `Integer` | Optional | Max Transaction Amount | Integer getMaxTransactionAmount() | setMaxTransactionAmount(Integer maxTransactionAmount) |
| `MinFeeAmount` | `Integer` | Optional | Min Fee Amount | Integer getMinFeeAmount() | setMinFeeAmount(Integer minFeeAmount) |
| `MaxFeeAmount` | `Integer` | Optional | Max Fee Amount | Integer getMaxFeeAmount() | setMaxFeeAmount(Integer maxFeeAmount) |
| `SurchargeOnRecurring` | `Boolean` | Optional | Surcharge On Recurring | Boolean getSurchargeOnRecurring() | setSurchargeOnRecurring(Boolean surchargeOnRecurring) |
| `RefundSurcharges` | `Boolean` | Optional | Refund Surcharges | Boolean getRefundSurcharges() | setRefundSurcharges(Boolean refundSurcharges) |
| `BlindRefundSurcharges` | `Boolean` | Optional | Blind Refund Surcharges | Boolean getBlindRefundSurcharges() | setBlindRefundSurcharges(Boolean blindRefundSurcharges) |
| `ProductTransactionId` | `String` | Optional | Product Transaction Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getProductTransactionId() | setProductTransactionId(String productTransactionId) |
| `RunAsSeparateTransaction` | `Boolean` | Optional | Run As Separate Transaction | Boolean getRunAsSeparateTransaction() | setRunAsSeparateTransaction(Boolean runAsSeparateTransaction) |
| `ApplyToUserTypeId` | `String` | Optional | Apply To User Type Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getApplyToUserTypeId() | setApplyToUserTypeId(String applyToUserTypeId) |
| `Title` | `String` | Optional | Title<br><br>**Constraints**: *Maximum Length*: `256` | String getTitle() | setTitle(String title) |
| `SurchargeLabel` | `String` | Optional | Surcharge Label<br><br>**Constraints**: *Maximum Length*: `64` | String getSurchargeLabel() | setSurchargeLabel(String surchargeLabel) |
| `SurchargeTransactionProductId` | `String` | Optional | Surcharge Transaction Product Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getSurchargeTransactionProductId() | setSurchargeTransactionProductId(String surchargeTransactionProductId) |
| `StateExceptionCheck` | `Boolean` | Optional | State Exception Check | Boolean getStateExceptionCheck() | setStateExceptionCheck(Boolean stateExceptionCheck) |
| `Compliant` | `Boolean` | Optional | Compliant | Boolean getCompliant() | setCompliant(Boolean compliant) |
| `Id` | `String` | Optional | Surcharge Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `ModifiedUserId` | `String` | Optional | Last User ID that updated the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getModifiedUserId() | setModifiedUserId(String modifiedUserId) |
| `CreatedTs` | `Integer` | Optional | Created Time Stamp | Integer getCreatedTs() | setCreatedTs(Integer createdTs) |
| `ModifiedTs` | `Integer` | Optional | Modified Time Stamp | Integer getModifiedTs() | setModifiedTs(Integer modifiedTs) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "surcharge_fee": 10,
  "surcharge_rate": 1,
  "product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "apply_to_user_type_id": "11e95f8ec39de8fbdb0a4f1a",
  "surcharge_transaction_product_id": "11e95f8ec39de8fbdb0a4f1a",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "modified_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "max_transaction_amount": 252,
  "min_fee_amount": 198,
  "max_fee_amount": 172,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

