# HouseholdsWebhooksApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createOneApiHouseholdsWebhooksPost**](#createoneapihouseholdswebhookspost) | **POST** /api/households/webhooks | Create One|
|[**deleteOneApiHouseholdsWebhooksItemIdDelete**](#deleteoneapihouseholdswebhooksitemiddelete) | **DELETE** /api/households/webhooks/{item_id} | Delete One|
|[**getAllApiHouseholdsWebhooksGet**](#getallapihouseholdswebhooksget) | **GET** /api/households/webhooks | Get All|
|[**getOneApiHouseholdsWebhooksItemIdGet**](#getoneapihouseholdswebhooksitemidget) | **GET** /api/households/webhooks/{item_id} | Get One|
|[**rerunWebhooksApiHouseholdsWebhooksRerunPost**](#rerunwebhooksapihouseholdswebhooksrerunpost) | **POST** /api/households/webhooks/rerun | Rerun Webhooks|
|[**testOneApiHouseholdsWebhooksItemIdTestPost**](#testoneapihouseholdswebhooksitemidtestpost) | **POST** /api/households/webhooks/{item_id}/test | Test One|
|[**updateOneApiHouseholdsWebhooksItemIdPut**](#updateoneapihouseholdswebhooksitemidput) | **PUT** /api/households/webhooks/{item_id} | Update One|

# **createOneApiHouseholdsWebhooksPost**
> ReadWebhook createOneApiHouseholdsWebhooksPost(createWebhook)


### Example

```typescript
import {
    HouseholdsWebhooksApi,
    Configuration,
    CreateWebhook
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsWebhooksApi(configuration);

let createWebhook: CreateWebhook; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createOneApiHouseholdsWebhooksPost(
    createWebhook,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createWebhook** | **CreateWebhook**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ReadWebhook**

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

# **deleteOneApiHouseholdsWebhooksItemIdDelete**
> ReadWebhook deleteOneApiHouseholdsWebhooksItemIdDelete()


### Example

```typescript
import {
    HouseholdsWebhooksApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsWebhooksApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteOneApiHouseholdsWebhooksItemIdDelete(
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

**ReadWebhook**

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

# **getAllApiHouseholdsWebhooksGet**
> WebhookPagination getAllApiHouseholdsWebhooksGet()


### Example

```typescript
import {
    HouseholdsWebhooksApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsWebhooksApi(configuration);

let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiHouseholdsWebhooksGet(
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

**WebhookPagination**

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

# **getOneApiHouseholdsWebhooksItemIdGet**
> ReadWebhook getOneApiHouseholdsWebhooksItemIdGet()


### Example

```typescript
import {
    HouseholdsWebhooksApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsWebhooksApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiHouseholdsWebhooksItemIdGet(
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

**ReadWebhook**

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

# **rerunWebhooksApiHouseholdsWebhooksRerunPost**
> any rerunWebhooksApiHouseholdsWebhooksRerunPost()

Manually re-fires all previously scheduled webhooks for today

### Example

```typescript
import {
    HouseholdsWebhooksApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsWebhooksApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.rerunWebhooksApiHouseholdsWebhooksRerunPost(
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

# **testOneApiHouseholdsWebhooksItemIdTestPost**
> any testOneApiHouseholdsWebhooksItemIdTestPost()


### Example

```typescript
import {
    HouseholdsWebhooksApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsWebhooksApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.testOneApiHouseholdsWebhooksItemIdTestPost(
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

# **updateOneApiHouseholdsWebhooksItemIdPut**
> ReadWebhook updateOneApiHouseholdsWebhooksItemIdPut(createWebhook)


### Example

```typescript
import {
    HouseholdsWebhooksApi,
    Configuration,
    CreateWebhook
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsWebhooksApi(configuration);

let itemId: string; // (default to undefined)
let createWebhook: CreateWebhook; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateOneApiHouseholdsWebhooksItemIdPut(
    itemId,
    createWebhook,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createWebhook** | **CreateWebhook**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ReadWebhook**

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

