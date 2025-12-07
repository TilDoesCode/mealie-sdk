# UserIn


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] [default to undefined]
**username** | **string** |  | [default to undefined]
**fullName** | **string** |  | [default to undefined]
**email** | **string** |  | [default to undefined]
**authMethod** | [**AuthMethod**](AuthMethod.md) |  | [optional] [default to undefined]
**admin** | **boolean** |  | [optional] [default to false]
**group** | **string** |  | [optional] [default to undefined]
**household** | **string** |  | [optional] [default to undefined]
**advanced** | **boolean** |  | [optional] [default to false]
**canInvite** | **boolean** |  | [optional] [default to false]
**canManage** | **boolean** |  | [optional] [default to false]
**canManageHousehold** | **boolean** |  | [optional] [default to false]
**canOrganize** | **boolean** |  | [optional] [default to false]
**password** | **string** |  | [default to undefined]

## Example

```typescript
import { UserIn } from 'mealie-typescript';

const instance: UserIn = {
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
    password,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
