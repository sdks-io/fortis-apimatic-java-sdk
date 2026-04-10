
# Surcharge Transaction

Surcharge Transaction Information on `expand`

*This model accepts additional fields of type Object.*

## Structure

`SurchargeTransaction`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `String` | Optional | ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getId() | setId(String id) |
| `ModelName` | `String` | Optional | Model Name | String getModelName() | setModelName(String modelName) |
| `TransactionId` | `String` | Optional | Transaction ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getTransactionId() | setTransactionId(String transactionId) |
| `SurchargeFee` | `Integer` | Optional | Surcharge Fee<br><br>**Constraints**: `>= 0` | Integer getSurchargeFee() | setSurchargeFee(Integer surchargeFee) |
| `SurchargeRate` | `Integer` | Optional | Surcharge Rate<br><br>**Constraints**: `>= 0` | Integer getSurchargeRate() | setSurchargeRate(Integer surchargeRate) |
| `SurchargeAmount` | `Integer` | Optional | Surcharge Amount<br><br>**Constraints**: `>= 0` | Integer getSurchargeAmount() | setSurchargeAmount(Integer surchargeAmount) |
| `SurchargeTransactionMin` | `Integer` | Optional | Surcharge Transaction Minimum<br><br>**Constraints**: `>= 0` | Integer getSurchargeTransactionMin() | setSurchargeTransactionMin(Integer surchargeTransactionMin) |
| `SurchargeTransactionMax` | `Integer` | Optional | Surcharge Transaction Maximum<br><br>**Constraints**: `>= 0` | Integer getSurchargeTransactionMax() | setSurchargeTransactionMax(Integer surchargeTransactionMax) |
| `Created` | `Integer` | Optional | Created | Integer getCreated() | setCreated(Integer created) |
| `Modified` | `Integer` | Optional | Modified | Integer getModified() | setModified(Integer modified) |
| `CreatedUserId` | `String` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getCreatedUserId() | setCreatedUserId(String createdUserId) |
| `ModifiedUserId` | `String` | Optional | Last User ID that updated the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | String getModifiedUserId() | setModifiedUserId(String modifiedUserId) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "model_name": "Model Name",
  "transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "surcharge_fee": 0,
  "surcharge_rate": 0,
  "created": 1422040992,
  "modified": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "modified_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

