# ShoppingListUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [optional] [default to undefined]
**extras** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**createdAt** | **string** |  | [optional] [default to undefined]
**update_at** | **string** |  | [optional] [default to undefined]
**groupId** | **string** |  | [default to undefined]
**userId** | **string** |  | [default to undefined]
**id** | **string** |  | [default to undefined]
**listItems** | [**Array&lt;ShoppingListItemOutInput&gt;**](ShoppingListItemOutInput.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ShoppingListUpdate } from 'mealie-typescript';

const instance: ShoppingListUpdate = {
    name,
    extras,
    createdAt,
    update_at,
    groupId,
    userId,
    id,
    listItems,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
