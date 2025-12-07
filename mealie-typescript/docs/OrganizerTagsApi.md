# OrganizerTagsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createOneApiOrganizersTagsPost**](#createoneapiorganizerstagspost) | **POST** /api/organizers/tags | Create One|
|[**deleteRecipeTagApiOrganizersTagsItemIdDelete**](#deleterecipetagapiorganizerstagsitemiddelete) | **DELETE** /api/organizers/tags/{item_id} | Delete Recipe Tag|
|[**getAllApiOrganizersTagsGet**](#getallapiorganizerstagsget) | **GET** /api/organizers/tags | Get All|
|[**getEmptyTagsApiOrganizersTagsEmptyGet**](#getemptytagsapiorganizerstagsemptyget) | **GET** /api/organizers/tags/empty | Get Empty Tags|
|[**getOneApiOrganizersTagsItemIdGet**](#getoneapiorganizerstagsitemidget) | **GET** /api/organizers/tags/{item_id} | Get One|
|[**getOneBySlugApiOrganizersTagsSlugTagSlugGet**](#getonebyslugapiorganizerstagsslugtagslugget) | **GET** /api/organizers/tags/slug/{tag_slug} | Get One By Slug|
|[**updateOneApiOrganizersTagsItemIdPut**](#updateoneapiorganizerstagsitemidput) | **PUT** /api/organizers/tags/{item_id} | Update One|

# **createOneApiOrganizersTagsPost**
> any createOneApiOrganizersTagsPost(tagIn)

Creates a Tag in the database

### Example

```typescript
import {
    OrganizerTagsApi,
    Configuration,
    TagIn
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerTagsApi(configuration);

let tagIn: TagIn; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createOneApiOrganizersTagsPost(
    tagIn,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tagIn** | **TagIn**|  | |
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

# **deleteRecipeTagApiOrganizersTagsItemIdDelete**
> any deleteRecipeTagApiOrganizersTagsItemIdDelete()

Removes a recipe tag from the database. Deleting a tag does not impact a recipe. The tag will be removed from any recipes that contain it

### Example

```typescript
import {
    OrganizerTagsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerTagsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteRecipeTagApiOrganizersTagsItemIdDelete(
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

# **getAllApiOrganizersTagsGet**
> RecipeTagPagination getAllApiOrganizersTagsGet()

Returns a list of available tags in the database

### Example

```typescript
import {
    OrganizerTagsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerTagsApi(configuration);

let search: string; // (optional) (default to undefined)
let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiOrganizersTagsGet(
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

**RecipeTagPagination**

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

# **getEmptyTagsApiOrganizersTagsEmptyGet**
> any getEmptyTagsApiOrganizersTagsEmptyGet()

Returns a list of tags that do not contain any recipes

### Example

```typescript
import {
    OrganizerTagsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerTagsApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getEmptyTagsApiOrganizersTagsEmptyGet(
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

# **getOneApiOrganizersTagsItemIdGet**
> RecipeTagResponse getOneApiOrganizersTagsItemIdGet()

Returns a list of recipes associated with the provided tag.

### Example

```typescript
import {
    OrganizerTagsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerTagsApi(configuration);

let itemId: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiOrganizersTagsItemIdGet(
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

**RecipeTagResponse**

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

# **getOneBySlugApiOrganizersTagsSlugTagSlugGet**
> RecipeTagResponse getOneBySlugApiOrganizersTagsSlugTagSlugGet()


### Example

```typescript
import {
    OrganizerTagsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerTagsApi(configuration);

let tagSlug: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneBySlugApiOrganizersTagsSlugTagSlugGet(
    tagSlug,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tagSlug** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**RecipeTagResponse**

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

# **updateOneApiOrganizersTagsItemIdPut**
> RecipeTagResponse updateOneApiOrganizersTagsItemIdPut(tagIn)

Updates an existing Tag in the database

### Example

```typescript
import {
    OrganizerTagsApi,
    Configuration,
    TagIn
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new OrganizerTagsApi(configuration);

let itemId: string; // (default to undefined)
let tagIn: TagIn; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateOneApiOrganizersTagsItemIdPut(
    itemId,
    tagIn,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tagIn** | **TagIn**|  | |
| **itemId** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**RecipeTagResponse**

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

