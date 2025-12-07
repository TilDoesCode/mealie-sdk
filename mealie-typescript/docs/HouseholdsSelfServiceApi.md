# HouseholdsSelfServiceApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getHouseholdMembersApiHouseholdsMembersGet**](#gethouseholdmembersapihouseholdsmembersget) | **GET** /api/households/members | Get Household Members|
|[**getHouseholdPreferencesApiHouseholdsPreferencesGet**](#gethouseholdpreferencesapihouseholdspreferencesget) | **GET** /api/households/preferences | Get Household Preferences|
|[**getHouseholdRecipeApiHouseholdsSelfRecipesRecipeSlugGet**](#gethouseholdrecipeapihouseholdsselfrecipesrecipeslugget) | **GET** /api/households/self/recipes/{recipe_slug} | Get Household Recipe|
|[**getLoggedInUserHouseholdApiHouseholdsSelfGet**](#getloggedinuserhouseholdapihouseholdsselfget) | **GET** /api/households/self | Get Logged In User Household|
|[**getStatisticsApiHouseholdsStatisticsGet**](#getstatisticsapihouseholdsstatisticsget) | **GET** /api/households/statistics | Get Statistics|
|[**setMemberPermissionsApiHouseholdsPermissionsPut**](#setmemberpermissionsapihouseholdspermissionsput) | **PUT** /api/households/permissions | Set Member Permissions|
|[**updateHouseholdPreferencesApiHouseholdsPreferencesPut**](#updatehouseholdpreferencesapihouseholdspreferencesput) | **PUT** /api/households/preferences | Update Household Preferences|

# **getHouseholdMembersApiHouseholdsMembersGet**
> PaginationBaseUserOut getHouseholdMembersApiHouseholdsMembersGet()

Returns all users belonging to the current household

### Example

```typescript
import {
    HouseholdsSelfServiceApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsSelfServiceApi(configuration);

let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getHouseholdMembersApiHouseholdsMembersGet(
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

**PaginationBaseUserOut**

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

# **getHouseholdPreferencesApiHouseholdsPreferencesGet**
> ReadHouseholdPreferences getHouseholdPreferencesApiHouseholdsPreferencesGet()


### Example

```typescript
import {
    HouseholdsSelfServiceApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsSelfServiceApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getHouseholdPreferencesApiHouseholdsPreferencesGet(
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ReadHouseholdPreferences**

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

# **getHouseholdRecipeApiHouseholdsSelfRecipesRecipeSlugGet**
> HouseholdRecipeSummary getHouseholdRecipeApiHouseholdsSelfRecipesRecipeSlugGet()

Returns recipe data for the current household

### Example

```typescript
import {
    HouseholdsSelfServiceApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsSelfServiceApi(configuration);

let recipeSlug: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getHouseholdRecipeApiHouseholdsSelfRecipesRecipeSlugGet(
    recipeSlug,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **recipeSlug** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**HouseholdRecipeSummary**

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

# **getLoggedInUserHouseholdApiHouseholdsSelfGet**
> HouseholdInDB getLoggedInUserHouseholdApiHouseholdsSelfGet()

Returns the Household Data for the Current User

### Example

```typescript
import {
    HouseholdsSelfServiceApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsSelfServiceApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getLoggedInUserHouseholdApiHouseholdsSelfGet(
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**HouseholdInDB**

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

# **getStatisticsApiHouseholdsStatisticsGet**
> HouseholdStatistics getStatisticsApiHouseholdsStatisticsGet()


### Example

```typescript
import {
    HouseholdsSelfServiceApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsSelfServiceApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getStatisticsApiHouseholdsStatisticsGet(
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**HouseholdStatistics**

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

# **setMemberPermissionsApiHouseholdsPermissionsPut**
> UserOut setMemberPermissionsApiHouseholdsPermissionsPut(setPermissions)


### Example

```typescript
import {
    HouseholdsSelfServiceApi,
    Configuration,
    SetPermissions
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsSelfServiceApi(configuration);

let setPermissions: SetPermissions; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.setMemberPermissionsApiHouseholdsPermissionsPut(
    setPermissions,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **setPermissions** | **SetPermissions**|  | |
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

# **updateHouseholdPreferencesApiHouseholdsPreferencesPut**
> ReadHouseholdPreferences updateHouseholdPreferencesApiHouseholdsPreferencesPut(updateHouseholdPreferences)


### Example

```typescript
import {
    HouseholdsSelfServiceApi,
    Configuration,
    UpdateHouseholdPreferences
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsSelfServiceApi(configuration);

let updateHouseholdPreferences: UpdateHouseholdPreferences; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateHouseholdPreferencesApiHouseholdsPreferencesPut(
    updateHouseholdPreferences,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateHouseholdPreferences** | **UpdateHouseholdPreferences**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ReadHouseholdPreferences**

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

