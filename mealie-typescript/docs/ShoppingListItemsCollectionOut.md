# ShoppingListItemsCollectionOut

Container for bulk shopping list item changes

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**createdItems** | [**Array&lt;ShoppingListItemOutOutput&gt;**](ShoppingListItemOutOutput.md) |  | [optional] [default to undefined]
**updatedItems** | [**Array&lt;ShoppingListItemOutOutput&gt;**](ShoppingListItemOutOutput.md) |  | [optional] [default to undefined]
**deletedItems** | [**Array&lt;ShoppingListItemOutOutput&gt;**](ShoppingListItemOutOutput.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ShoppingListItemsCollectionOut } from 'mealie-typescript';

const instance: ShoppingListItemsCollectionOut = {
    createdItems,
    updatedItems,
    deletedItems,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
