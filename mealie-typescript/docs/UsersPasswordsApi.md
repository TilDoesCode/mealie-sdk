# UsersPasswordsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**forgotPasswordApiUsersForgotPasswordPost**](#forgotpasswordapiusersforgotpasswordpost) | **POST** /api/users/forgot-password | Forgot Password|
|[**resetPasswordApiUsersResetPasswordPost**](#resetpasswordapiusersresetpasswordpost) | **POST** /api/users/reset-password | Reset Password|

# **forgotPasswordApiUsersForgotPasswordPost**
> any forgotPasswordApiUsersForgotPasswordPost(forgotPassword)

Sends an email with a reset link to the user

### Example

```typescript
import {
    UsersPasswordsApi,
    Configuration,
    ForgotPassword
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersPasswordsApi(configuration);

let forgotPassword: ForgotPassword; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.forgotPasswordApiUsersForgotPasswordPost(
    forgotPassword,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **forgotPassword** | **ForgotPassword**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **resetPasswordApiUsersResetPasswordPost**
> any resetPasswordApiUsersResetPasswordPost(resetPassword)

Resets the user password

### Example

```typescript
import {
    UsersPasswordsApi,
    Configuration,
    ResetPassword
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersPasswordsApi(configuration);

let resetPassword: ResetPassword; //

const { status, data } = await apiInstance.resetPasswordApiUsersResetPasswordPost(
    resetPassword
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **resetPassword** | **ResetPassword**|  | |


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

