# UserOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**username** | **string** |  | [optional] [default to undefined]
**fullName** | **string** |  | [optional] [default to undefined]
**email** | **string** |  | [default to undefined]
**authMethod** | [**AuthMethod**](AuthMethod.md) |  | [optional] [default to undefined]
**admin** | **boolean** |  | [optional] [default to false]
**group** | **string** |  | [default to undefined]
**household** | **string** |  | [default to undefined]
**advanced** | **boolean** |  | [optional] [default to false]
**canInvite** | **boolean** |  | [optional] [default to false]
**canManage** | **boolean** |  | [optional] [default to false]
**canManageHousehold** | **boolean** |  | [optional] [default to false]
**canOrganize** | **boolean** |  | [optional] [default to false]
**groupId** | **string** |  | [default to undefined]
**groupSlug** | **string** |  | [default to undefined]
**householdId** | **string** |  | [default to undefined]
**householdSlug** | **string** |  | [default to undefined]
**tokens** | [**Array&lt;LongLiveTokenOut&gt;**](LongLiveTokenOut.md) |  | [optional] [default to undefined]
**cacheKey** | **string** |  | [default to undefined]

## Example

```typescript
import { UserOut } from 'mealie-typescript';

const instance: UserOut = {
    id,
    username,
    fullName,
    email,
    authMethod,
    admin,
    group,
    household,
    advanced,
    canInvite,
    canManage,
    canManageHousehold,
    canOrganize,
    groupId,
    groupSlug,
    householdId,
    householdSlug,
    tokens,
    cacheKey,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
