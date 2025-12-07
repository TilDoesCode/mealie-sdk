# RecipesFoodsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createOneApiFoodsPost**](#createoneapifoodspost) | **POST** /api/foods | Create One|
|[**deleteOneApiFoodsItemIdDelete**](#deleteoneapifoodsitemiddelete) | **DELETE** /api/foods/{item_id} | Delete One|
|[**getAllApiFoodsGet**](#getallapifoodsget) | **GET** /api/foods | Get All|
|[**getOneApiFoodsItemIdGet**](#getoneapifoodsitemidget) | **GET** /api/foods/{item_id} | Get One|
|[**mergeOneApiFoodsMergePut**](#mergeoneapifoodsmergeput) | **PUT** /api/foods/merge | Merge One|
|[**updateOneApiFoodsItemIdPut**](#updateoneapifoodsitemidput) | **PUT** /api/foods/{item_id} | Update One|

# **createOneApiFoodsPost**
> IngredientFoodOutput createOneApiFoodsPost(createIngredientFood)


### Example

```typescript
import {
    RecipesFoodsApi,
    Configuration,
    CreateIngredientFood
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipesFoodsApi(configuration);

let createIngredientFood: CreateIngredientFood; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createOneApiFoodsPost(
    createIngredientFood,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createIngredientFood** | **CreateIngredientFood**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**IngredientFoodOutput**

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

# **deleteOneApiFoodsItemIdDelete**
> IngredientFoodOutput deleteOneApiFoodsItemIdDelete()


### Example

```typescript
import {
    RecipesFoodsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipesFoodsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteOneApiFoodsItemIdDelete(
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

**IngredientFoodOutput**

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

# **getAllApiFoodsGet**
> IngredientFoodPagination getAllApiFoodsGet()


### Example

```typescript
import {
    RecipesFoodsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipesFoodsApi(configuration);

let search: string; // (optional) (default to undefined)
let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiFoodsGet(
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

**IngredientFoodPagination**

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

# **getOneApiFoodsItemIdGet**
> IngredientFoodOutput getOneApiFoodsItemIdGet()


### Example

```typescript
import {
    RecipesFoodsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipesFoodsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiFoodsItemIdGet(
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

**IngredientFoodOutput**

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

# **mergeOneApiFoodsMergePut**
> SuccessResponse mergeOneApiFoodsMergePut(mergeFood)


### Example

```typescript
import {
    RecipesFoodsApi,
    Configuration,
    MergeFood
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipesFoodsApi(configuration);

let mergeFood: MergeFood; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.mergeOneApiFoodsMergePut(
    mergeFood,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **mergeFood** | **MergeFood**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**SuccessResponse**

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

# **updateOneApiFoodsItemIdPut**
> IngredientFoodOutput updateOneApiFoodsItemIdPut(createIngredientFood)


### Example

```typescript
import {
    RecipesFoodsApi,
    Configuration,
    CreateIngredientFood
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipesFoodsApi(configuration);

let itemId: string; // (default to undefined)
let createIngredientFood: CreateIngredientFood; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateOneApiFoodsItemIdPut(
    itemId,
    createIngredientFood,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createIngredientFood** | **CreateIngredientFood**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**IngredientFoodOutput**

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

