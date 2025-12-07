# UtilsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**downloadFileApiUtilsDownloadGet**](#downloadfileapiutilsdownloadget) | **GET** /api/utils/download | Download File|

# **downloadFileApiUtilsDownloadGet**
> any downloadFileApiUtilsDownloadGet()

Uses a file token obtained by an active user to retrieve a file from the operating system.

### Example

```typescript
import {
    UtilsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UtilsApi(configuration);

let token: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.downloadFileApiUtilsDownloadGet(
    token
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **token** | [**string**] |  | (optional) defaults to undefined|


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

