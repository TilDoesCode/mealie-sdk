# HouseholdsInvitationsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createInviteTokenApiHouseholdsInvitationsPost**](#createinvitetokenapihouseholdsinvitationspost) | **POST** /api/households/invitations | Create Invite Token|
|[**emailInvitationApiHouseholdsInvitationsEmailPost**](#emailinvitationapihouseholdsinvitationsemailpost) | **POST** /api/households/invitations/email | Email Invitation|
|[**getInviteTokensApiHouseholdsInvitationsGet**](#getinvitetokensapihouseholdsinvitationsget) | **GET** /api/households/invitations | Get Invite Tokens|

# **createInviteTokenApiHouseholdsInvitationsPost**
> ReadInviteToken createInviteTokenApiHouseholdsInvitationsPost(createInviteToken)


### Example

```typescript
import {
    HouseholdsInvitationsApi,
    Configuration,
    CreateInviteToken
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsInvitationsApi(configuration);

let createInviteToken: CreateInviteToken; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createInviteTokenApiHouseholdsInvitationsPost(
    createInviteToken,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createInviteToken** | **CreateInviteToken**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ReadInviteToken**

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

# **emailInvitationApiHouseholdsInvitationsEmailPost**
> EmailInitationResponse emailInvitationApiHouseholdsInvitationsEmailPost(emailInvitation)


### Example

```typescript
import {
    HouseholdsInvitationsApi,
    Configuration,
    EmailInvitation
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsInvitationsApi(configuration);

let emailInvitation: EmailInvitation; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.emailInvitationApiHouseholdsInvitationsEmailPost(
    emailInvitation,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **emailInvitation** | **EmailInvitation**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**EmailInitationResponse**

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

# **getInviteTokensApiHouseholdsInvitationsGet**
> Array<ReadInviteToken> getInviteTokensApiHouseholdsInvitationsGet()


### Example

```typescript
import {
    HouseholdsInvitationsApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new HouseholdsInvitationsApi(configuration);

let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getInviteTokensApiHouseholdsInvitationsGet(
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Array<ReadInviteToken>**

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

