# RecipeExportsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getRecipeAsFormatApiRecipesSlugExportsGet**](#getrecipeasformatapirecipesslugexportsget) | **GET** /api/recipes/{slug}/exports | Get Recipe As Format|
|[**getRecipeFormatsAndTemplatesApiRecipesExportsGet**](#getrecipeformatsandtemplatesapirecipesexportsget) | **GET** /api/recipes/exports | Get Recipe Formats And Templates|

# **getRecipeAsFormatApiRecipesSlugExportsGet**
> getRecipeAsFormatApiRecipesSlugExportsGet()

## Parameters `template_name`: The name of the template to use to use in the exports listed. Template type will automatically be set on the backend. Because of this, it\'s important that your templates have unique names. See available names and formats in the /api/recipes/exports endpoint.

### Example

```typescript
import {
    RecipeExportsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeExportsApi(configuration);

let slug: string; // (default to undefined)
let templateName: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getRecipeAsFormatApiRecipesSlugExportsGet(
    slug,
    templateName,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **slug** | [**string**] |  | defaults to undefined|
| **templateName** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

void (empty response body)

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

# **getRecipeFormatsAndTemplatesApiRecipesExportsGet**
> FormatResponse getRecipeFormatsAndTemplatesApiRecipesExportsGet()


### Example

```typescript
import {
    RecipeExportsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeExportsApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getRecipeFormatsAndTemplatesApiRecipesExportsGet(
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**FormatResponse**

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

