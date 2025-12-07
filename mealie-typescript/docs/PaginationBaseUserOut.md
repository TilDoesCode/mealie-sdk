# PaginationBaseUserOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **number** |  | [optional] [default to 1]
**per_page** | **number** |  | [optional] [default to 10]
**total** | **number** |  | [optional] [default to 0]
**total_pages** | **number** |  | [optional] [default to 0]
**items** | [**Array&lt;UserOut&gt;**](UserOut.md) |  | [default to undefined]
**next** | **string** |  | [optional] [default to undefined]
**previous** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { PaginationBaseUserOut } from 'mealie-typescript';

const instance: PaginationBaseUserOut = {
    page,
    per_page,
    total,
    total_pages,
    items,
    next,
    previous,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
