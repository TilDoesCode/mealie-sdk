# AdminMaintenanceApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**cleanImagesApiAdminMaintenanceCleanImagesPost**](#cleanimagesapiadminmaintenancecleanimagespost) | **POST** /api/admin/maintenance/clean/images | Clean Images|
|[**cleanRecipeFoldersApiAdminMaintenanceCleanRecipeFoldersPost**](#cleanrecipefoldersapiadminmaintenancecleanrecipefolderspost) | **POST** /api/admin/maintenance/clean/recipe-folders | Clean Recipe Folders|
|[**cleanTempApiAdminMaintenanceCleanTempPost**](#cleantempapiadminmaintenancecleantemppost) | **POST** /api/admin/maintenance/clean/temp | Clean Temp|
|[**getMaintenanceSummaryApiAdminMaintenanceGet**](#getmaintenancesummaryapiadminmaintenanceget) | **GET** /api/admin/maintenance | Get Maintenance Summary|
|[**getStorageDetailsApiAdminMaintenanceStorageGet**](#getstoragedetailsapiadminmaintenancestorageget) | **GET** /api/admin/maintenance/storage | Get Storage Details|

# **cleanImagesApiAdminMaintenanceCleanImagesPost**
> SuccessResponse cleanImagesApiAdminMaintenanceCleanImagesPost()

Purges all the images from the filesystem that aren\'t .webp

### Example

```typescript
import {
    AdminMaintenanceApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminMaintenanceApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.cleanImagesApiAdminMaintenanceCleanImagesPost(
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

# **cleanRecipeFoldersApiAdminMaintenanceCleanRecipeFoldersPost**
> SuccessResponse cleanRecipeFoldersApiAdminMaintenanceCleanRecipeFoldersPost()

Deletes all the recipe folders that don\'t have names that are valid UUIDs

### Example

```typescript
import {
    AdminMaintenanceApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminMaintenanceApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.cleanRecipeFoldersApiAdminMaintenanceCleanRecipeFoldersPost(
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

# **cleanTempApiAdminMaintenanceCleanTempPost**
> SuccessResponse cleanTempApiAdminMaintenanceCleanTempPost()


### Example

```typescript
import {
    AdminMaintenanceApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminMaintenanceApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.cleanTempApiAdminMaintenanceCleanTempPost(
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

# **getMaintenanceSummaryApiAdminMaintenanceGet**
> MaintenanceSummary getMaintenanceSummaryApiAdminMaintenanceGet()

Get the maintenance summary

### Example

```typescript
import {
    AdminMaintenanceApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminMaintenanceApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getMaintenanceSummaryApiAdminMaintenanceGet(
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**MaintenanceSummary**

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

# **getStorageDetailsApiAdminMaintenanceStorageGet**
> MaintenanceStorageDetails getStorageDetailsApiAdminMaintenanceStorageGet()


### Example

```typescript
import {
    AdminMaintenanceApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminMaintenanceApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getStorageDetailsApiAdminMaintenanceStorageGet(
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**MaintenanceStorageDetails**

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

