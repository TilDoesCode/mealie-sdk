# GroupsMultiPurposeLabelsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createOneApiGroupsLabelsPost**](#createoneapigroupslabelspost) | **POST** /api/groups/labels | Create One|
|[**deleteOneApiGroupsLabelsItemIdDelete**](#deleteoneapigroupslabelsitemiddelete) | **DELETE** /api/groups/labels/{item_id} | Delete One|
|[**getAllApiGroupsLabelsGet**](#getallapigroupslabelsget) | **GET** /api/groups/labels | Get All|
|[**getOneApiGroupsLabelsItemIdGet**](#getoneapigroupslabelsitemidget) | **GET** /api/groups/labels/{item_id} | Get One|
|[**updateOneApiGroupsLabelsItemIdPut**](#updateoneapigroupslabelsitemidput) | **PUT** /api/groups/labels/{item_id} | Update One|

# **createOneApiGroupsLabelsPost**
> MultiPurposeLabelOut createOneApiGroupsLabelsPost(multiPurposeLabelCreate)


### Example

```typescript
import {
    GroupsMultiPurposeLabelsApi,
    Configuration,
    MultiPurposeLabelCreate
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new GroupsMultiPurposeLabelsApi(configuration);

let multiPurposeLabelCreate: MultiPurposeLabelCreate; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createOneApiGroupsLabelsPost(
    multiPurposeLabelCreate,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **multiPurposeLabelCreate** | **MultiPurposeLabelCreate**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**MultiPurposeLabelOut**

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

# **deleteOneApiGroupsLabelsItemIdDelete**
> MultiPurposeLabelOut deleteOneApiGroupsLabelsItemIdDelete()


### Example

```typescript
import {
    GroupsMultiPurposeLabelsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new GroupsMultiPurposeLabelsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteOneApiGroupsLabelsItemIdDelete(
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

**MultiPurposeLabelOut**

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

# **getAllApiGroupsLabelsGet**
> MultiPurposeLabelPagination getAllApiGroupsLabelsGet()


### Example

```typescript
import {
    GroupsMultiPurposeLabelsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new GroupsMultiPurposeLabelsApi(configuration);

let search: string; // (optional) (default to undefined)
let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiGroupsLabelsGet(
    search,
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
| **search** | [**string**] |  | (optional) defaults to undefined|
| **orderBy** | [**string**] |  | (optional) defaults to undefined|
| **orderByNullPosition** | **OrderByNullPosition** |  | (optional) defaults to undefined|
| **orderDirection** | **OrderDirection** |  | (optional) defaults to undefined|
| **queryFilter** | [**string**] |  | (optional) defaults to undefined|
| **paginationSeed** | [**string**] |  | (optional) defaults to undefined|
| **page** | [**number**] |  | (optional) defaults to 1|
| **perPage** | [**number**] |  | (optional) defaults to 50|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**MultiPurposeLabelPagination**

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

# **getOneApiGroupsLabelsItemIdGet**
> MultiPurposeLabelOut getOneApiGroupsLabelsItemIdGet()


### Example

```typescript
import {
    GroupsMultiPurposeLabelsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new GroupsMultiPurposeLabelsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiGroupsLabelsItemIdGet(
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

**MultiPurposeLabelOut**

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

# **updateOneApiGroupsLabelsItemIdPut**
> MultiPurposeLabelOut updateOneApiGroupsLabelsItemIdPut(multiPurposeLabelUpdate)


### Example

```typescript
import {
    GroupsMultiPurposeLabelsApi,
    Configuration,
    MultiPurposeLabelUpdate
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new GroupsMultiPurposeLabelsApi(configuration);

let itemId: string; // (default to undefined)
let multiPurposeLabelUpdate: MultiPurposeLabelUpdate; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateOneApiGroupsLabelsItemIdPut(
    itemId,
    multiPurposeLabelUpdate,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **multiPurposeLabelUpdate** | **MultiPurposeLabelUpdate**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**MultiPurposeLabelOut**

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

