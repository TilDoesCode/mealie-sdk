# UsersRegistrationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**registerNewUserApiUsersRegisterPost**](#registernewuserapiusersregisterpost) | **POST** /api/users/register | Register New User|

# **registerNewUserApiUsersRegisterPost**
> UserOut registerNewUserApiUsersRegisterPost(createUserRegistration)


### Example

```typescript
import {
    UsersRegistrationApi,
    Configuration,
    CreateUserRegistration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersRegistrationApi(configuration);

let createUserRegistration: CreateUserRegistration; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.registerNewUserApiUsersRegisterPost(
    createUserRegistration,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createUserRegistration** | **CreateUserRegistration**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**UserOut**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

