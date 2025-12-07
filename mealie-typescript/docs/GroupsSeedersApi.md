# GroupsSeedersApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**seedFoodsApiGroupsSeedersFoodsPost**](#seedfoodsapigroupsseedersfoodspost) | **POST** /api/groups/seeders/foods | Seed Foods|
|[**seedLabelsApiGroupsSeedersLabelsPost**](#seedlabelsapigroupsseederslabelspost) | **POST** /api/groups/seeders/labels | Seed Labels|
|[**seedUnitsApiGroupsSeedersUnitsPost**](#seedunitsapigroupsseedersunitspost) | **POST** /api/groups/seeders/units | Seed Units|

# **seedFoodsApiGroupsSeedersFoodsPost**
> SuccessResponse seedFoodsApiGroupsSeedersFoodsPost(seederConfig)


### Example

```typescript
import {
    GroupsSeedersApi,
    Configuration,
    SeederConfig
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new GroupsSeedersApi(configuration);

let seederConfig: SeederConfig; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.seedFoodsApiGroupsSeedersFoodsPost(
    seederConfig,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **seederConfig** | **SeederConfig**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**SuccessResponse**

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

# **seedLabelsApiGroupsSeedersLabelsPost**
> SuccessResponse seedLabelsApiGroupsSeedersLabelsPost(seederConfig)


### Example

```typescript
import {
    GroupsSeedersApi,
    Configuration,
    SeederConfig
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new GroupsSeedersApi(configuration);

let seederConfig: SeederConfig; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.seedLabelsApiGroupsSeedersLabelsPost(
    seederConfig,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **seederConfig** | **SeederConfig**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**SuccessResponse**

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

# **seedUnitsApiGroupsSeedersUnitsPost**
> SuccessResponse seedUnitsApiGroupsSeedersUnitsPost(seederConfig)


### Example

```typescript
import {
    GroupsSeedersApi,
    Configuration,
    SeederConfig
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new GroupsSeedersApi(configuration);

let seederConfig: SeederConfig; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.seedUnitsApiGroupsSeedersUnitsPost(
    seederConfig,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **seederConfig** | **SeederConfig**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**SuccessResponse**

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

