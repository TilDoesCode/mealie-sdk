# Food


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**pluralName** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to '']
**extras** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**labelId** | **string** |  | [optional] [default to undefined]
**aliases** | [**Array&lt;CreateIngredientFoodAlias&gt;**](CreateIngredientFoodAlias.md) |  | [optional] [default to undefined]
**householdsWithIngredientFood** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**label** | [**MultiPurposeLabelSummary**](MultiPurposeLabelSummary.md) |  | [optional] [default to undefined]
**createdAt** | **string** |  | [optional] [default to undefined]
**update_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { Food } from 'mealie-typescript';

const instance: Food = {
    id,
    name,
    pluralName,
    description,
    extras,
    labelId,
    aliases,
    householdsWithIngredientFood,
    label,
    createdAt,
    update_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
