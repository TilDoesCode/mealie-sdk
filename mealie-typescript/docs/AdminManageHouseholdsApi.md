# AdminManageHouseholdsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createOneApiAdminHouseholdsPost**](#createoneapiadminhouseholdspost) | **POST** /api/admin/households | Create One|
|[**deleteOneApiAdminHouseholdsItemIdDelete**](#deleteoneapiadminhouseholdsitemiddelete) | **DELETE** /api/admin/households/{item_id} | Delete One|
|[**getAllApiAdminHouseholdsGet**](#getallapiadminhouseholdsget) | **GET** /api/admin/households | Get All|
|[**getOneApiAdminHouseholdsItemIdGet**](#getoneapiadminhouseholdsitemidget) | **GET** /api/admin/households/{item_id} | Get One|
|[**updateOneApiAdminHouseholdsItemIdPut**](#updateoneapiadminhouseholdsitemidput) | **PUT** /api/admin/households/{item_id} | Update One|

# **createOneApiAdminHouseholdsPost**
> HouseholdInDB createOneApiAdminHouseholdsPost(householdCreate)


### Example

```typescript
import {
    AdminManageHouseholdsApi,
    Configuration,
    HouseholdCreate
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminManageHouseholdsApi(configuration);

let householdCreate: HouseholdCreate; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createOneApiAdminHouseholdsPost(
    householdCreate,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **householdCreate** | **HouseholdCreate**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**HouseholdInDB**

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

# **deleteOneApiAdminHouseholdsItemIdDelete**
> HouseholdInDB deleteOneApiAdminHouseholdsItemIdDelete()


### Example

```typescript
import {
    AdminManageHouseholdsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminManageHouseholdsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteOneApiAdminHouseholdsItemIdDelete(
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

# **getAllApiAdminHouseholdsGet**
> HouseholdPagination getAllApiAdminHouseholdsGet()


### Example

```typescript
import {
    AdminManageHouseholdsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminManageHouseholdsApi(configuration);

let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiAdminHouseholdsGet(
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

**HouseholdPagination**

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

# **getOneApiAdminHouseholdsItemIdGet**
> HouseholdInDB getOneApiAdminHouseholdsItemIdGet()


### Example

```typescript
import {
    AdminManageHouseholdsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminManageHouseholdsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiAdminHouseholdsItemIdGet(
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

# **updateOneApiAdminHouseholdsItemIdPut**
> HouseholdInDB updateOneApiAdminHouseholdsItemIdPut(updateHouseholdAdmin)


### Example

```typescript
import {
    AdminManageHouseholdsApi,
    Configuration,
    UpdateHouseholdAdmin
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminManageHouseholdsApi(configuration);

let itemId: string; // (default to undefined)
let updateHouseholdAdmin: UpdateHouseholdAdmin; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateOneApiAdminHouseholdsItemIdPut(
    itemId,
    updateHouseholdAdmin,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateHouseholdAdmin** | **UpdateHouseholdAdmin**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**HouseholdInDB**

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

