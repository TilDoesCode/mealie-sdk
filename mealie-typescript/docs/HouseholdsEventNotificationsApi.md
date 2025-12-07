# HouseholdsEventNotificationsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createOneApiHouseholdsEventsNotificationsPost**](#createoneapihouseholdseventsnotificationspost) | **POST** /api/households/events/notifications | Create One|
|[**deleteOneApiHouseholdsEventsNotificationsItemIdDelete**](#deleteoneapihouseholdseventsnotificationsitemiddelete) | **DELETE** /api/households/events/notifications/{item_id} | Delete One|
|[**getAllApiHouseholdsEventsNotificationsGet**](#getallapihouseholdseventsnotificationsget) | **GET** /api/households/events/notifications | Get All|
|[**getOneApiHouseholdsEventsNotificationsItemIdGet**](#getoneapihouseholdseventsnotificationsitemidget) | **GET** /api/households/events/notifications/{item_id} | Get One|
|[**testNotificationApiHouseholdsEventsNotificationsItemIdTestPost**](#testnotificationapihouseholdseventsnotificationsitemidtestpost) | **POST** /api/households/events/notifications/{item_id}/test | Test Notification|
|[**updateOneApiHouseholdsEventsNotificationsItemIdPut**](#updateoneapihouseholdseventsnotificationsitemidput) | **PUT** /api/households/events/notifications/{item_id} | Update One|

# **createOneApiHouseholdsEventsNotificationsPost**
> GroupEventNotifierOut createOneApiHouseholdsEventsNotificationsPost(groupEventNotifierCreate)


### Example

```typescript
import {
    HouseholdsEventNotificationsApi,
    Configuration,
    GroupEventNotifierCreate
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsEventNotificationsApi(configuration);

let groupEventNotifierCreate: GroupEventNotifierCreate; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createOneApiHouseholdsEventsNotificationsPost(
    groupEventNotifierCreate,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **groupEventNotifierCreate** | **GroupEventNotifierCreate**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**GroupEventNotifierOut**

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

# **deleteOneApiHouseholdsEventsNotificationsItemIdDelete**
> deleteOneApiHouseholdsEventsNotificationsItemIdDelete()


### Example

```typescript
import {
    HouseholdsEventNotificationsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsEventNotificationsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteOneApiHouseholdsEventsNotificationsItemIdDelete(
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

void (empty response body)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAllApiHouseholdsEventsNotificationsGet**
> GroupEventPagination getAllApiHouseholdsEventsNotificationsGet()


### Example

```typescript
import {
    HouseholdsEventNotificationsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsEventNotificationsApi(configuration);

let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiHouseholdsEventsNotificationsGet(
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

**GroupEventPagination**

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

# **getOneApiHouseholdsEventsNotificationsItemIdGet**
> GroupEventNotifierOut getOneApiHouseholdsEventsNotificationsItemIdGet()


### Example

```typescript
import {
    HouseholdsEventNotificationsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsEventNotificationsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiHouseholdsEventsNotificationsItemIdGet(
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

**GroupEventNotifierOut**

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

# **testNotificationApiHouseholdsEventsNotificationsItemIdTestPost**
> testNotificationApiHouseholdsEventsNotificationsItemIdTestPost()


### Example

```typescript
import {
    HouseholdsEventNotificationsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsEventNotificationsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.testNotificationApiHouseholdsEventsNotificationsItemIdTestPost(
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

void (empty response body)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateOneApiHouseholdsEventsNotificationsItemIdPut**
> GroupEventNotifierOut updateOneApiHouseholdsEventsNotificationsItemIdPut(groupEventNotifierUpdate)


### Example

```typescript
import {
    HouseholdsEventNotificationsApi,
    Configuration,
    GroupEventNotifierUpdate
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsEventNotificationsApi(configuration);

let itemId: string; // (default to undefined)
let groupEventNotifierUpdate: GroupEventNotifierUpdate; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateOneApiHouseholdsEventsNotificationsItemIdPut(
    itemId,
    groupEventNotifierUpdate,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **groupEventNotifierUpdate** | **GroupEventNotifierUpdate**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**GroupEventNotifierOut**

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

