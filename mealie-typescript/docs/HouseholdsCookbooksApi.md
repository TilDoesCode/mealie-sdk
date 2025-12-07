# HouseholdsCookbooksApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createOneApiHouseholdsCookbooksPost**](#createoneapihouseholdscookbookspost) | **POST** /api/households/cookbooks | Create One|
|[**deleteOneApiHouseholdsCookbooksItemIdDelete**](#deleteoneapihouseholdscookbooksitemiddelete) | **DELETE** /api/households/cookbooks/{item_id} | Delete One|
|[**getAllApiHouseholdsCookbooksGet**](#getallapihouseholdscookbooksget) | **GET** /api/households/cookbooks | Get All|
|[**getOneApiHouseholdsCookbooksItemIdGet**](#getoneapihouseholdscookbooksitemidget) | **GET** /api/households/cookbooks/{item_id} | Get One|
|[**updateManyApiHouseholdsCookbooksPut**](#updatemanyapihouseholdscookbooksput) | **PUT** /api/households/cookbooks | Update Many|
|[**updateOneApiHouseholdsCookbooksItemIdPut**](#updateoneapihouseholdscookbooksitemidput) | **PUT** /api/households/cookbooks/{item_id} | Update One|

# **createOneApiHouseholdsCookbooksPost**
> ReadCookBook createOneApiHouseholdsCookbooksPost(createCookBook)


### Example

```typescript
import {
    HouseholdsCookbooksApi,
    Configuration,
    CreateCookBook
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsCookbooksApi(configuration);

let createCookBook: CreateCookBook; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createOneApiHouseholdsCookbooksPost(
    createCookBook,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createCookBook** | **CreateCookBook**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ReadCookBook**

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

# **deleteOneApiHouseholdsCookbooksItemIdDelete**
> ReadCookBook deleteOneApiHouseholdsCookbooksItemIdDelete()


### Example

```typescript
import {
    HouseholdsCookbooksApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsCookbooksApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteOneApiHouseholdsCookbooksItemIdDelete(
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

**ReadCookBook**

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

# **getAllApiHouseholdsCookbooksGet**
> CookBookPagination getAllApiHouseholdsCookbooksGet()


### Example

```typescript
import {
    HouseholdsCookbooksApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsCookbooksApi(configuration);

let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiHouseholdsCookbooksGet(
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

**CookBookPagination**

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

# **getOneApiHouseholdsCookbooksItemIdGet**
> ReadCookBook getOneApiHouseholdsCookbooksItemIdGet()


### Example

```typescript
import {
    HouseholdsCookbooksApi,
    Configuration,
    ItemId
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsCookbooksApi(configuration);

let itemId: ItemId; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiHouseholdsCookbooksItemIdGet(
    itemId,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **itemId** | **ItemId** |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ReadCookBook**

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

# **updateManyApiHouseholdsCookbooksPut**
> Array<ReadCookBook> updateManyApiHouseholdsCookbooksPut(updateCookBook)


### Example

```typescript
import {
    HouseholdsCookbooksApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsCookbooksApi(configuration);

let updateCookBook: Array<UpdateCookBook>; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateManyApiHouseholdsCookbooksPut(
    updateCookBook,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateCookBook** | **Array<UpdateCookBook>**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Array<ReadCookBook>**

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

# **updateOneApiHouseholdsCookbooksItemIdPut**
> ReadCookBook updateOneApiHouseholdsCookbooksItemIdPut(createCookBook)


### Example

```typescript
import {
    HouseholdsCookbooksApi,
    Configuration,
    CreateCookBook
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsCookbooksApi(configuration);

let itemId: string; // (default to undefined)
let createCookBook: CreateCookBook; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateOneApiHouseholdsCookbooksItemIdPut(
    itemId,
    createCookBook,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createCookBook** | **CreateCookBook**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ReadCookBook**

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

