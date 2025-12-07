# RecipeSuggestionResponseItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**recipe** | [**RecipeSummary**](RecipeSummary.md) |  | [default to undefined]
**missingFoods** | [**Array&lt;IngredientFoodOutput&gt;**](IngredientFoodOutput.md) |  | [default to undefined]
**missingTools** | [**Array&lt;RecipeTool&gt;**](RecipeTool.md) |  | [default to undefined]

## Example

```typescript
import { RecipeSuggestionResponseItem } from 'mealie-typescript';

const instance: RecipeSuggestionResponseItem = {
    recipe,
    missingFoods,
    missingTools,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
