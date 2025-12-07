# ShoppingListOut


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
**listItems** | [**Array&lt;ShoppingListItemOutOutput&gt;**](ShoppingListItemOutOutput.md) |  | [optional] [default to undefined]
**householdId** | **string** |  | [default to undefined]
**recipeReferences** | [**Array&lt;ShoppingListRecipeRefOut&gt;**](ShoppingListRecipeRefOut.md) |  | [optional] [default to undefined]
**labelSettings** | [**Array&lt;ShoppingListMultiPurposeLabelOut&gt;**](ShoppingListMultiPurposeLabelOut.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ShoppingListOut } from 'mealie-typescript';

const instance: ShoppingListOut = {
    name,
    extras,
    createdAt,
    updatedAt,
    groupId,
    userId,
    id,
    listItems,
    householdId,
    recipeReferences,
    labelSettings,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
