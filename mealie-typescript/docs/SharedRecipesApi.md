# SharedRecipesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createOneApiSharedRecipesPost**](#createoneapisharedrecipespost) | **POST** /api/shared/recipes | Create One|
|[**deleteOneApiSharedRecipesItemIdDelete**](#deleteoneapisharedrecipesitemiddelete) | **DELETE** /api/shared/recipes/{item_id} | Delete One|
|[**getAllApiSharedRecipesGet**](#getallapisharedrecipesget) | **GET** /api/shared/recipes | Get All|
|[**getOneApiSharedRecipesItemIdGet**](#getoneapisharedrecipesitemidget) | **GET** /api/shared/recipes/{item_id} | Get One|

# **createOneApiSharedRecipesPost**
> RecipeShareToken createOneApiSharedRecipesPost(recipeShareTokenCreate)


### Example

```typescript
import {
    SharedRecipesApi,
    Configuration,
    RecipeShareTokenCreate
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new SharedRecipesApi(configuration);

let recipeShareTokenCreate: RecipeShareTokenCreate; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createOneApiSharedRecipesPost(
    recipeShareTokenCreate,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **recipeShareTokenCreate** | **RecipeShareTokenCreate**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**RecipeShareToken**

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

# **deleteOneApiSharedRecipesItemIdDelete**
> any deleteOneApiSharedRecipesItemIdDelete()


### Example

```typescript
import {
    SharedRecipesApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new SharedRecipesApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteOneApiSharedRecipesItemIdDelete(
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

**any**

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

# **getAllApiSharedRecipesGet**
> Array<RecipeShareTokenSummary> getAllApiSharedRecipesGet()


### Example

```typescript
import {
    SharedRecipesApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new SharedRecipesApi(configuration);

let recipeId: string; // (optional) (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiSharedRecipesGet(
    recipeId,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **recipeId** | [**string**] |  | (optional) defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Array<RecipeShareTokenSummary>**

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

# **getOneApiSharedRecipesItemIdGet**
> RecipeShareToken getOneApiSharedRecipesItemIdGet()


### Example

```typescript
import {
    SharedRecipesApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new SharedRecipesApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiSharedRecipesItemIdGet(
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

**RecipeShareToken**

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

