# HouseholdsShoppingListItemsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createManyApiHouseholdsShoppingItemsCreateBulkPost**](#createmanyapihouseholdsshoppingitemscreatebulkpost) | **POST** /api/households/shopping/items/create-bulk | Create Many|
|[**createOneApiHouseholdsShoppingItemsPost**](#createoneapihouseholdsshoppingitemspost) | **POST** /api/households/shopping/items | Create One|
|[**deleteManyApiHouseholdsShoppingItemsDelete**](#deletemanyapihouseholdsshoppingitemsdelete) | **DELETE** /api/households/shopping/items | Delete Many|
|[**deleteOneApiHouseholdsShoppingItemsItemIdDelete**](#deleteoneapihouseholdsshoppingitemsitemiddelete) | **DELETE** /api/households/shopping/items/{item_id} | Delete One|
|[**getAllApiHouseholdsShoppingItemsGet**](#getallapihouseholdsshoppingitemsget) | **GET** /api/households/shopping/items | Get All|
|[**getOneApiHouseholdsShoppingItemsItemIdGet**](#getoneapihouseholdsshoppingitemsitemidget) | **GET** /api/households/shopping/items/{item_id} | Get One|
|[**updateManyApiHouseholdsShoppingItemsPut**](#updatemanyapihouseholdsshoppingitemsput) | **PUT** /api/households/shopping/items | Update Many|
|[**updateOneApiHouseholdsShoppingItemsItemIdPut**](#updateoneapihouseholdsshoppingitemsitemidput) | **PUT** /api/households/shopping/items/{item_id} | Update One|

# **createManyApiHouseholdsShoppingItemsCreateBulkPost**
> ShoppingListItemsCollectionOut createManyApiHouseholdsShoppingItemsCreateBulkPost(shoppingListItemCreate)


### Example

```typescript
import {
    HouseholdsShoppingListItemsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsShoppingListItemsApi(configuration);

let shoppingListItemCreate: Array<ShoppingListItemCreate>; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createManyApiHouseholdsShoppingItemsCreateBulkPost(
    shoppingListItemCreate,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **shoppingListItemCreate** | **Array<ShoppingListItemCreate>**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ShoppingListItemsCollectionOut**

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

# **createOneApiHouseholdsShoppingItemsPost**
> ShoppingListItemsCollectionOut createOneApiHouseholdsShoppingItemsPost(shoppingListItemCreate)


### Example

```typescript
import {
    HouseholdsShoppingListItemsApi,
    Configuration,
    ShoppingListItemCreate
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsShoppingListItemsApi(configuration);

let shoppingListItemCreate: ShoppingListItemCreate; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createOneApiHouseholdsShoppingItemsPost(
    shoppingListItemCreate,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **shoppingListItemCreate** | **ShoppingListItemCreate**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ShoppingListItemsCollectionOut**

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

# **deleteManyApiHouseholdsShoppingItemsDelete**
> SuccessResponse deleteManyApiHouseholdsShoppingItemsDelete()


### Example

```typescript
import {
    HouseholdsShoppingListItemsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsShoppingListItemsApi(configuration);

let ids: Array<string>; // (optional) (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteManyApiHouseholdsShoppingItemsDelete(
    ids,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **ids** | **Array&lt;string&gt;** |  | (optional) defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**SuccessResponse**

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

# **deleteOneApiHouseholdsShoppingItemsItemIdDelete**
> SuccessResponse deleteOneApiHouseholdsShoppingItemsItemIdDelete()


### Example

```typescript
import {
    HouseholdsShoppingListItemsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsShoppingListItemsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteOneApiHouseholdsShoppingItemsItemIdDelete(
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

**SuccessResponse**

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

# **getAllApiHouseholdsShoppingItemsGet**
> ShoppingListItemPagination getAllApiHouseholdsShoppingItemsGet()


### Example

```typescript
import {
    HouseholdsShoppingListItemsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsShoppingListItemsApi(configuration);

let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiHouseholdsShoppingItemsGet(
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

**ShoppingListItemPagination**

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

# **getOneApiHouseholdsShoppingItemsItemIdGet**
> ShoppingListItemOutOutput getOneApiHouseholdsShoppingItemsItemIdGet()


### Example

```typescript
import {
    HouseholdsShoppingListItemsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsShoppingListItemsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiHouseholdsShoppingItemsItemIdGet(
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

**ShoppingListItemOutOutput**

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

# **updateManyApiHouseholdsShoppingItemsPut**
> ShoppingListItemsCollectionOut updateManyApiHouseholdsShoppingItemsPut(shoppingListItemUpdateBulk)


### Example

```typescript
import {
    HouseholdsShoppingListItemsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsShoppingListItemsApi(configuration);

let shoppingListItemUpdateBulk: Array<ShoppingListItemUpdateBulk>; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateManyApiHouseholdsShoppingItemsPut(
    shoppingListItemUpdateBulk,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **shoppingListItemUpdateBulk** | **Array<ShoppingListItemUpdateBulk>**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ShoppingListItemsCollectionOut**

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

# **updateOneApiHouseholdsShoppingItemsItemIdPut**
> ShoppingListItemsCollectionOut updateOneApiHouseholdsShoppingItemsItemIdPut(shoppingListItemUpdate)


### Example

```typescript
import {
    HouseholdsShoppingListItemsApi,
    Configuration,
    ShoppingListItemUpdate
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsShoppingListItemsApi(configuration);

let itemId: string; // (default to undefined)
let shoppingListItemUpdate: ShoppingListItemUpdate; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateOneApiHouseholdsShoppingItemsItemIdPut(
    itemId,
    shoppingListItemUpdate,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **shoppingListItemUpdate** | **ShoppingListItemUpdate**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ShoppingListItemsCollectionOut**

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

