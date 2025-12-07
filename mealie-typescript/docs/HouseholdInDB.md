# HouseholdInDB


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**groupId** | **string** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**id** | **string** |  | [default to undefined]
**slug** | **string** |  | [default to undefined]
**preferences** | [**ReadHouseholdPreferences**](ReadHouseholdPreferences.md) |  | [optional] [default to undefined]
**group** | **string** |  | [default to undefined]
**users** | [**Array&lt;HouseholdUserSummary&gt;**](HouseholdUserSummary.md) |  | [optional] [default to undefined]
**webhooks** | [**Array&lt;ReadWebhook&gt;**](ReadWebhook.md) |  | [optional] [default to undefined]

## Example

```typescript
import { HouseholdInDB } from 'mealie-typescript';

const instance: HouseholdInDB = {
    groupId,
    name,
    id,
    slug,
    preferences,
    group,
    users,
    webhooks,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
