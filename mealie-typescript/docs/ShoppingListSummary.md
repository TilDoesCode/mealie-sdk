# ShoppingListSummary


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [optional] [default to undefined]
**extras** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**createdAt** | **string** |  | [optional] [default to undefined]
**updatedAt** | **string** |  | [optional] [default to undefined]
**groupId** | **string** |  | [default to undefined]
**userId** | **string** |  | [default to undefined]
**id** | **string** |  | [default to undefined]
**householdId** | **string** |  | [default to undefined]
**recipeReferences** | [**Array&lt;ShoppingListRecipeRefOut&gt;**](ShoppingListRecipeRefOut.md) |  | [default to undefined]
**labelSettings** | [**Array&lt;ShoppingListMultiPurposeLabelOut&gt;**](ShoppingListMultiPurposeLabelOut.md) |  | [default to undefined]

## Example

```typescript
import { ShoppingListSummary } from 'mealie-typescript';

const instance: ShoppingListSummary = {
    name,
    extras,
    createdAt,
    updatedAt,
    groupId,
    userId,
    id,
    householdId,
    recipeReferences,
    labelSettings,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
