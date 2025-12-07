# GroupsReportsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**deleteOneApiGroupsReportsItemIdDelete**](#deleteoneapigroupsreportsitemiddelete) | **DELETE** /api/groups/reports/{item_id} | Delete One|
|[**getAllApiGroupsReportsGet**](#getallapigroupsreportsget) | **GET** /api/groups/reports | Get All|
|[**getOneApiGroupsReportsItemIdGet**](#getoneapigroupsreportsitemidget) | **GET** /api/groups/reports/{item_id} | Get One|

# **deleteOneApiGroupsReportsItemIdDelete**
> any deleteOneApiGroupsReportsItemIdDelete()


### Example

```typescript
import {
    GroupsReportsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new GroupsReportsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteOneApiGroupsReportsItemIdDelete(
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

# **getAllApiGroupsReportsGet**
> Array<ReportSummary> getAllApiGroupsReportsGet()


### Example

```typescript
import {
    GroupsReportsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new GroupsReportsApi(configuration);

let reportType: ReportCategory; // (optional) (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiGroupsReportsGet(
    reportType,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **reportType** | **ReportCategory** |  | (optional) defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Array<ReportSummary>**

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

# **getOneApiGroupsReportsItemIdGet**
> ReportOut getOneApiGroupsReportsItemIdGet()


### Example

```typescript
import {
    GroupsReportsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new GroupsReportsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiGroupsReportsItemIdGet(
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

**ReportOut**

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

