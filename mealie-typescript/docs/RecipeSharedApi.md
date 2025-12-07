# RecipeSharedApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getSharedRecipeApiRecipesSharedTokenIdGet**](#getsharedrecipeapirecipessharedtokenidget) | **GET** /api/recipes/shared/{token_id} | Get Shared Recipe|
|[**getSharedRecipeAsZipApiRecipesSharedTokenIdZipGet**](#getsharedrecipeaszipapirecipessharedtokenidzipget) | **GET** /api/recipes/shared/{token_id}/zip | Get Shared Recipe As Zip|

# **getSharedRecipeApiRecipesSharedTokenIdGet**
> RecipeOutput getSharedRecipeApiRecipesSharedTokenIdGet()


### Example

```typescript
import {
    RecipeSharedApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeSharedApi(configuration);

let tokenId: string; // (default to undefined)

const { status, data } = await apiInstance.getSharedRecipeApiRecipesSharedTokenIdGet(
    tokenId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tokenId** | [**string**] |  | defaults to undefined|


### Return type

**RecipeOutput**

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

# **getSharedRecipeAsZipApiRecipesSharedTokenIdZipGet**
> getSharedRecipeAsZipApiRecipesSharedTokenIdZipGet()

Get a recipe and its original image as a Zip file

### Example

```typescript
import {
    RecipeSharedApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeSharedApi(configuration);

let tokenId: string; // (default to undefined)

const { status, data } = await apiInstance.getSharedRecipeAsZipApiRecipesSharedTokenIdZipGet(
    tokenId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tokenId** | [**string**] |  | defaults to undefined|


### Return type

void (empty response body)

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

