# RecipeTimelineApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createOneApiRecipesTimelineEventsPost**](#createoneapirecipestimelineeventspost) | **POST** /api/recipes/timeline/events | Create One|
|[**deleteOneApiRecipesTimelineEventsItemIdDelete**](#deleteoneapirecipestimelineeventsitemiddelete) | **DELETE** /api/recipes/timeline/events/{item_id} | Delete One|
|[**getAllApiRecipesTimelineEventsGet**](#getallapirecipestimelineeventsget) | **GET** /api/recipes/timeline/events | Get All|
|[**getOneApiRecipesTimelineEventsItemIdGet**](#getoneapirecipestimelineeventsitemidget) | **GET** /api/recipes/timeline/events/{item_id} | Get One|
|[**updateEventImageApiRecipesTimelineEventsItemIdImagePut**](#updateeventimageapirecipestimelineeventsitemidimageput) | **PUT** /api/recipes/timeline/events/{item_id}/image | Update Event Image|
|[**updateOneApiRecipesTimelineEventsItemIdPut**](#updateoneapirecipestimelineeventsitemidput) | **PUT** /api/recipes/timeline/events/{item_id} | Update One|

# **createOneApiRecipesTimelineEventsPost**
> RecipeTimelineEventOut createOneApiRecipesTimelineEventsPost(recipeTimelineEventIn)


### Example

```typescript
import {
    RecipeTimelineApi,
    Configuration,
    RecipeTimelineEventIn
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeTimelineApi(configuration);

let recipeTimelineEventIn: RecipeTimelineEventIn; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createOneApiRecipesTimelineEventsPost(
    recipeTimelineEventIn,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **recipeTimelineEventIn** | **RecipeTimelineEventIn**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**RecipeTimelineEventOut**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteOneApiRecipesTimelineEventsItemIdDelete**
> RecipeTimelineEventOut deleteOneApiRecipesTimelineEventsItemIdDelete()


### Example

```typescript
import {
    RecipeTimelineApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeTimelineApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteOneApiRecipesTimelineEventsItemIdDelete(
    itemId,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**RecipeTimelineEventOut**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAllApiRecipesTimelineEventsGet**
> RecipeTimelineEventPagination getAllApiRecipesTimelineEventsGet()


### Example

```typescript
import {
    RecipeTimelineApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeTimelineApi(configuration);

let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiRecipesTimelineEventsGet(
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
| **orderBy** | [**string**] |  | (optional) defaults to undefined|
| **orderByNullPosition** | **OrderByNullPosition** |  | (optional) defaults to undefined|
| **orderDirection** | **OrderDirection** |  | (optional) defaults to undefined|
| **queryFilter** | [**string**] |  | (optional) defaults to undefined|
| **paginationSeed** | [**string**] |  | (optional) defaults to undefined|
| **page** | [**number**] |  | (optional) defaults to 1|
| **perPage** | [**number**] |  | (optional) defaults to 50|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**RecipeTimelineEventPagination**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getOneApiRecipesTimelineEventsItemIdGet**
> RecipeTimelineEventOut getOneApiRecipesTimelineEventsItemIdGet()


### Example

```typescript
import {
    RecipeTimelineApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeTimelineApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiRecipesTimelineEventsItemIdGet(
    itemId,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**RecipeTimelineEventOut**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateEventImageApiRecipesTimelineEventsItemIdImagePut**
> UpdateImageResponse updateEventImageApiRecipesTimelineEventsItemIdImagePut()


### Example

```typescript
import {
    RecipeTimelineApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeTimelineApi(configuration);

let itemId: string; // (default to undefined)
let image: File; // (default to undefined)
let extension: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateEventImageApiRecipesTimelineEventsItemIdImagePut(
    itemId,
    image,
    extension,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **itemId** | [**string**] |  | defaults to undefined|
| **image** | [**File**] |  | defaults to undefined|
| **extension** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**UpdateImageResponse**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateOneApiRecipesTimelineEventsItemIdPut**
> RecipeTimelineEventOut updateOneApiRecipesTimelineEventsItemIdPut(recipeTimelineEventUpdate)


### Example

```typescript
import {
    RecipeTimelineApi,
    Configuration,
    RecipeTimelineEventUpdate
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeTimelineApi(configuration);

let itemId: string; // (default to undefined)
let recipeTimelineEventUpdate: RecipeTimelineEventUpdate; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateOneApiRecipesTimelineEventsItemIdPut(
    itemId,
    recipeTimelineEventUpdate,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **recipeTimelineEventUpdate** | **RecipeTimelineEventUpdate**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**RecipeTimelineEventOut**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

