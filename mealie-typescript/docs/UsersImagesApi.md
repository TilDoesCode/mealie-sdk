# UsersImagesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**updateUserImageApiUsersIdImagePost**](#updateuserimageapiusersidimagepost) | **POST** /api/users/{id}/image | Update User Image|

# **updateUserImageApiUsersIdImagePost**
> any updateUserImageApiUsersIdImagePost()

Updates a User Image

### Example

```typescript
import {
    UsersImagesApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersImagesApi(configuration);

let id: string; // (default to undefined)
let profile: File; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateUserImageApiUsersIdImagePost(
    id,
    profile,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **profile** | [**File**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**any**

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

