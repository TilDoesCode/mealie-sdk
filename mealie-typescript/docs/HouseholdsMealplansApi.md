# HouseholdsMealplansApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createOneApiHouseholdsMealplansPost**](#createoneapihouseholdsmealplanspost) | **POST** /api/households/mealplans | Create One|
|[**createRandomMealApiHouseholdsMealplansRandomPost**](#createrandommealapihouseholdsmealplansrandompost) | **POST** /api/households/mealplans/random | Create Random Meal|
|[**deleteOneApiHouseholdsMealplansItemIdDelete**](#deleteoneapihouseholdsmealplansitemiddelete) | **DELETE** /api/households/mealplans/{item_id} | Delete One|
|[**getAllApiHouseholdsMealplansGet**](#getallapihouseholdsmealplansget) | **GET** /api/households/mealplans | Get All|
|[**getOneApiHouseholdsMealplansItemIdGet**](#getoneapihouseholdsmealplansitemidget) | **GET** /api/households/mealplans/{item_id} | Get One|
|[**getTodaysMealsApiHouseholdsMealplansTodayGet**](#gettodaysmealsapihouseholdsmealplanstodayget) | **GET** /api/households/mealplans/today | Get Todays Meals|
|[**updateOneApiHouseholdsMealplansItemIdPut**](#updateoneapihouseholdsmealplansitemidput) | **PUT** /api/households/mealplans/{item_id} | Update One|

# **createOneApiHouseholdsMealplansPost**
> ReadPlanEntry createOneApiHouseholdsMealplansPost(createPlanEntry)


### Example

```typescript
import {
    HouseholdsMealplansApi,
    Configuration,
    CreatePlanEntry
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsMealplansApi(configuration);

let createPlanEntry: CreatePlanEntry; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createOneApiHouseholdsMealplansPost(
    createPlanEntry,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createPlanEntry** | **CreatePlanEntry**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ReadPlanEntry**

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

# **createRandomMealApiHouseholdsMealplansRandomPost**
> ReadPlanEntry createRandomMealApiHouseholdsMealplansRandomPost(createRandomEntry)

`create_random_meal` is a route that provides the randomized functionality for mealplaners. It operates by following the rules set out in the household\'s mealplan settings. If no settings are set, it will return any random meal.  Refer to the mealplan settings routes for more information on how rules can be applied to the random meal selector.

### Example

```typescript
import {
    HouseholdsMealplansApi,
    Configuration,
    CreateRandomEntry
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsMealplansApi(configuration);

let createRandomEntry: CreateRandomEntry; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createRandomMealApiHouseholdsMealplansRandomPost(
    createRandomEntry,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createRandomEntry** | **CreateRandomEntry**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ReadPlanEntry**

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

# **deleteOneApiHouseholdsMealplansItemIdDelete**
> ReadPlanEntry deleteOneApiHouseholdsMealplansItemIdDelete()


### Example

```typescript
import {
    HouseholdsMealplansApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsMealplansApi(configuration);

let itemId: number; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteOneApiHouseholdsMealplansItemIdDelete(
    itemId,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **itemId** | [**number**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ReadPlanEntry**

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

# **getAllApiHouseholdsMealplansGet**
> PlanEntryPagination getAllApiHouseholdsMealplansGet()


### Example

```typescript
import {
    HouseholdsMealplansApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsMealplansApi(configuration);

let startDate: string; // (optional) (default to undefined)
let endDate: string; // (optional) (default to undefined)
let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiHouseholdsMealplansGet(
    startDate,
    endDate,
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
| **startDate** | [**string**] |  | (optional) defaults to undefined|
| **endDate** | [**string**] |  | (optional) defaults to undefined|
| **orderBy** | [**string**] |  | (optional) defaults to undefined|
| **orderByNullPosition** | **OrderByNullPosition** |  | (optional) defaults to undefined|
| **orderDirection** | **OrderDirection** |  | (optional) defaults to undefined|
| **queryFilter** | [**string**] |  | (optional) defaults to undefined|
| **paginationSeed** | [**string**] |  | (optional) defaults to undefined|
| **page** | [**number**] |  | (optional) defaults to 1|
| **perPage** | [**number**] |  | (optional) defaults to 50|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**PlanEntryPagination**

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

# **getOneApiHouseholdsMealplansItemIdGet**
> ReadPlanEntry getOneApiHouseholdsMealplansItemIdGet()


### Example

```typescript
import {
    HouseholdsMealplansApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsMealplansApi(configuration);

let itemId: number; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiHouseholdsMealplansItemIdGet(
    itemId,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **itemId** | [**number**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ReadPlanEntry**

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

# **getTodaysMealsApiHouseholdsMealplansTodayGet**
> any getTodaysMealsApiHouseholdsMealplansTodayGet()


### Example

```typescript
import {
    HouseholdsMealplansApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsMealplansApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getTodaysMealsApiHouseholdsMealplansTodayGet(
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

# **updateOneApiHouseholdsMealplansItemIdPut**
> ReadPlanEntry updateOneApiHouseholdsMealplansItemIdPut(updatePlanEntry)


### Example

```typescript
import {
    HouseholdsMealplansApi,
    Configuration,
    UpdatePlanEntry
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsMealplansApi(configuration);

let itemId: number; // (default to undefined)
let updatePlanEntry: UpdatePlanEntry; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateOneApiHouseholdsMealplansItemIdPut(
    itemId,
    updatePlanEntry,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updatePlanEntry** | **UpdatePlanEntry**|  | |
| **itemId** | [**number**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ReadPlanEntry**

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

