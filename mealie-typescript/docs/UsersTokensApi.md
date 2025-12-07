# UsersTokensApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createApiTokenApiUsersApiTokensPost**](#createapitokenapiusersapitokenspost) | **POST** /api/users/api-tokens | Create Api Token|
|[**deleteApiTokenApiUsersApiTokensTokenIdDelete**](#deleteapitokenapiusersapitokenstokeniddelete) | **DELETE** /api/users/api-tokens/{token_id} | Delete Api Token|

# **createApiTokenApiUsersApiTokensPost**
> LongLiveTokenCreateResponse createApiTokenApiUsersApiTokensPost(longLiveTokenIn)

Create api_token in the Database

### Example

```typescript
import {
    UsersTokensApi,
    Configuration,
    LongLiveTokenIn
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersTokensApi(configuration);

let longLiveTokenIn: LongLiveTokenIn; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createApiTokenApiUsersApiTokensPost(
    longLiveTokenIn,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **longLiveTokenIn** | **LongLiveTokenIn**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**LongLiveTokenCreateResponse**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteApiTokenApiUsersApiTokensTokenIdDelete**
> DeleteTokenResponse deleteApiTokenApiUsersApiTokensTokenIdDelete()

Delete api_token from the Database

### Example

```typescript
import {
    UsersTokensApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersTokensApi(configuration);

let tokenId: number; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteApiTokenApiUsersApiTokensTokenIdDelete(
    tokenId,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tokenId** | [**number**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**DeleteTokenResponse**

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

