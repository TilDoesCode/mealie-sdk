# UsersAuthenticationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getTokenApiAuthTokenPost**](#gettokenapiauthtokenpost) | **POST** /api/auth/token | Get Token|
|[**logoutApiAuthLogoutPost**](#logoutapiauthlogoutpost) | **POST** /api/auth/logout | Logout|
|[**oauthCallbackApiAuthOauthCallbackGet**](#oauthcallbackapiauthoauthcallbackget) | **GET** /api/auth/oauth/callback | Oauth Callback|
|[**oauthLoginApiAuthOauthGet**](#oauthloginapiauthoauthget) | **GET** /api/auth/oauth | Oauth Login|
|[**refreshTokenApiAuthRefreshGet**](#refreshtokenapiauthrefreshget) | **GET** /api/auth/refresh | Refresh Token|

# **getTokenApiAuthTokenPost**
> any getTokenApiAuthTokenPost()


### Example

```typescript
import {
    UsersAuthenticationApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersAuthenticationApi(configuration);

let username: string; // (optional) (default to '')
let password: string; // (optional) (default to '')
let rememberMe: boolean; // (optional) (default to false)

const { status, data } = await apiInstance.getTokenApiAuthTokenPost(
    username,
    password,
    rememberMe
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | (optional) defaults to ''|
| **password** | [**string**] |  | (optional) defaults to ''|
| **rememberMe** | [**boolean**] |  | (optional) defaults to false|


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **logoutApiAuthLogoutPost**
> any logoutApiAuthLogoutPost()


### Example

```typescript
import {
    UsersAuthenticationApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersAuthenticationApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.logoutApiAuthLogoutPost(
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
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

# **oauthCallbackApiAuthOauthCallbackGet**
> any oauthCallbackApiAuthOauthCallbackGet()


### Example

```typescript
import {
    UsersAuthenticationApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersAuthenticationApi(configuration);

const { status, data } = await apiInstance.oauthCallbackApiAuthOauthCallbackGet();
```

### Parameters
This endpoint does not have any parameters.


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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **oauthLoginApiAuthOauthGet**
> any oauthLoginApiAuthOauthGet()


### Example

```typescript
import {
    UsersAuthenticationApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersAuthenticationApi(configuration);

const { status, data } = await apiInstance.oauthLoginApiAuthOauthGet();
```

### Parameters
This endpoint does not have any parameters.


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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **refreshTokenApiAuthRefreshGet**
> any refreshTokenApiAuthRefreshGet()

Use a valid token to get another token

### Example

```typescript
import {
    UsersAuthenticationApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersAuthenticationApi(configuration);

const { status, data } = await apiInstance.refreshTokenApiAuthRefreshGet();
```

### Parameters
This endpoint does not have any parameters.


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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

