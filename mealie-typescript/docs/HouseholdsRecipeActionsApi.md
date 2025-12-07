# HouseholdsRecipeActionsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createOneApiHouseholdsRecipeActionsPost**](#createoneapihouseholdsrecipeactionspost) | **POST** /api/households/recipe-actions | Create One|
|[**deleteOneApiHouseholdsRecipeActionsItemIdDelete**](#deleteoneapihouseholdsrecipeactionsitemiddelete) | **DELETE** /api/households/recipe-actions/{item_id} | Delete One|
|[**getAllApiHouseholdsRecipeActionsGet**](#getallapihouseholdsrecipeactionsget) | **GET** /api/households/recipe-actions | Get All|
|[**getOneApiHouseholdsRecipeActionsItemIdGet**](#getoneapihouseholdsrecipeactionsitemidget) | **GET** /api/households/recipe-actions/{item_id} | Get One|
|[**triggerActionApiHouseholdsRecipeActionsItemIdTriggerRecipeSlugPost**](#triggeractionapihouseholdsrecipeactionsitemidtriggerrecipeslugpost) | **POST** /api/households/recipe-actions/{item_id}/trigger/{recipe_slug} | Trigger Action|
|[**updateOneApiHouseholdsRecipeActionsItemIdPut**](#updateoneapihouseholdsrecipeactionsitemidput) | **PUT** /api/households/recipe-actions/{item_id} | Update One|

# **createOneApiHouseholdsRecipeActionsPost**
> GroupRecipeActionOut createOneApiHouseholdsRecipeActionsPost(createGroupRecipeAction)


### Example

```typescript
import {
    HouseholdsRecipeActionsApi,
    Configuration,
    CreateGroupRecipeAction
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsRecipeActionsApi(configuration);

let createGroupRecipeAction: CreateGroupRecipeAction; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createOneApiHouseholdsRecipeActionsPost(
    createGroupRecipeAction,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createGroupRecipeAction** | **CreateGroupRecipeAction**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**GroupRecipeActionOut**

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

# **deleteOneApiHouseholdsRecipeActionsItemIdDelete**
> GroupRecipeActionOut deleteOneApiHouseholdsRecipeActionsItemIdDelete()


### Example

```typescript
import {
    HouseholdsRecipeActionsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsRecipeActionsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteOneApiHouseholdsRecipeActionsItemIdDelete(
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

**GroupRecipeActionOut**

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

# **getAllApiHouseholdsRecipeActionsGet**
> GroupRecipeActionPagination getAllApiHouseholdsRecipeActionsGet()


### Example

```typescript
import {
    HouseholdsRecipeActionsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsRecipeActionsApi(configuration);

let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiHouseholdsRecipeActionsGet(
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

**GroupRecipeActionPagination**

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

# **getOneApiHouseholdsRecipeActionsItemIdGet**
> GroupRecipeActionOut getOneApiHouseholdsRecipeActionsItemIdGet()


### Example

```typescript
import {
    HouseholdsRecipeActionsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsRecipeActionsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiHouseholdsRecipeActionsItemIdGet(
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

**GroupRecipeActionOut**

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

# **triggerActionApiHouseholdsRecipeActionsItemIdTriggerRecipeSlugPost**
> any triggerActionApiHouseholdsRecipeActionsItemIdTriggerRecipeSlugPost()


### Example

```typescript
import {
    HouseholdsRecipeActionsApi,
    Configuration,
    BodyTriggerActionApiHouseholdsRecipeActionsItemIdTriggerRecipeSlugPost
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsRecipeActionsApi(configuration);

let itemId: string; // (default to undefined)
let recipeSlug: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)
let bodyTriggerActionApiHouseholdsRecipeActionsItemIdTriggerRecipeSlugPost: BodyTriggerActionApiHouseholdsRecipeActionsItemIdTriggerRecipeSlugPost; // (optional)

const { status, data } = await apiInstance.triggerActionApiHouseholdsRecipeActionsItemIdTriggerRecipeSlugPost(
    itemId,
    recipeSlug,
    acceptLanguage,
    bodyTriggerActionApiHouseholdsRecipeActionsItemIdTriggerRecipeSlugPost
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bodyTriggerActionApiHouseholdsRecipeActionsItemIdTriggerRecipeSlugPost** | **BodyTriggerActionApiHouseholdsRecipeActionsItemIdTriggerRecipeSlugPost**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **recipeSlug** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**any**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**202** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateOneApiHouseholdsRecipeActionsItemIdPut**
> GroupRecipeActionOut updateOneApiHouseholdsRecipeActionsItemIdPut(saveGroupRecipeAction)


### Example

```typescript
import {
    HouseholdsRecipeActionsApi,
    Configuration,
    SaveGroupRecipeAction
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsRecipeActionsApi(configuration);

let itemId: string; // (default to undefined)
let saveGroupRecipeAction: SaveGroupRecipeAction; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateOneApiHouseholdsRecipeActionsItemIdPut(
    itemId,
    saveGroupRecipeAction,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **saveGroupRecipeAction** | **SaveGroupRecipeAction**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**GroupRecipeActionOut**

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

