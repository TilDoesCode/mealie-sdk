# GroupsSelfServiceApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getGroupMemberApiGroupsMembersUsernameOrIdGet**](#getgroupmemberapigroupsmembersusernameoridget) | **GET** /api/groups/members/{username_or_id} | Get Group Member|
|[**getGroupMembersApiGroupsMembersGet**](#getgroupmembersapigroupsmembersget) | **GET** /api/groups/members | Get Group Members|
|[**getGroupPreferencesApiGroupsPreferencesGet**](#getgrouppreferencesapigroupspreferencesget) | **GET** /api/groups/preferences | Get Group Preferences|
|[**getLoggedInUserGroupApiGroupsSelfGet**](#getloggedinusergroupapigroupsselfget) | **GET** /api/groups/self | Get Logged In User Group|
|[**getStorageApiGroupsStorageGet**](#getstorageapigroupsstorageget) | **GET** /api/groups/storage | Get Storage|
|[**updateGroupPreferencesApiGroupsPreferencesPut**](#updategrouppreferencesapigroupspreferencesput) | **PUT** /api/groups/preferences | Update Group Preferences|

# **getGroupMemberApiGroupsMembersUsernameOrIdGet**
> UserSummary getGroupMemberApiGroupsMembersUsernameOrIdGet()

Returns a single user belonging to the current group

### Example

```typescript
import {
    GroupsSelfServiceApi,
    Configuration,
    UsernameOrId
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new GroupsSelfServiceApi(configuration);

let usernameOrId: UsernameOrId; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getGroupMemberApiGroupsMembersUsernameOrIdGet(
    usernameOrId,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **usernameOrId** | **UsernameOrId** |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**UserSummary**

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

# **getGroupMembersApiGroupsMembersGet**
> PaginationBaseUserSummary getGroupMembersApiGroupsMembersGet()

Returns all users belonging to the current group

### Example

```typescript
import {
    GroupsSelfServiceApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new GroupsSelfServiceApi(configuration);

let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getGroupMembersApiGroupsMembersGet(
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

**PaginationBaseUserSummary**

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

# **getGroupPreferencesApiGroupsPreferencesGet**
> ReadGroupPreferences getGroupPreferencesApiGroupsPreferencesGet()


### Example

```typescript
import {
    GroupsSelfServiceApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new GroupsSelfServiceApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getGroupPreferencesApiGroupsPreferencesGet(
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ReadGroupPreferences**

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

# **getLoggedInUserGroupApiGroupsSelfGet**
> GroupSummary getLoggedInUserGroupApiGroupsSelfGet()

Returns the Group Data for the Current User

### Example

```typescript
import {
    GroupsSelfServiceApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new GroupsSelfServiceApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getLoggedInUserGroupApiGroupsSelfGet(
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**GroupSummary**

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

# **getStorageApiGroupsStorageGet**
> GroupStorage getStorageApiGroupsStorageGet()


### Example

```typescript
import {
    GroupsSelfServiceApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new GroupsSelfServiceApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getStorageApiGroupsStorageGet(
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**GroupStorage**

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

# **updateGroupPreferencesApiGroupsPreferencesPut**
> ReadGroupPreferences updateGroupPreferencesApiGroupsPreferencesPut(updateGroupPreferences)


### Example

```typescript
import {
    GroupsSelfServiceApi,
    Configuration,
    UpdateGroupPreferences
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new GroupsSelfServiceApi(configuration);

let updateGroupPreferences: UpdateGroupPreferences; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateGroupPreferencesApiGroupsPreferencesPut(
    updateGroupPreferences,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateGroupPreferences** | **UpdateGroupPreferences**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ReadGroupPreferences**

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

