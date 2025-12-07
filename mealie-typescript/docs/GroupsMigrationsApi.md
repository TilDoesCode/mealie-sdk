# GroupsMigrationsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**startDataMigrationApiGroupsMigrationsPost**](#startdatamigrationapigroupsmigrationspost) | **POST** /api/groups/migrations | Start Data Migration|

# **startDataMigrationApiGroupsMigrationsPost**
> ReportSummary startDataMigrationApiGroupsMigrationsPost()


### Example

```typescript
import {
    GroupsMigrationsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new GroupsMigrationsApi(configuration);

let migrationType: SupportedMigrations; // (default to undefined)
let archive: File; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)
let addMigrationTag: boolean; // (optional) (default to false)

const { status, data } = await apiInstance.startDataMigrationApiGroupsMigrationsPost(
    migrationType,
    archive,
    acceptLanguage,
    addMigrationTag
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **migrationType** | **SupportedMigrations** |  | defaults to undefined|
| **archive** | [**File**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|
| **addMigrationTag** | [**boolean**] |  | (optional) defaults to false|


### Return type

**ReportSummary**

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

