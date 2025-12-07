# GroupInDB


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [default to undefined]
**id** | **string** |  | [default to undefined]
**slug** | **string** |  | [default to undefined]
**categories** | [**Array&lt;CategoryBase&gt;**](CategoryBase.md) |  | [optional] [default to undefined]
**webhooks** | [**Array&lt;ReadWebhook&gt;**](ReadWebhook.md) |  | [optional] [default to undefined]
**households** | [**Array&lt;GroupHouseholdSummary&gt;**](GroupHouseholdSummary.md) |  | [optional] [default to undefined]
**users** | [**Array&lt;UserSummary&gt;**](UserSummary.md) |  | [optional] [default to undefined]
**preferences** | [**ReadGroupPreferences**](ReadGroupPreferences.md) |  | [optional] [default to undefined]

## Example

```typescript
import { GroupInDB } from 'mealie-typescript';

const instance: GroupInDB = {
    name,
    id,
    slug,
    categories,
    webhooks,
    households,
    users,
    preferences,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
