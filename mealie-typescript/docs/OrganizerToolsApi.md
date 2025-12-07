# OrganizerToolsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createOneApiOrganizersToolsPost**](#createoneapiorganizerstoolspost) | **POST** /api/organizers/tools | Create One|
|[**deleteOneApiOrganizersToolsItemIdDelete**](#deleteoneapiorganizerstoolsitemiddelete) | **DELETE** /api/organizers/tools/{item_id} | Delete One|
|[**getAllApiOrganizersToolsGet**](#getallapiorganizerstoolsget) | **GET** /api/organizers/tools | Get All|
|[**getOneApiOrganizersToolsItemIdGet**](#getoneapiorganizerstoolsitemidget) | **GET** /api/organizers/tools/{item_id} | Get One|
|[**getOneBySlugApiOrganizersToolsSlugToolSlugGet**](#getonebyslugapiorganizerstoolsslugtoolslugget) | **GET** /api/organizers/tools/slug/{tool_slug} | Get One By Slug|
|[**updateOneApiOrganizersToolsItemIdPut**](#updateoneapiorganizerstoolsitemidput) | **PUT** /api/organizers/tools/{item_id} | Update One|

# **createOneApiOrganizersToolsPost**
> RecipeTool createOneApiOrganizersToolsPost(recipeToolCreate)


### Example

```typescript
import {
    OrganizerToolsApi,
    Configuration,
    RecipeToolCreate
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerToolsApi(configuration);

let recipeToolCreate: RecipeToolCreate; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createOneApiOrganizersToolsPost(
    recipeToolCreate,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **recipeToolCreate** | **RecipeToolCreate**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**RecipeTool**

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

# **deleteOneApiOrganizersToolsItemIdDelete**
> RecipeTool deleteOneApiOrganizersToolsItemIdDelete()


### Example

```typescript
import {
    OrganizerToolsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerToolsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteOneApiOrganizersToolsItemIdDelete(
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

**RecipeTool**

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

# **getAllApiOrganizersToolsGet**
> RecipeToolPagination getAllApiOrganizersToolsGet()


### Example

```typescript
import {
    OrganizerToolsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerToolsApi(configuration);

let search: string; // (optional) (default to undefined)
let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiOrganizersToolsGet(
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

**RecipeToolPagination**

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

# **getOneApiOrganizersToolsItemIdGet**
> RecipeTool getOneApiOrganizersToolsItemIdGet()


### Example

```typescript
import {
    OrganizerToolsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerToolsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiOrganizersToolsItemIdGet(
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

**RecipeTool**

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

# **getOneBySlugApiOrganizersToolsSlugToolSlugGet**
> RecipeToolResponse getOneBySlugApiOrganizersToolsSlugToolSlugGet()


### Example

```typescript
import {
    OrganizerToolsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerToolsApi(configuration);

let toolSlug: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneBySlugApiOrganizersToolsSlugToolSlugGet(
    toolSlug,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **toolSlug** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**RecipeToolResponse**

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

# **updateOneApiOrganizersToolsItemIdPut**
> RecipeTool updateOneApiOrganizersToolsItemIdPut(recipeToolCreate)


### Example

```typescript
import {
    OrganizerToolsApi,
    Configuration,
    RecipeToolCreate
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerToolsApi(configuration);

let itemId: string; // (default to undefined)
let recipeToolCreate: RecipeToolCreate; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateOneApiOrganizersToolsItemIdPut(
    itemId,
    recipeToolCreate,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **recipeToolCreate** | **RecipeToolCreate**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**RecipeTool**

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

