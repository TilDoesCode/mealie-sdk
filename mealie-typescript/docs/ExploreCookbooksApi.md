# ExploreCookbooksApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getAllApiExploreGroupsGroupSlugCookbooksGet**](#getallapiexploregroupsgroupslugcookbooksget) | **GET** /api/explore/groups/{group_slug}/cookbooks | Get All|
|[**getOneApiExploreGroupsGroupSlugCookbooksItemIdGet**](#getoneapiexploregroupsgroupslugcookbooksitemidget) | **GET** /api/explore/groups/{group_slug}/cookbooks/{item_id} | Get One|

# **getAllApiExploreGroupsGroupSlugCookbooksGet**
> PaginationBaseReadCookBook getAllApiExploreGroupsGroupSlugCookbooksGet()


### Example

```typescript
import {
    ExploreCookbooksApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new ExploreCookbooksApi(configuration);

let groupSlug: string; // (default to undefined)
let search: string; // (optional) (default to undefined)
let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiExploreGroupsGroupSlugCookbooksGet(
    groupSlug,
    search,
    orderBy,
    orderByNullPosition,
    orderDirection,
    queryFilter,
    paginationSeed,
    page,
    perPage,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **groupSlug** | [**string**] |  | defaults to undefined|
| **search** | [**string**] |  | (optional) defaults to undefined|
| **orderBy** | [**string**] |  | (optional) defaults to undefined|
| **orderByNullPosition** | **OrderByNullPosition** |  | (optional) defaults to undefined|
| **orderDirection** | **OrderDirection** |  | (optional) defaults to undefined|
| **queryFilter** | [**string**] |  | (optional) defaults to undefined|
| **paginationSeed** | [**string**] |  | (optional) defaults to undefined|
| **page** | [**number**] |  | (optional) defaults to 1|
| **perPage** | [**number**] |  | (optional) defaults to 50|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**PaginationBaseReadCookBook**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getOneApiExploreGroupsGroupSlugCookbooksItemIdGet**
> ReadCookBook getOneApiExploreGroupsGroupSlugCookbooksItemIdGet()


### Example

```typescript
import {
    ExploreCookbooksApi,
    Configuration,
    ItemId1
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new ExploreCookbooksApi(configuration);

let itemId: ItemId1; // (default to undefined)
let groupSlug: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiExploreGroupsGroupSlugCookbooksItemIdGet(
    itemId,
    groupSlug,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **itemId** | **ItemId1** |  | defaults to undefined|
| **groupSlug** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ReadCookBook**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

