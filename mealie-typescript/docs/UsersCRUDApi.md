# UsersCRUDApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getLoggedInUserApiUsersSelfGet**](#getloggedinuserapiusersselfget) | **GET** /api/users/self | Get Logged In User|
|[**getLoggedInUserFavoritesApiUsersSelfFavoritesGet**](#getloggedinuserfavoritesapiusersselffavoritesget) | **GET** /api/users/self/favorites | Get Logged In User Favorites|
|[**getLoggedInUserRatingForRecipeApiUsersSelfRatingsRecipeIdGet**](#getloggedinuserratingforrecipeapiusersselfratingsrecipeidget) | **GET** /api/users/self/ratings/{recipe_id} | Get Logged In User Rating For Recipe|
|[**getLoggedInUserRatingsApiUsersSelfRatingsGet**](#getloggedinuserratingsapiusersselfratingsget) | **GET** /api/users/self/ratings | Get Logged In User Ratings|
|[**updatePasswordApiUsersPasswordPut**](#updatepasswordapiuserspasswordput) | **PUT** /api/users/password | Update Password|
|[**updateUserApiUsersItemIdPut**](#updateuserapiusersitemidput) | **PUT** /api/users/{item_id} | Update User|

# **getLoggedInUserApiUsersSelfGet**
> UserOut getLoggedInUserApiUsersSelfGet()


### Example

```typescript
import {
    UsersCRUDApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersCRUDApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getLoggedInUserApiUsersSelfGet(
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
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

# **getLoggedInUserFavoritesApiUsersSelfFavoritesGet**
> UserRatingsUserRatingSummary getLoggedInUserFavoritesApiUsersSelfFavoritesGet()


### Example

```typescript
import {
    UsersCRUDApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersCRUDApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getLoggedInUserFavoritesApiUsersSelfFavoritesGet(
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**UserRatingsUserRatingSummary**

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

# **getLoggedInUserRatingForRecipeApiUsersSelfRatingsRecipeIdGet**
> UserRatingSummary getLoggedInUserRatingForRecipeApiUsersSelfRatingsRecipeIdGet()


### Example

```typescript
import {
    UsersCRUDApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersCRUDApi(configuration);

let recipeId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getLoggedInUserRatingForRecipeApiUsersSelfRatingsRecipeIdGet(
    recipeId,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **recipeId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**UserRatingSummary**

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

# **getLoggedInUserRatingsApiUsersSelfRatingsGet**
> UserRatingsUserRatingSummary getLoggedInUserRatingsApiUsersSelfRatingsGet()


### Example

```typescript
import {
    UsersCRUDApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersCRUDApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getLoggedInUserRatingsApiUsersSelfRatingsGet(
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**UserRatingsUserRatingSummary**

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

# **updatePasswordApiUsersPasswordPut**
> any updatePasswordApiUsersPasswordPut(changePassword)

Resets the User Password

### Example

```typescript
import {
    UsersCRUDApi,
    Configuration,
    ChangePassword
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersCRUDApi(configuration);

let changePassword: ChangePassword; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updatePasswordApiUsersPasswordPut(
    changePassword,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **changePassword** | **ChangePassword**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**any**

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

# **updateUserApiUsersItemIdPut**
> any updateUserApiUsersItemIdPut(mealieSchemaUserUserUserBase)


### Example

```typescript
import {
    UsersCRUDApi,
    Configuration,
    MealieSchemaUserUserUserBase
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersCRUDApi(configuration);

let itemId: string; // (default to undefined)
let mealieSchemaUserUserUserBase: MealieSchemaUserUserUserBase; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateUserApiUsersItemIdPut(
    itemId,
    mealieSchemaUserUserUserBase,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **mealieSchemaUserUserUserBase** | **MealieSchemaUserUserUserBase**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**any**

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

