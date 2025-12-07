# UsersRatingsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**addFavoriteApiUsersIdFavoritesSlugPost**](#addfavoriteapiusersidfavoritesslugpost) | **POST** /api/users/{id}/favorites/{slug} | Add Favorite|
|[**getFavoritesApiUsersIdFavoritesGet**](#getfavoritesapiusersidfavoritesget) | **GET** /api/users/{id}/favorites | Get Favorites|
|[**getRatingsApiUsersIdRatingsGet**](#getratingsapiusersidratingsget) | **GET** /api/users/{id}/ratings | Get Ratings|
|[**removeFavoriteApiUsersIdFavoritesSlugDelete**](#removefavoriteapiusersidfavoritesslugdelete) | **DELETE** /api/users/{id}/favorites/{slug} | Remove Favorite|
|[**setRatingApiUsersIdRatingsSlugPost**](#setratingapiusersidratingsslugpost) | **POST** /api/users/{id}/ratings/{slug} | Set Rating|

# **addFavoriteApiUsersIdFavoritesSlugPost**
> any addFavoriteApiUsersIdFavoritesSlugPost()

Adds a recipe to the user\'s favorites

### Example

```typescript
import {
    UsersRatingsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersRatingsApi(configuration);

let id: string; // (default to undefined)
let slug: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.addFavoriteApiUsersIdFavoritesSlugPost(
    id,
    slug,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **slug** | [**string**] |  | defaults to undefined|
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

# **getFavoritesApiUsersIdFavoritesGet**
> UserRatingsUserRatingOut getFavoritesApiUsersIdFavoritesGet()

Get user\'s favorited recipes

### Example

```typescript
import {
    UsersRatingsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersRatingsApi(configuration);

let id: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getFavoritesApiUsersIdFavoritesGet(
    id,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**UserRatingsUserRatingOut**

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

# **getRatingsApiUsersIdRatingsGet**
> UserRatingsUserRatingOut getRatingsApiUsersIdRatingsGet()

Get user\'s rated recipes

### Example

```typescript
import {
    UsersRatingsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersRatingsApi(configuration);

let id: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getRatingsApiUsersIdRatingsGet(
    id,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**UserRatingsUserRatingOut**

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

# **removeFavoriteApiUsersIdFavoritesSlugDelete**
> any removeFavoriteApiUsersIdFavoritesSlugDelete()

Removes a recipe from the user\'s favorites

### Example

```typescript
import {
    UsersRatingsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersRatingsApi(configuration);

let id: string; // (default to undefined)
let slug: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.removeFavoriteApiUsersIdFavoritesSlugDelete(
    id,
    slug,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **slug** | [**string**] |  | defaults to undefined|
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

# **setRatingApiUsersIdRatingsSlugPost**
> any setRatingApiUsersIdRatingsSlugPost(userRatingUpdate)

Sets the user\'s rating for a recipe

### Example

```typescript
import {
    UsersRatingsApi,
    Configuration,
    UserRatingUpdate
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new UsersRatingsApi(configuration);

let id: string; // (default to undefined)
let slug: string; // (default to undefined)
let userRatingUpdate: UserRatingUpdate; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.setRatingApiUsersIdRatingsSlugPost(
    id,
    slug,
    userRatingUpdate,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userRatingUpdate** | **UserRatingUpdate**|  | |
| **id** | [**string**] |  | defaults to undefined|
| **slug** | [**string**] |  | defaults to undefined|
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

