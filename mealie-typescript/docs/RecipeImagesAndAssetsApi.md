# RecipeImagesAndAssetsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**deleteRecipeImageApiRecipesSlugImageDelete**](#deleterecipeimageapirecipesslugimagedelete) | **DELETE** /api/recipes/{slug}/image | Delete Recipe Image|
|[**getRecipeAssetApiMediaRecipesRecipeIdAssetsFileNameGet**](#getrecipeassetapimediarecipesrecipeidassetsfilenameget) | **GET** /api/media/recipes/{recipe_id}/assets/{file_name} | Get Recipe Asset|
|[**getRecipeImgApiMediaRecipesRecipeIdImagesFileNameGet**](#getrecipeimgapimediarecipesrecipeidimagesfilenameget) | **GET** /api/media/recipes/{recipe_id}/images/{file_name} | Get Recipe Img|
|[**getRecipeTimelineEventImgApiMediaRecipesRecipeIdImagesTimelineTimelineEventIdFileNameGet**](#getrecipetimelineeventimgapimediarecipesrecipeidimagestimelinetimelineeventidfilenameget) | **GET** /api/media/recipes/{recipe_id}/images/timeline/{timeline_event_id}/{file_name} | Get Recipe Timeline Event Img|
|[**getUserImageApiMediaUsersUserIdFileNameGet**](#getuserimageapimediausersuseridfilenameget) | **GET** /api/media/users/{user_id}/{file_name} | Get User Image|
|[**getValidationTextApiMediaDockerValidateTxtGet**](#getvalidationtextapimediadockervalidatetxtget) | **GET** /api/media/docker/validate.txt | Get Validation Text|
|[**scrapeImageUrlApiRecipesSlugImagePost**](#scrapeimageurlapirecipesslugimagepost) | **POST** /api/recipes/{slug}/image | Scrape Image Url|
|[**updateRecipeImageApiRecipesSlugImagePut**](#updaterecipeimageapirecipesslugimageput) | **PUT** /api/recipes/{slug}/image | Update Recipe Image|
|[**uploadRecipeAssetApiRecipesSlugAssetsPost**](#uploadrecipeassetapirecipesslugassetspost) | **POST** /api/recipes/{slug}/assets | Upload Recipe Asset|

# **deleteRecipeImageApiRecipesSlugImageDelete**
> any deleteRecipeImageApiRecipesSlugImageDelete()


### Example

```typescript
import {
    RecipeImagesAndAssetsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeImagesAndAssetsApi(configuration);

let slug: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteRecipeImageApiRecipesSlugImageDelete(
    slug,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **slug** | [**string**] |  | defaults to undefined|
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

# **getRecipeAssetApiMediaRecipesRecipeIdAssetsFileNameGet**
> any getRecipeAssetApiMediaRecipesRecipeIdAssetsFileNameGet()

Returns a recipe asset

### Example

```typescript
import {
    RecipeImagesAndAssetsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeImagesAndAssetsApi(configuration);

let recipeId: string; // (default to undefined)
let fileName: string; // (default to undefined)

const { status, data } = await apiInstance.getRecipeAssetApiMediaRecipesRecipeIdAssetsFileNameGet(
    recipeId,
    fileName
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **recipeId** | [**string**] |  | defaults to undefined|
| **fileName** | [**string**] |  | defaults to undefined|


### Return type

**any**

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

# **getRecipeImgApiMediaRecipesRecipeIdImagesFileNameGet**
> any getRecipeImgApiMediaRecipesRecipeIdImagesFileNameGet()

Takes in a recipe id, returns the static image. This route is proxied in the docker image and should not hit the API in production

### Example

```typescript
import {
    RecipeImagesAndAssetsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeImagesAndAssetsApi(configuration);

let recipeId: string; // (default to undefined)
let fileName: ImageType; // (default to undefined)

const { status, data } = await apiInstance.getRecipeImgApiMediaRecipesRecipeIdImagesFileNameGet(
    recipeId,
    fileName
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **recipeId** | [**string**] |  | defaults to undefined|
| **fileName** | **ImageType** |  | defaults to undefined|


### Return type

**any**

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

# **getRecipeTimelineEventImgApiMediaRecipesRecipeIdImagesTimelineTimelineEventIdFileNameGet**
> any getRecipeTimelineEventImgApiMediaRecipesRecipeIdImagesTimelineTimelineEventIdFileNameGet()

Takes in a recipe id and event timeline id, returns the static image. This route is proxied in the docker image and should not hit the API in production

### Example

```typescript
import {
    RecipeImagesAndAssetsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeImagesAndAssetsApi(configuration);

let recipeId: string; // (default to undefined)
let timelineEventId: string; // (default to undefined)
let fileName: ImageType; // (default to undefined)

const { status, data } = await apiInstance.getRecipeTimelineEventImgApiMediaRecipesRecipeIdImagesTimelineTimelineEventIdFileNameGet(
    recipeId,
    timelineEventId,
    fileName
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **recipeId** | [**string**] |  | defaults to undefined|
| **timelineEventId** | [**string**] |  | defaults to undefined|
| **fileName** | **ImageType** |  | defaults to undefined|


### Return type

**any**

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

# **getUserImageApiMediaUsersUserIdFileNameGet**
> getUserImageApiMediaUsersUserIdFileNameGet()

Takes in a recipe slug, returns the static image. This route is proxied in the docker image and should not hit the API in production

### Example

```typescript
import {
    RecipeImagesAndAssetsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeImagesAndAssetsApi(configuration);

let userId: string; // (default to undefined)
let fileName: string; // (default to undefined)

const { status, data } = await apiInstance.getUserImageApiMediaUsersUserIdFileNameGet(
    userId,
    fileName
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**string**] |  | defaults to undefined|
| **fileName** | [**string**] |  | defaults to undefined|


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

# **getValidationTextApiMediaDockerValidateTxtGet**
> getValidationTextApiMediaDockerValidateTxtGet()


### Example

```typescript
import {
    RecipeImagesAndAssetsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeImagesAndAssetsApi(configuration);

const { status, data } = await apiInstance.getValidationTextApiMediaDockerValidateTxtGet();
```

### Parameters
This endpoint does not have any parameters.


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **scrapeImageUrlApiRecipesSlugImagePost**
> any scrapeImageUrlApiRecipesSlugImagePost(scrapeRecipe)


### Example

```typescript
import {
    RecipeImagesAndAssetsApi,
    Configuration,
    ScrapeRecipe
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeImagesAndAssetsApi(configuration);

let slug: string; // (default to undefined)
let scrapeRecipe: ScrapeRecipe; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.scrapeImageUrlApiRecipesSlugImagePost(
    slug,
    scrapeRecipe,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **scrapeRecipe** | **ScrapeRecipe**|  | |
| **slug** | [**string**] |  | defaults to undefined|
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
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateRecipeImageApiRecipesSlugImagePut**
> UpdateImageResponse updateRecipeImageApiRecipesSlugImagePut()


### Example

```typescript
import {
    RecipeImagesAndAssetsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeImagesAndAssetsApi(configuration);

let slug: string; // (default to undefined)
let image: File; // (default to undefined)
let extension: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateRecipeImageApiRecipesSlugImagePut(
    slug,
    image,
    extension,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **slug** | [**string**] |  | defaults to undefined|
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

# **uploadRecipeAssetApiRecipesSlugAssetsPost**
> RecipeAsset uploadRecipeAssetApiRecipesSlugAssetsPost()

Upload a file to store as a recipe asset

### Example

```typescript
import {
    RecipeImagesAndAssetsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeImagesAndAssetsApi(configuration);

let slug: string; // (default to undefined)
let name: string; // (default to undefined)
let icon: string; // (default to undefined)
let extension: string; // (default to undefined)
let file: File; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.uploadRecipeAssetApiRecipesSlugAssetsPost(
    slug,
    name,
    icon,
    extension,
    file,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **slug** | [**string**] |  | defaults to undefined|
| **name** | [**string**] |  | defaults to undefined|
| **icon** | [**string**] |  | defaults to undefined|
| **extension** | [**string**] |  | defaults to undefined|
| **file** | [**File**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**RecipeAsset**

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

