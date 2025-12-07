# PaginationBaseReadCookBook


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **number** |  | [optional] [default to 1]
**per_page** | **number** |  | [optional] [default to 10]
**total** | **number** |  | [optional] [default to 0]
**total_pages** | **number** |  | [optional] [default to 0]
**items** | [**Array&lt;ReadCookBook&gt;**](ReadCookBook.md) |  | [default to undefined]
**next** | **string** |  | [optional] [default to undefined]
**previous** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { PaginationBaseReadCookBook } from 'mealie-typescript';

const instance: PaginationBaseReadCookBook = {
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
