# ShoppingListItemOutOutput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**quantity** | **number** |  | [optional] [default to 1]
**unit** | [**IngredientUnitOutput**](IngredientUnitOutput.md) |  | [optional] [default to undefined]
**food** | [**IngredientFoodOutput**](IngredientFoodOutput.md) |  | [optional] [default to undefined]
**referencedRecipe** | [**RecipeOutput**](RecipeOutput.md) |  | [optional] [default to undefined]
**note** | **string** |  | [optional] [default to undefined]
**display** | **string** |  | [optional] [default to '']
**shoppingListId** | **string** |  | [default to undefined]
**checked** | **boolean** |  | [optional] [default to false]
**position** | **number** |  | [optional] [default to 0]
**foodId** | **string** |  | [optional] [default to undefined]
**labelId** | **string** |  | [optional] [default to undefined]
**unitId** | **string** |  | [optional] [default to undefined]
**extras** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**id** | **string** |  | [default to undefined]
**groupId** | **string** |  | [default to undefined]
**householdId** | **string** |  | [default to undefined]
**label** | [**MultiPurposeLabelSummary**](MultiPurposeLabelSummary.md) |  | [optional] [default to undefined]
**recipeReferences** | [**Array&lt;ShoppingListItemRecipeRefOut&gt;**](ShoppingListItemRecipeRefOut.md) |  | [optional] [default to undefined]
**createdAt** | **string** |  | [optional] [default to undefined]
**updatedAt** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { ShoppingListItemOutOutput } from 'mealie-typescript';

const instance: ShoppingListItemOutOutput = {
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
    id,
    groupId,
    householdId,
    label,
    recipeReferences,
    createdAt,
    updatedAt,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
