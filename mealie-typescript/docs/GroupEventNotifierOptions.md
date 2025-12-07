# GroupEventNotifierOptions

These events are in-sync with the EventTypes found in the EventBusService. If you modify this, make sure to update the EventBusService as well.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**testMessage** | **boolean** |  | [optional] [default to false]
**webhookTask** | **boolean** |  | [optional] [default to false]
**recipeCreated** | **boolean** |  | [optional] [default to false]
**recipeUpdated** | **boolean** |  | [optional] [default to false]
**recipeDeleted** | **boolean** |  | [optional] [default to false]
**userSignup** | **boolean** |  | [optional] [default to false]
**dataMigrations** | **boolean** |  | [optional] [default to false]
**dataExport** | **boolean** |  | [optional] [default to false]
**dataImport** | **boolean** |  | [optional] [default to false]
**mealplanEntryCreated** | **boolean** |  | [optional] [default to false]
**shoppingListCreated** | **boolean** |  | [optional] [default to false]
**shoppingListUpdated** | **boolean** |  | [optional] [default to false]
**shoppingListDeleted** | **boolean** |  | [optional] [default to false]
**cookbookCreated** | **boolean** |  | [optional] [default to false]
**cookbookUpdated** | **boolean** |  | [optional] [default to false]
**cookbookDeleted** | **boolean** |  | [optional] [default to false]
**tagCreated** | **boolean** |  | [optional] [default to false]
**tagUpdated** | **boolean** |  | [optional] [default to false]
**tagDeleted** | **boolean** |  | [optional] [default to false]
**categoryCreated** | **boolean** |  | [optional] [default to false]
**categoryUpdated** | **boolean** |  | [optional] [default to false]
**categoryDeleted** | **boolean** |  | [optional] [default to false]
**labelCreated** | **boolean** |  | [optional] [default to false]
**labelUpdated** | **boolean** |  | [optional] [default to false]
**labelDeleted** | **boolean** |  | [optional] [default to false]

## Example

```typescript
import { GroupEventNotifierOptions } from 'mealie-typescript';

const instance: GroupEventNotifierOptions = {
    testMessage,
    webhookTask,
    recipeCreated,
    recipeUpdated,
    recipeDeleted,
    userSignup,
    dataMigrations,
    dataExport,
    dataImport,
    mealplanEntryCreated,
    shoppingListCreated,
    shoppingListUpdated,
    shoppingListDeleted,
    cookbookCreated,
    cookbookUpdated,
    cookbookDeleted,
    tagCreated,
    tagUpdated,
    tagDeleted,
    categoryCreated,
    categoryUpdated,
    categoryDeleted,
    labelCreated,
    labelUpdated,
    labelDeleted,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
