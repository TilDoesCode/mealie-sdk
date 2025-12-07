# RecipeInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] [default to undefined]
**userId** | **string** |  | [optional] [default to undefined]
**householdId** | **string** |  | [optional] [default to undefined]
**groupId** | **string** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**slug** | **string** |  | [optional] [default to '']
**image** | [****](.md) |  | [optional] [default to undefined]
**recipeServings** | **number** |  | [optional] [default to 0]
**recipeYieldQuantity** | **number** |  | [optional] [default to 0]
**recipeYield** | **string** |  | [optional] [default to undefined]
**totalTime** | **string** |  | [optional] [default to undefined]
**prepTime** | **string** |  | [optional] [default to undefined]
**cookTime** | **string** |  | [optional] [default to undefined]
**performTime** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**recipeCategory** | [**Array&lt;RecipeCategory&gt;**](RecipeCategory.md) |  | [optional] [default to undefined]
**tags** | [**Array&lt;RecipeTag&gt;**](RecipeTag.md) |  | [optional] [default to undefined]
**tools** | [**Array&lt;RecipeTool&gt;**](RecipeTool.md) |  | [optional] [default to undefined]
**rating** | **number** |  | [optional] [default to undefined]
**orgURL** | **string** |  | [optional] [default to undefined]
**dateAdded** | **string** |  | [optional] [default to undefined]
**dateUpdated** | **string** |  | [optional] [default to undefined]
**createdAt** | **string** |  | [optional] [default to undefined]
**update_at** | **string** |  | [optional] [default to undefined]
**lastMade** | **string** |  | [optional] [default to undefined]
**recipeIngredient** | [**Array&lt;RecipeIngredientInput&gt;**](RecipeIngredientInput.md) |  | [optional] [default to undefined]
**recipeInstructions** | [**Array&lt;RecipeStep&gt;**](RecipeStep.md) |  | [optional] [default to undefined]
**nutrition** | [**Nutrition**](Nutrition.md) |  | [optional] [default to undefined]
**settings** | [**RecipeSettings**](RecipeSettings.md) |  | [optional] [default to undefined]
**assets** | [**Array&lt;RecipeAsset&gt;**](RecipeAsset.md) |  | [optional] [default to undefined]
**notes** | [**Array&lt;RecipeNote&gt;**](RecipeNote.md) |  | [optional] [default to undefined]
**extras** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**comments** | [**Array&lt;RecipeCommentOutInput&gt;**](RecipeCommentOutInput.md) |  | [optional] [default to undefined]

## Example

```typescript
import { RecipeInput } from 'mealie-typescript';

const instance: RecipeInput = {
    id,
    userId,
    householdId,
    groupId,
    name,
    slug,
    image,
    recipeServings,
    recipeYieldQuantity,
    recipeYield,
    totalTime,
    prepTime,
    cookTime,
    performTime,
    description,
    recipeCategory,
    tags,
    tools,
    rating,
    orgURL,
    dateAdded,
    dateUpdated,
    createdAt,
    update_at,
    lastMade,
    recipeIngredient,
    recipeInstructions,
    nutrition,
    settings,
    assets,
    notes,
    extras,
    comments,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
