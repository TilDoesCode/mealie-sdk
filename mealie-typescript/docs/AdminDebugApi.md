# AdminDebugApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**debugOpenaiApiAdminDebugOpenaiPost**](#debugopenaiapiadmindebugopenaipost) | **POST** /api/admin/debug/openai | Debug Openai|

# **debugOpenaiApiAdminDebugOpenaiPost**
> DebugResponse debugOpenaiApiAdminDebugOpenaiPost()


### Example

```typescript
import {
    AdminDebugApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminDebugApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)
let image: File; // (optional) (default to undefined)

const { status, data } = await apiInstance.debugOpenaiApiAdminDebugOpenaiPost(
    acceptLanguage,
    image
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|
| **image** | [**File**] |  | (optional) defaults to undefined|


### Return type

**DebugResponse**

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

