# ReadCookBook


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [default to undefined]
**description** | **string** |  | [optional] [default to '']
**slug** | **string** |  | [optional] [default to undefined]
**position** | **number** |  | [optional] [default to 1]
**_public** | **boolean** |  | [optional] [default to false]
**queryFilterString** | **string** |  | [optional] [default to '']
**groupId** | **string** |  | [default to undefined]
**householdId** | **string** |  | [default to undefined]
**id** | **string** |  | [default to undefined]
**queryFilter** | [**QueryFilterJSON**](QueryFilterJSON.md) |  | [optional] [default to undefined]
**household** | [**CookbookHousehold**](CookbookHousehold.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ReadCookBook } from 'mealie-typescript';

const instance: ReadCookBook = {
    name,
    description,
    slug,
    position,
    _public,
    queryFilterString,
    groupId,
    householdId,
    id,
    queryFilter,
    household,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
