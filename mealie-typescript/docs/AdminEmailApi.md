# AdminEmailApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**checkEmailConfigApiAdminEmailGet**](#checkemailconfigapiadminemailget) | **GET** /api/admin/email | Check Email Config|
|[**sendTestEmailApiAdminEmailPost**](#sendtestemailapiadminemailpost) | **POST** /api/admin/email | Send Test Email|

# **checkEmailConfigApiAdminEmailGet**
> EmailReady checkEmailConfigApiAdminEmailGet()

Get general application information

### Example

```typescript
import {
    AdminEmailApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminEmailApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.checkEmailConfigApiAdminEmailGet(
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**EmailReady**

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

# **sendTestEmailApiAdminEmailPost**
> EmailSuccess sendTestEmailApiAdminEmailPost(emailTest)


### Example

```typescript
import {
    AdminEmailApi,
    Configuration,
    EmailTest
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new AdminEmailApi(configuration);

let emailTest: EmailTest; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.sendTestEmailApiAdminEmailPost(
    emailTest,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **emailTest** | **EmailTest**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**EmailSuccess**

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

