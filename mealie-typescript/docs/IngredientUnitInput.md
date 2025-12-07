# IngredientUnitInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**pluralName** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to '']
**extras** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**fraction** | **boolean** |  | [optional] [default to true]
**abbreviation** | **string** |  | [optional] [default to '']
**pluralAbbreviation** | **string** |  | [optional] [default to undefined]
**useAbbreviation** | **boolean** |  | [optional] [default to false]
**aliases** | [**Array&lt;IngredientUnitAlias&gt;**](IngredientUnitAlias.md) |  | [optional] [default to undefined]
**createdAt** | **string** |  | [optional] [default to undefined]
**update_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { IngredientUnitInput } from 'mealie-typescript';

const instance: IngredientUnitInput = {
    id,
    name,
    pluralName,
    description,
    extras,
    fraction,
    abbreviation,
    pluralAbbreviation,
    useAbbreviation,
    aliases,
    createdAt,
    update_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
