# HouseholdsShoppingListsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**addRecipeIngredientsToListApiHouseholdsShoppingListsItemIdRecipePost**](#addrecipeingredientstolistapihouseholdsshoppinglistsitemidrecipepost) | **POST** /api/households/shopping/lists/{item_id}/recipe | Add Recipe Ingredients To List|
|[**addSingleRecipeIngredientsToListApiHouseholdsShoppingListsItemIdRecipeRecipeIdPost**](#addsinglerecipeingredientstolistapihouseholdsshoppinglistsitemidreciperecipeidpost) | **POST** /api/households/shopping/lists/{item_id}/recipe/{recipe_id} | Add Single Recipe Ingredients To List|
|[**createOneApiHouseholdsShoppingListsPost**](#createoneapihouseholdsshoppinglistspost) | **POST** /api/households/shopping/lists | Create One|
|[**deleteOneApiHouseholdsShoppingListsItemIdDelete**](#deleteoneapihouseholdsshoppinglistsitemiddelete) | **DELETE** /api/households/shopping/lists/{item_id} | Delete One|
|[**getAllApiHouseholdsShoppingListsGet**](#getallapihouseholdsshoppinglistsget) | **GET** /api/households/shopping/lists | Get All|
|[**getOneApiHouseholdsShoppingListsItemIdGet**](#getoneapihouseholdsshoppinglistsitemidget) | **GET** /api/households/shopping/lists/{item_id} | Get One|
|[**removeRecipeIngredientsFromListApiHouseholdsShoppingListsItemIdRecipeRecipeIdDeletePost**](#removerecipeingredientsfromlistapihouseholdsshoppinglistsitemidreciperecipeiddeletepost) | **POST** /api/households/shopping/lists/{item_id}/recipe/{recipe_id}/delete | Remove Recipe Ingredients From List|
|[**updateLabelSettingsApiHouseholdsShoppingListsItemIdLabelSettingsPut**](#updatelabelsettingsapihouseholdsshoppinglistsitemidlabelsettingsput) | **PUT** /api/households/shopping/lists/{item_id}/label-settings | Update Label Settings|
|[**updateOneApiHouseholdsShoppingListsItemIdPut**](#updateoneapihouseholdsshoppinglistsitemidput) | **PUT** /api/households/shopping/lists/{item_id} | Update One|

# **addRecipeIngredientsToListApiHouseholdsShoppingListsItemIdRecipePost**
> ShoppingListOut addRecipeIngredientsToListApiHouseholdsShoppingListsItemIdRecipePost(shoppingListAddRecipeParamsBulk)


### Example

```typescript
import {
    HouseholdsShoppingListsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsShoppingListsApi(configuration);

let itemId: string; // (default to undefined)
let shoppingListAddRecipeParamsBulk: Array<ShoppingListAddRecipeParamsBulk>; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.addRecipeIngredientsToListApiHouseholdsShoppingListsItemIdRecipePost(
    itemId,
    shoppingListAddRecipeParamsBulk,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **shoppingListAddRecipeParamsBulk** | **Array<ShoppingListAddRecipeParamsBulk>**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ShoppingListOut**

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

# **addSingleRecipeIngredientsToListApiHouseholdsShoppingListsItemIdRecipeRecipeIdPost**
> ShoppingListOut addSingleRecipeIngredientsToListApiHouseholdsShoppingListsItemIdRecipeRecipeIdPost()


### Example

```typescript
import {
    HouseholdsShoppingListsApi,
    Configuration,
    ShoppingListAddRecipeParams
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsShoppingListsApi(configuration);

let itemId: string; // (default to undefined)
let recipeId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)
let shoppingListAddRecipeParams: ShoppingListAddRecipeParams; // (optional)

const { status, data } = await apiInstance.addSingleRecipeIngredientsToListApiHouseholdsShoppingListsItemIdRecipeRecipeIdPost(
    itemId,
    recipeId,
    acceptLanguage,
    shoppingListAddRecipeParams
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **shoppingListAddRecipeParams** | **ShoppingListAddRecipeParams**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **recipeId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ShoppingListOut**

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

# **createOneApiHouseholdsShoppingListsPost**
> ShoppingListOut createOneApiHouseholdsShoppingListsPost(shoppingListCreate)


### Example

```typescript
import {
    HouseholdsShoppingListsApi,
    Configuration,
    ShoppingListCreate
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsShoppingListsApi(configuration);

let shoppingListCreate: ShoppingListCreate; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createOneApiHouseholdsShoppingListsPost(
    shoppingListCreate,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **shoppingListCreate** | **ShoppingListCreate**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ShoppingListOut**

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

# **deleteOneApiHouseholdsShoppingListsItemIdDelete**
> ShoppingListOut deleteOneApiHouseholdsShoppingListsItemIdDelete()


### Example

```typescript
import {
    HouseholdsShoppingListsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsShoppingListsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteOneApiHouseholdsShoppingListsItemIdDelete(
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

**ShoppingListOut**

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

# **getAllApiHouseholdsShoppingListsGet**
> ShoppingListPagination getAllApiHouseholdsShoppingListsGet()


### Example

```typescript
import {
    HouseholdsShoppingListsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsShoppingListsApi(configuration);

let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiHouseholdsShoppingListsGet(
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

**ShoppingListPagination**

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

# **getOneApiHouseholdsShoppingListsItemIdGet**
> ShoppingListOut getOneApiHouseholdsShoppingListsItemIdGet()


### Example

```typescript
import {
    HouseholdsShoppingListsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsShoppingListsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiHouseholdsShoppingListsItemIdGet(
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

**ShoppingListOut**

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

# **removeRecipeIngredientsFromListApiHouseholdsShoppingListsItemIdRecipeRecipeIdDeletePost**
> ShoppingListOut removeRecipeIngredientsFromListApiHouseholdsShoppingListsItemIdRecipeRecipeIdDeletePost()


### Example

```typescript
import {
    HouseholdsShoppingListsApi,
    Configuration,
    ShoppingListRemoveRecipeParams
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsShoppingListsApi(configuration);

let itemId: string; // (default to undefined)
let recipeId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)
let shoppingListRemoveRecipeParams: ShoppingListRemoveRecipeParams; // (optional)

const { status, data } = await apiInstance.removeRecipeIngredientsFromListApiHouseholdsShoppingListsItemIdRecipeRecipeIdDeletePost(
    itemId,
    recipeId,
    acceptLanguage,
    shoppingListRemoveRecipeParams
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **shoppingListRemoveRecipeParams** | **ShoppingListRemoveRecipeParams**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **recipeId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ShoppingListOut**

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

# **updateLabelSettingsApiHouseholdsShoppingListsItemIdLabelSettingsPut**
> ShoppingListOut updateLabelSettingsApiHouseholdsShoppingListsItemIdLabelSettingsPut(shoppingListMultiPurposeLabelUpdate)


### Example

```typescript
import {
    HouseholdsShoppingListsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsShoppingListsApi(configuration);

let itemId: string; // (default to undefined)
let shoppingListMultiPurposeLabelUpdate: Array<ShoppingListMultiPurposeLabelUpdate>; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateLabelSettingsApiHouseholdsShoppingListsItemIdLabelSettingsPut(
    itemId,
    shoppingListMultiPurposeLabelUpdate,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **shoppingListMultiPurposeLabelUpdate** | **Array<ShoppingListMultiPurposeLabelUpdate>**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ShoppingListOut**

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

# **updateOneApiHouseholdsShoppingListsItemIdPut**
> ShoppingListOut updateOneApiHouseholdsShoppingListsItemIdPut(shoppingListUpdate)


### Example

```typescript
import {
    HouseholdsShoppingListsApi,
    Configuration,
    ShoppingListUpdate
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsShoppingListsApi(configuration);

let itemId: string; // (default to undefined)
let shoppingListUpdate: ShoppingListUpdate; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateOneApiHouseholdsShoppingListsItemIdPut(
    itemId,
    shoppingListUpdate,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **shoppingListUpdate** | **ShoppingListUpdate**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ShoppingListOut**

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

