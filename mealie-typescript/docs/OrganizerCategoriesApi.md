# OrganizerCategoriesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createOneApiOrganizersCategoriesPost**](#createoneapiorganizerscategoriespost) | **POST** /api/organizers/categories | Create One|
|[**deleteOneApiOrganizersCategoriesItemIdDelete**](#deleteoneapiorganizerscategoriesitemiddelete) | **DELETE** /api/organizers/categories/{item_id} | Delete One|
|[**getAllApiOrganizersCategoriesGet**](#getallapiorganizerscategoriesget) | **GET** /api/organizers/categories | Get All|
|[**getAllEmptyApiOrganizersCategoriesEmptyGet**](#getallemptyapiorganizerscategoriesemptyget) | **GET** /api/organizers/categories/empty | Get All Empty|
|[**getOneApiOrganizersCategoriesItemIdGet**](#getoneapiorganizerscategoriesitemidget) | **GET** /api/organizers/categories/{item_id} | Get One|
|[**getOneBySlugApiOrganizersCategoriesSlugCategorySlugGet**](#getonebyslugapiorganizerscategoriesslugcategoryslugget) | **GET** /api/organizers/categories/slug/{category_slug} | Get One By Slug|
|[**updateOneApiOrganizersCategoriesItemIdPut**](#updateoneapiorganizerscategoriesitemidput) | **PUT** /api/organizers/categories/{item_id} | Update One|

# **createOneApiOrganizersCategoriesPost**
> any createOneApiOrganizersCategoriesPost(categoryIn)

Creates a Category in the database

### Example

```typescript
import {
    OrganizerCategoriesApi,
    Configuration,
    CategoryIn
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerCategoriesApi(configuration);

let categoryIn: CategoryIn; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createOneApiOrganizersCategoriesPost(
    categoryIn,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **categoryIn** | **CategoryIn**|  | |
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
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteOneApiOrganizersCategoriesItemIdDelete**
> any deleteOneApiOrganizersCategoriesItemIdDelete()

Removes a recipe category from the database. Deleting a category does not impact a recipe. The category will be removed from any recipes that contain it

### Example

```typescript
import {
    OrganizerCategoriesApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerCategoriesApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteOneApiOrganizersCategoriesItemIdDelete(
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

# **getAllApiOrganizersCategoriesGet**
> RecipeCategoryPagination getAllApiOrganizersCategoriesGet()

Returns a list of available categories in the database

### Example

```typescript
import {
    OrganizerCategoriesApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerCategoriesApi(configuration);

let search: string; // (optional) (default to undefined)
let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiOrganizersCategoriesGet(
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

**RecipeCategoryPagination**

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

# **getAllEmptyApiOrganizersCategoriesEmptyGet**
> Array<CategoryBase> getAllEmptyApiOrganizersCategoriesEmptyGet()

Returns a list of categories that do not contain any recipes

### Example

```typescript
import {
    OrganizerCategoriesApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerCategoriesApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllEmptyApiOrganizersCategoriesEmptyGet(
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Array<CategoryBase>**

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

# **getOneApiOrganizersCategoriesItemIdGet**
> CategorySummary getOneApiOrganizersCategoriesItemIdGet()

Returns a list of recipes associated with the provided category.

### Example

```typescript
import {
    OrganizerCategoriesApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerCategoriesApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiOrganizersCategoriesItemIdGet(
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

**CategorySummary**

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

# **getOneBySlugApiOrganizersCategoriesSlugCategorySlugGet**
> any getOneBySlugApiOrganizersCategoriesSlugCategorySlugGet()

Returns a category object with the associated recieps relating to the category

### Example

```typescript
import {
    OrganizerCategoriesApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerCategoriesApi(configuration);

let categorySlug: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneBySlugApiOrganizersCategoriesSlugCategorySlugGet(
    categorySlug,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **categorySlug** | [**string**] |  | defaults to undefined|
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

# **updateOneApiOrganizersCategoriesItemIdPut**
> CategorySummary updateOneApiOrganizersCategoriesItemIdPut(categoryIn)

Updates an existing Tag in the database

### Example

```typescript
import {
    OrganizerCategoriesApi,
    Configuration,
    CategoryIn
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerCategoriesApi(configuration);

let itemId: string; // (default to undefined)
let categoryIn: CategoryIn; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateOneApiOrganizersCategoriesItemIdPut(
    itemId,
    categoryIn,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **categoryIn** | **CategoryIn**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**CategorySummary**

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

