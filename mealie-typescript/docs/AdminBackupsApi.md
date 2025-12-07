# AdminBackupsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createOneApiAdminBackupsPost**](#createoneapiadminbackupspost) | **POST** /api/admin/backups | Create One|
|[**deleteOneApiAdminBackupsFileNameDelete**](#deleteoneapiadminbackupsfilenamedelete) | **DELETE** /api/admin/backups/{file_name} | Delete One|
|[**getAllApiAdminBackupsGet**](#getallapiadminbackupsget) | **GET** /api/admin/backups | Get All|
|[**getOneApiAdminBackupsFileNameGet**](#getoneapiadminbackupsfilenameget) | **GET** /api/admin/backups/{file_name} | Get One|
|[**importOneApiAdminBackupsFileNameRestorePost**](#importoneapiadminbackupsfilenamerestorepost) | **POST** /api/admin/backups/{file_name}/restore | Import One|
|[**uploadOneApiAdminBackupsUploadPost**](#uploadoneapiadminbackupsuploadpost) | **POST** /api/admin/backups/upload | Upload One|

# **createOneApiAdminBackupsPost**
> SuccessResponse createOneApiAdminBackupsPost()


### Example

```typescript
import {
    AdminBackupsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminBackupsApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createOneApiAdminBackupsPost(
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
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteOneApiAdminBackupsFileNameDelete**
> SuccessResponse deleteOneApiAdminBackupsFileNameDelete()


### Example

```typescript
import {
    AdminBackupsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminBackupsApi(configuration);

let fileName: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteOneApiAdminBackupsFileNameDelete(
    fileName,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **fileName** | [**string**] |  | defaults to undefined|
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

# **getAllApiAdminBackupsGet**
> AllBackups getAllApiAdminBackupsGet()


### Example

```typescript
import {
    AdminBackupsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminBackupsApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiAdminBackupsGet(
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**AllBackups**

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

# **getOneApiAdminBackupsFileNameGet**
> FileTokenResponse getOneApiAdminBackupsFileNameGet()

Returns a token to download a file

### Example

```typescript
import {
    AdminBackupsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminBackupsApi(configuration);

let fileName: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiAdminBackupsFileNameGet(
    fileName,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **fileName** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**FileTokenResponse**

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

# **importOneApiAdminBackupsFileNameRestorePost**
> SuccessResponse importOneApiAdminBackupsFileNameRestorePost()


### Example

```typescript
import {
    AdminBackupsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminBackupsApi(configuration);

let fileName: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.importOneApiAdminBackupsFileNameRestorePost(
    fileName,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **fileName** | [**string**] |  | defaults to undefined|
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

# **uploadOneApiAdminBackupsUploadPost**
> SuccessResponse uploadOneApiAdminBackupsUploadPost()

Upload a .zip File to later be imported into Mealie

### Example

```typescript
import {
    AdminBackupsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminBackupsApi(configuration);

let archive: File; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.uploadOneApiAdminBackupsUploadPost(
    archive,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **archive** | [**File**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**SuccessResponse**

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

