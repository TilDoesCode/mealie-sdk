# RecipesUnitsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createOneApiUnitsPost**](#createoneapiunitspost) | **POST** /api/units | Create One|
|[**deleteOneApiUnitsItemIdDelete**](#deleteoneapiunitsitemiddelete) | **DELETE** /api/units/{item_id} | Delete One|
|[**getAllApiUnitsGet**](#getallapiunitsget) | **GET** /api/units | Get All|
|[**getOneApiUnitsItemIdGet**](#getoneapiunitsitemidget) | **GET** /api/units/{item_id} | Get One|
|[**mergeOneApiUnitsMergePut**](#mergeoneapiunitsmergeput) | **PUT** /api/units/merge | Merge One|
|[**updateOneApiUnitsItemIdPut**](#updateoneapiunitsitemidput) | **PUT** /api/units/{item_id} | Update One|

# **createOneApiUnitsPost**
> IngredientUnitOutput createOneApiUnitsPost(createIngredientUnit)


### Example

```typescript
import {
    RecipesUnitsApi,
    Configuration,
    CreateIngredientUnit
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipesUnitsApi(configuration);

let createIngredientUnit: CreateIngredientUnit; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createOneApiUnitsPost(
    createIngredientUnit,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createIngredientUnit** | **CreateIngredientUnit**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**IngredientUnitOutput**

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

# **deleteOneApiUnitsItemIdDelete**
> IngredientUnitOutput deleteOneApiUnitsItemIdDelete()


### Example

```typescript
import {
    RecipesUnitsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipesUnitsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteOneApiUnitsItemIdDelete(
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

**IngredientUnitOutput**

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

# **getAllApiUnitsGet**
> IngredientUnitPagination getAllApiUnitsGet()


### Example

```typescript
import {
    RecipesUnitsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipesUnitsApi(configuration);

let search: string; // (optional) (default to undefined)
let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiUnitsGet(
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

**IngredientUnitPagination**

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

# **getOneApiUnitsItemIdGet**
> IngredientUnitOutput getOneApiUnitsItemIdGet()


### Example

```typescript
import {
    RecipesUnitsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipesUnitsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiUnitsItemIdGet(
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

**IngredientUnitOutput**

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

# **mergeOneApiUnitsMergePut**
> SuccessResponse mergeOneApiUnitsMergePut(mergeUnit)


### Example

```typescript
import {
    RecipesUnitsApi,
    Configuration,
    MergeUnit
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipesUnitsApi(configuration);

let mergeUnit: MergeUnit; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.mergeOneApiUnitsMergePut(
    mergeUnit,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **mergeUnit** | **MergeUnit**|  | |
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

# **updateOneApiUnitsItemIdPut**
> IngredientUnitOutput updateOneApiUnitsItemIdPut(createIngredientUnit)


### Example

```typescript
import {
    RecipesUnitsApi,
    Configuration,
    CreateIngredientUnit
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipesUnitsApi(configuration);

let itemId: string; // (default to undefined)
let createIngredientUnit: CreateIngredientUnit; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateOneApiUnitsItemIdPut(
    itemId,
    createIngredientUnit,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createIngredientUnit** | **CreateIngredientUnit**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**IngredientUnitOutput**

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

