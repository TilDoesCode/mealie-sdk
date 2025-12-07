# ShoppingListItemUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**quantity** | **number** |  | [optional] [default to 1]
**unit** | [**Unit**](Unit.md) |  | [optional] [default to undefined]
**food** | [**Food**](Food.md) |  | [optional] [default to undefined]
**referencedRecipe** | [**RecipeInput**](RecipeInput.md) |  | [optional] [default to undefined]
**note** | **string** |  | [optional] [default to undefined]
**display** | **string** |  | [optional] [default to '']
**shoppingListId** | **string** |  | [default to undefined]
**checked** | **boolean** |  | [optional] [default to false]
**position** | **number** |  | [optional] [default to 0]
**foodId** | **string** |  | [optional] [default to undefined]
**labelId** | **string** |  | [optional] [default to undefined]
**unitId** | **string** |  | [optional] [default to undefined]
**extras** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**recipeReferences** | [**Array&lt;ShoppingListItemUpdateRecipeReferencesInner&gt;**](ShoppingListItemUpdateRecipeReferencesInner.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ShoppingListItemUpdate } from 'mealie-typescript';

const instance: ShoppingListItemUpdate = {
    quantity,
    unit,
    food,
    referencedRecipe,
    note,
    display,
    shoppingListId,
    checked,
    position,
    foodId,
    labelId,
    unitId,
    extras,
    recipeReferences,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
