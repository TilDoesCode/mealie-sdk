# RecipeBulkActionsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**bulkCategorizeRecipesApiRecipesBulkActionsCategorizePost**](#bulkcategorizerecipesapirecipesbulkactionscategorizepost) | **POST** /api/recipes/bulk-actions/categorize | Bulk Categorize Recipes|
|[**bulkDeleteRecipesApiRecipesBulkActionsDeletePost**](#bulkdeleterecipesapirecipesbulkactionsdeletepost) | **POST** /api/recipes/bulk-actions/delete | Bulk Delete Recipes|
|[**bulkExportRecipesApiRecipesBulkActionsExportPost**](#bulkexportrecipesapirecipesbulkactionsexportpost) | **POST** /api/recipes/bulk-actions/export | Bulk Export Recipes|
|[**bulkSettingsRecipesApiRecipesBulkActionsSettingsPost**](#bulksettingsrecipesapirecipesbulkactionssettingspost) | **POST** /api/recipes/bulk-actions/settings | Bulk Settings Recipes|
|[**bulkTagRecipesApiRecipesBulkActionsTagPost**](#bulktagrecipesapirecipesbulkactionstagpost) | **POST** /api/recipes/bulk-actions/tag | Bulk Tag Recipes|
|[**getExportedDataApiRecipesBulkActionsExportGet**](#getexporteddataapirecipesbulkactionsexportget) | **GET** /api/recipes/bulk-actions/export | Get Exported Data|
|[**getExportedDataTokenApiRecipesBulkActionsExportDownloadGet**](#getexporteddatatokenapirecipesbulkactionsexportdownloadget) | **GET** /api/recipes/bulk-actions/export/download | Get Exported Data Token|
|[**purgeExportDataApiRecipesBulkActionsExportPurgeDelete**](#purgeexportdataapirecipesbulkactionsexportpurgedelete) | **DELETE** /api/recipes/bulk-actions/export/purge | Purge Export Data|

# **bulkCategorizeRecipesApiRecipesBulkActionsCategorizePost**
> any bulkCategorizeRecipesApiRecipesBulkActionsCategorizePost(assignCategories)


### Example

```typescript
import {
    RecipeBulkActionsApi,
    Configuration,
    AssignCategories
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeBulkActionsApi(configuration);

let assignCategories: AssignCategories; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.bulkCategorizeRecipesApiRecipesBulkActionsCategorizePost(
    assignCategories,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **assignCategories** | **AssignCategories**|  | |
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

# **bulkDeleteRecipesApiRecipesBulkActionsDeletePost**
> any bulkDeleteRecipesApiRecipesBulkActionsDeletePost(deleteRecipes)


### Example

```typescript
import {
    RecipeBulkActionsApi,
    Configuration,
    DeleteRecipes
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeBulkActionsApi(configuration);

let deleteRecipes: DeleteRecipes; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.bulkDeleteRecipesApiRecipesBulkActionsDeletePost(
    deleteRecipes,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **deleteRecipes** | **DeleteRecipes**|  | |
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

# **bulkExportRecipesApiRecipesBulkActionsExportPost**
> any bulkExportRecipesApiRecipesBulkActionsExportPost(exportRecipes)


### Example

```typescript
import {
    RecipeBulkActionsApi,
    Configuration,
    ExportRecipes
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeBulkActionsApi(configuration);

let exportRecipes: ExportRecipes; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.bulkExportRecipesApiRecipesBulkActionsExportPost(
    exportRecipes,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **exportRecipes** | **ExportRecipes**|  | |
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

# **bulkSettingsRecipesApiRecipesBulkActionsSettingsPost**
> any bulkSettingsRecipesApiRecipesBulkActionsSettingsPost(assignSettings)


### Example

```typescript
import {
    RecipeBulkActionsApi,
    Configuration,
    AssignSettings
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeBulkActionsApi(configuration);

let assignSettings: AssignSettings; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.bulkSettingsRecipesApiRecipesBulkActionsSettingsPost(
    assignSettings,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **assignSettings** | **AssignSettings**|  | |
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

# **bulkTagRecipesApiRecipesBulkActionsTagPost**
> any bulkTagRecipesApiRecipesBulkActionsTagPost(assignTags)


### Example

```typescript
import {
    RecipeBulkActionsApi,
    Configuration,
    AssignTags
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeBulkActionsApi(configuration);

let assignTags: AssignTags; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.bulkTagRecipesApiRecipesBulkActionsTagPost(
    assignTags,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **assignTags** | **AssignTags**|  | |
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

# **getExportedDataApiRecipesBulkActionsExportGet**
> Array<GroupDataExport> getExportedDataApiRecipesBulkActionsExportGet()


### Example

```typescript
import {
    RecipeBulkActionsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeBulkActionsApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getExportedDataApiRecipesBulkActionsExportGet(
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Array<GroupDataExport>**

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

# **getExportedDataTokenApiRecipesBulkActionsExportDownloadGet**
> any getExportedDataTokenApiRecipesBulkActionsExportDownloadGet()

Returns a token to download a file

### Example

```typescript
import {
    RecipeBulkActionsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeBulkActionsApi(configuration);

let path: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getExportedDataTokenApiRecipesBulkActionsExportDownloadGet(
    path,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **path** | [**string**] |  | defaults to undefined|
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

# **purgeExportDataApiRecipesBulkActionsExportPurgeDelete**
> SuccessResponse purgeExportDataApiRecipesBulkActionsExportPurgeDelete()

Remove all exports data, including items on disk without database entry

### Example

```typescript
import {
    RecipeBulkActionsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeBulkActionsApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.purgeExportDataApiRecipesBulkActionsExportPurgeDelete(
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**SuccessResponse**

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

