# AppAboutApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getAppInfoApiAppAboutGet**](#getappinfoapiappaboutget) | **GET** /api/app/about | Get App Info|
|[**getAppThemeApiAppAboutThemeGet**](#getappthemeapiappaboutthemeget) | **GET** /api/app/about/theme | Get App Theme|
|[**getStartupInfoApiAppAboutStartupInfoGet**](#getstartupinfoapiappaboutstartupinfoget) | **GET** /api/app/about/startup-info | Get Startup Info|

# **getAppInfoApiAppAboutGet**
> AppInfo getAppInfoApiAppAboutGet()

Get general application information

### Example

```typescript
import {
    AppAboutApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AppAboutApi(configuration);

const { status, data } = await apiInstance.getAppInfoApiAppAboutGet();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**AppInfo**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAppThemeApiAppAboutThemeGet**
> AppTheme getAppThemeApiAppAboutThemeGet()

Get\'s the current theme settings

### Example

```typescript
import {
    AppAboutApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AppAboutApi(configuration);

const { status, data } = await apiInstance.getAppThemeApiAppAboutThemeGet();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**AppTheme**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getStartupInfoApiAppAboutStartupInfoGet**
> AppStartupInfo getStartupInfoApiAppAboutStartupInfoGet()

returns helpful startup information

### Example

```typescript
import {
    AppAboutApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AppAboutApi(configuration);

const { status, data } = await apiInstance.getStartupInfoApiAppAboutStartupInfoGet();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**AppStartupInfo**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

