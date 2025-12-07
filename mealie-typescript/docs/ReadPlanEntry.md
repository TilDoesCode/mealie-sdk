# ReadPlanEntry


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**date** | **string** |  | [default to undefined]
**entryType** | [**PlanEntryType**](PlanEntryType.md) |  | [optional] [default to undefined]
**title** | **string** |  | [optional] [default to '']
**text** | **string** |  | [optional] [default to '']
**recipeId** | **string** |  | [optional] [default to undefined]
**id** | **number** |  | [default to undefined]
**groupId** | **string** |  | [default to undefined]
**userId** | **string** |  | [default to undefined]
**householdId** | **string** |  | [default to undefined]
**recipe** | [**RecipeSummary**](RecipeSummary.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ReadPlanEntry } from 'mealie-typescript';

const instance: ReadPlanEntry = {
    date,
    entryType,
    title,
    text,
    recipeId,
    id,
    groupId,
    userId,
    householdId,
    recipe,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
