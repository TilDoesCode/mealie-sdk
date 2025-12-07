# AdminManageUsersApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createOneApiAdminUsersPost**](#createoneapiadminuserspost) | **POST** /api/admin/users | Create One|
|[**deleteOneApiAdminUsersItemIdDelete**](#deleteoneapiadminusersitemiddelete) | **DELETE** /api/admin/users/{item_id} | Delete One|
|[**generateTokenApiAdminUsersPasswordResetTokenPost**](#generatetokenapiadminuserspasswordresettokenpost) | **POST** /api/admin/users/password-reset-token | Generate Token|
|[**getAllApiAdminUsersGet**](#getallapiadminusersget) | **GET** /api/admin/users | Get All|
|[**getOneApiAdminUsersItemIdGet**](#getoneapiadminusersitemidget) | **GET** /api/admin/users/{item_id} | Get One|
|[**unlockUsersApiAdminUsersUnlockPost**](#unlockusersapiadminusersunlockpost) | **POST** /api/admin/users/unlock | Unlock Users|
|[**updateOneApiAdminUsersItemIdPut**](#updateoneapiadminusersitemidput) | **PUT** /api/admin/users/{item_id} | Update One|

# **createOneApiAdminUsersPost**
> UserOut createOneApiAdminUsersPost(userIn)


### Example

```typescript
import {
    AdminManageUsersApi,
    Configuration,
    UserIn
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminManageUsersApi(configuration);

let userIn: UserIn; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createOneApiAdminUsersPost(
    userIn,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userIn** | **UserIn**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**UserOut**

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

# **deleteOneApiAdminUsersItemIdDelete**
> UserOut deleteOneApiAdminUsersItemIdDelete()


### Example

```typescript
import {
    AdminManageUsersApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminManageUsersApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteOneApiAdminUsersItemIdDelete(
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

**UserOut**

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

# **generateTokenApiAdminUsersPasswordResetTokenPost**
> PasswordResetToken generateTokenApiAdminUsersPasswordResetTokenPost(forgotPassword)

Generates a reset token and returns it. This is an authenticated endpoint

### Example

```typescript
import {
    AdminManageUsersApi,
    Configuration,
    ForgotPassword
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminManageUsersApi(configuration);

let forgotPassword: ForgotPassword; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.generateTokenApiAdminUsersPasswordResetTokenPost(
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

**PasswordResetToken**

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

# **getAllApiAdminUsersGet**
> UserPagination getAllApiAdminUsersGet()


### Example

```typescript
import {
    AdminManageUsersApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminManageUsersApi(configuration);

let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiAdminUsersGet(
    orderBy,
    orderByNullPosition,
    orderDirection,
    queryFilter,
    paginationSeed,
    page,
    perPage,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **orderBy** | [**string**] |  | (optional) defaults to undefined|
| **orderByNullPosition** | **OrderByNullPosition** |  | (optional) defaults to undefined|
| **orderDirection** | **OrderDirection** |  | (optional) defaults to undefined|
| **queryFilter** | [**string**] |  | (optional) defaults to undefined|
| **paginationSeed** | [**string**] |  | (optional) defaults to undefined|
| **page** | [**number**] |  | (optional) defaults to 1|
| **perPage** | [**number**] |  | (optional) defaults to 50|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**UserPagination**

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

# **getOneApiAdminUsersItemIdGet**
> UserOut getOneApiAdminUsersItemIdGet()


### Example

```typescript
import {
    AdminManageUsersApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminManageUsersApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiAdminUsersItemIdGet(
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

**UserOut**

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

# **unlockUsersApiAdminUsersUnlockPost**
> UnlockResults unlockUsersApiAdminUsersUnlockPost()


### Example

```typescript
import {
    AdminManageUsersApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminManageUsersApi(configuration);

let force: boolean; // (optional) (default to false)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.unlockUsersApiAdminUsersUnlockPost(
    force,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **force** | [**boolean**] |  | (optional) defaults to false|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**UnlockResults**

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

# **updateOneApiAdminUsersItemIdPut**
> UserOut updateOneApiAdminUsersItemIdPut(userOut)


### Example

```typescript
import {
    AdminManageUsersApi,
    Configuration,
    UserOut
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminManageUsersApi(configuration);

let itemId: string; // (default to undefined)
let userOut: UserOut; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateOneApiAdminUsersItemIdPut(
    itemId,
    userOut,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userOut** | **UserOut**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**UserOut**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

