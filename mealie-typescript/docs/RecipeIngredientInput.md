# RecipeIngredientInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**quantity** | **number** |  | [optional] [default to undefined]
**unit** | [**Unit**](Unit.md) |  | [optional] [default to undefined]
**food** | [**Food**](Food.md) |  | [optional] [default to undefined]
**referencedRecipe** | [**RecipeInput**](RecipeInput.md) |  | [optional] [default to undefined]
**note** | **string** |  | [optional] [default to undefined]
**display** | **string** |  | [optional] [default to '']
**title** | **string** |  | [optional] [default to undefined]
**originalText** | **string** |  | [optional] [default to undefined]
**referenceId** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { RecipeIngredientInput } from 'mealie-typescript';

const instance: RecipeIngredientInput = {
    quantity,
    unit,
    food,
    referencedRecipe,
    note,
    display,
    title,
    originalText,
    referenceId,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
