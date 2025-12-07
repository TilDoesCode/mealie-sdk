# RecipeIngredientParserApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**parseIngredientApiParserIngredientPost**](#parseingredientapiparseringredientpost) | **POST** /api/parser/ingredient | Parse Ingredient|
|[**parseIngredientsApiParserIngredientsPost**](#parseingredientsapiparseringredientspost) | **POST** /api/parser/ingredients | Parse Ingredients|

# **parseIngredientApiParserIngredientPost**
> ParsedIngredient parseIngredientApiParserIngredientPost(ingredientRequest)


### Example

```typescript
import {
    RecipeIngredientParserApi,
    Configuration,
    IngredientRequest
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeIngredientParserApi(configuration);

let ingredientRequest: IngredientRequest; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.parseIngredientApiParserIngredientPost(
    ingredientRequest,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **ingredientRequest** | **IngredientRequest**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ParsedIngredient**

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

# **parseIngredientsApiParserIngredientsPost**
> Array<ParsedIngredient> parseIngredientsApiParserIngredientsPost(ingredientsRequest)


### Example

```typescript
import {
    RecipeIngredientParserApi,
    Configuration,
    IngredientsRequest
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeIngredientParserApi(configuration);

let ingredientsRequest: IngredientsRequest; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.parseIngredientsApiParserIngredientsPost(
    ingredientsRequest,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **ingredientsRequest** | **IngredientsRequest**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Array<ParsedIngredient>**

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

