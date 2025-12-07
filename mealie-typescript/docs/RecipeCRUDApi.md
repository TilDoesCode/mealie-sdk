# RecipeCRUDApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createOneApiRecipesPost**](#createoneapirecipespost) | **POST** /api/recipes | Create One|
|[**createRecipeFromHtmlOrJsonApiRecipesCreateHtmlOrJsonPost**](#createrecipefromhtmlorjsonapirecipescreatehtmlorjsonpost) | **POST** /api/recipes/create/html-or-json | Create Recipe From Html Or Json|
|[**createRecipeFromImageApiRecipesCreateImagePost**](#createrecipefromimageapirecipescreateimagepost) | **POST** /api/recipes/create/image | Create Recipe From Image|
|[**createRecipeFromZipApiRecipesCreateZipPost**](#createrecipefromzipapirecipescreatezippost) | **POST** /api/recipes/create/zip | Create Recipe From Zip|
|[**deleteOneApiRecipesSlugDelete**](#deleteoneapirecipesslugdelete) | **DELETE** /api/recipes/{slug} | Delete One|
|[**deleteRecipeImageApiRecipesSlugImageDelete**](#deleterecipeimageapirecipesslugimagedelete) | **DELETE** /api/recipes/{slug}/image | Delete Recipe Image|
|[**duplicateOneApiRecipesSlugDuplicatePost**](#duplicateoneapirecipesslugduplicatepost) | **POST** /api/recipes/{slug}/duplicate | Duplicate One|
|[**getAllApiRecipesGet**](#getallapirecipesget) | **GET** /api/recipes | Get All|
|[**getOneApiRecipesSlugGet**](#getoneapirecipesslugget) | **GET** /api/recipes/{slug} | Get One|
|[**parseRecipeUrlApiRecipesCreateUrlPost**](#parserecipeurlapirecipescreateurlpost) | **POST** /api/recipes/create/url | Parse Recipe Url|
|[**parseRecipeUrlBulkApiRecipesCreateUrlBulkPost**](#parserecipeurlbulkapirecipescreateurlbulkpost) | **POST** /api/recipes/create/url/bulk | Parse Recipe Url Bulk|
|[**patchManyApiRecipesPatch**](#patchmanyapirecipespatch) | **PATCH** /api/recipes | Patch Many|
|[**patchOneApiRecipesSlugPatch**](#patchoneapirecipesslugpatch) | **PATCH** /api/recipes/{slug} | Patch One|
|[**scrapeImageUrlApiRecipesSlugImagePost**](#scrapeimageurlapirecipesslugimagepost) | **POST** /api/recipes/{slug}/image | Scrape Image Url|
|[**suggestRecipesApiRecipesSuggestionsGet**](#suggestrecipesapirecipessuggestionsget) | **GET** /api/recipes/suggestions | Suggest Recipes|
|[**testParseRecipeUrlApiRecipesTestScrapeUrlPost**](#testparserecipeurlapirecipestestscrapeurlpost) | **POST** /api/recipes/test-scrape-url | Test Parse Recipe Url|
|[**updateLastMadeApiRecipesSlugLastMadePatch**](#updatelastmadeapirecipessluglastmadepatch) | **PATCH** /api/recipes/{slug}/last-made | Update Last Made|
|[**updateManyApiRecipesPut**](#updatemanyapirecipesput) | **PUT** /api/recipes | Update Many|
|[**updateOneApiRecipesSlugPut**](#updateoneapirecipesslugput) | **PUT** /api/recipes/{slug} | Update One|
|[**updateRecipeImageApiRecipesSlugImagePut**](#updaterecipeimageapirecipesslugimageput) | **PUT** /api/recipes/{slug}/image | Update Recipe Image|
|[**uploadRecipeAssetApiRecipesSlugAssetsPost**](#uploadrecipeassetapirecipesslugassetspost) | **POST** /api/recipes/{slug}/assets | Upload Recipe Asset|

# **createOneApiRecipesPost**
> string createOneApiRecipesPost(createRecipe)

Takes in a JSON string and loads data into the database as a new entry

### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration,
    CreateRecipe
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let createRecipe: CreateRecipe; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createOneApiRecipesPost(
    createRecipe,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createRecipe** | **CreateRecipe**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**string**

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

# **createRecipeFromHtmlOrJsonApiRecipesCreateHtmlOrJsonPost**
> any createRecipeFromHtmlOrJsonApiRecipesCreateHtmlOrJsonPost(scrapeRecipeData)

Takes in raw HTML or a https://schema.org/Recipe object as a JSON string and parses it like a URL

### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration,
    ScrapeRecipeData
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let scrapeRecipeData: ScrapeRecipeData; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createRecipeFromHtmlOrJsonApiRecipesCreateHtmlOrJsonPost(
    scrapeRecipeData,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **scrapeRecipeData** | **ScrapeRecipeData**|  | |
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

# **createRecipeFromImageApiRecipesCreateImagePost**
> any createRecipeFromImageApiRecipesCreateImagePost()

Create a recipe from an image using OpenAI. Optionally specify a language for it to translate the recipe to.

### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let images: Array<File>; // (default to undefined)
let translateLanguage: string; // (optional) (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createRecipeFromImageApiRecipesCreateImagePost(
    images,
    translateLanguage,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **images** | **Array&lt;File&gt;** |  | defaults to undefined|
| **translateLanguage** | [**string**] |  | (optional) defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**any**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createRecipeFromZipApiRecipesCreateZipPost**
> any createRecipeFromZipApiRecipesCreateZipPost()

Create recipe from archive

### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let archive: File; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createRecipeFromZipApiRecipesCreateZipPost(
    archive,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **archive** | [**File**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**any**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteOneApiRecipesSlugDelete**
> any deleteOneApiRecipesSlugDelete()

Deletes a recipe by slug

### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let slug: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteOneApiRecipesSlugDelete(
    slug,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **slug** | [**string**] |  | defaults to undefined|
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

# **deleteRecipeImageApiRecipesSlugImageDelete**
> any deleteRecipeImageApiRecipesSlugImageDelete()


### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let slug: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteRecipeImageApiRecipesSlugImageDelete(
    slug,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **slug** | [**string**] |  | defaults to undefined|
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

# **duplicateOneApiRecipesSlugDuplicatePost**
> RecipeOutput duplicateOneApiRecipesSlugDuplicatePost(recipeDuplicate)

Duplicates a recipe with a new custom name if given

### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration,
    RecipeDuplicate
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let slug: string; // (default to undefined)
let recipeDuplicate: RecipeDuplicate; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.duplicateOneApiRecipesSlugDuplicatePost(
    slug,
    recipeDuplicate,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **recipeDuplicate** | **RecipeDuplicate**|  | |
| **slug** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**RecipeOutput**

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

# **getAllApiRecipesGet**
> PaginationBaseRecipeSummary getAllApiRecipesGet()


### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration,
    Cookbook
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let categories: Array<GetAllApiRecipesGetCategoriesParameterInner>; // (optional) (default to undefined)
let tags: Array<GetAllApiRecipesGetTagsParameterInner>; // (optional) (default to undefined)
let tools: Array<GetAllApiRecipesGetTagsParameterInner>; // (optional) (default to undefined)
let foods: Array<GetAllApiRecipesGetTagsParameterInner>; // (optional) (default to undefined)
let households: Array<GetAllApiRecipesGetTagsParameterInner>; // (optional) (default to undefined)
let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 1)
let perPage: number; // (optional) (default to 50)
let cookbook: Cookbook; // (optional) (default to undefined)
let requireAllCategories: boolean; // (optional) (default to false)
let requireAllTags: boolean; // (optional) (default to false)
let requireAllTools: boolean; // (optional) (default to false)
let requireAllFoods: boolean; // (optional) (default to false)
let search: string; // (optional) (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiRecipesGet(
    categories,
    tags,
    tools,
    foods,
    households,
    orderBy,
    orderByNullPosition,
    orderDirection,
    queryFilter,
    paginationSeed,
    page,
    perPage,
    cookbook,
    requireAllCategories,
    requireAllTags,
    requireAllTools,
    requireAllFoods,
    search,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **categories** | **Array&lt;GetAllApiRecipesGetCategoriesParameterInner&gt;** |  | (optional) defaults to undefined|
| **tags** | **Array&lt;GetAllApiRecipesGetTagsParameterInner&gt;** |  | (optional) defaults to undefined|
| **tools** | **Array&lt;GetAllApiRecipesGetTagsParameterInner&gt;** |  | (optional) defaults to undefined|
| **foods** | **Array&lt;GetAllApiRecipesGetTagsParameterInner&gt;** |  | (optional) defaults to undefined|
| **households** | **Array&lt;GetAllApiRecipesGetTagsParameterInner&gt;** |  | (optional) defaults to undefined|
| **orderBy** | [**string**] |  | (optional) defaults to undefined|
| **orderByNullPosition** | **OrderByNullPosition** |  | (optional) defaults to undefined|
| **orderDirection** | **OrderDirection** |  | (optional) defaults to undefined|
| **queryFilter** | [**string**] |  | (optional) defaults to undefined|
| **paginationSeed** | [**string**] |  | (optional) defaults to undefined|
| **page** | [**number**] |  | (optional) defaults to 1|
| **perPage** | [**number**] |  | (optional) defaults to 50|
| **cookbook** | **Cookbook** |  | (optional) defaults to undefined|
| **requireAllCategories** | [**boolean**] |  | (optional) defaults to false|
| **requireAllTags** | [**boolean**] |  | (optional) defaults to false|
| **requireAllTools** | [**boolean**] |  | (optional) defaults to false|
| **requireAllFoods** | [**boolean**] |  | (optional) defaults to false|
| **search** | [**string**] |  | (optional) defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**PaginationBaseRecipeSummary**

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

# **getOneApiRecipesSlugGet**
> RecipeOutput getOneApiRecipesSlugGet()

Takes in a recipe\'s slug or id and returns all data for a recipe

### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let slug: string; //A recipe\'s slug or id (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getOneApiRecipesSlugGet(
    slug,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **slug** | [**string**] | A recipe\&#39;s slug or id | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**RecipeOutput**

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

# **parseRecipeUrlApiRecipesCreateUrlPost**
> string parseRecipeUrlApiRecipesCreateUrlPost(scrapeRecipe)

Takes in a URL and attempts to scrape data and load it into the database

### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration,
    ScrapeRecipe
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let scrapeRecipe: ScrapeRecipe; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.parseRecipeUrlApiRecipesCreateUrlPost(
    scrapeRecipe,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **scrapeRecipe** | **ScrapeRecipe**|  | |
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**string**

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

# **parseRecipeUrlBulkApiRecipesCreateUrlBulkPost**
> any parseRecipeUrlBulkApiRecipesCreateUrlBulkPost(createRecipeByUrlBulk)

Takes in a URL and attempts to scrape data and load it into the database

### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration,
    CreateRecipeByUrlBulk
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let createRecipeByUrlBulk: CreateRecipeByUrlBulk; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.parseRecipeUrlBulkApiRecipesCreateUrlBulkPost(
    createRecipeByUrlBulk,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createRecipeByUrlBulk** | **CreateRecipeByUrlBulk**|  | |
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
|**202** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patchManyApiRecipesPatch**
> any patchManyApiRecipesPatch(recipeInput)


### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let recipeInput: Array<RecipeInput>; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.patchManyApiRecipesPatch(
    recipeInput,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **recipeInput** | **Array<RecipeInput>**|  | |
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
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patchOneApiRecipesSlugPatch**
> any patchOneApiRecipesSlugPatch(recipeInput)

Updates a recipe by existing slug and data.

### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration,
    RecipeInput
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let slug: string; // (default to undefined)
let recipeInput: RecipeInput; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.patchOneApiRecipesSlugPatch(
    slug,
    recipeInput,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **recipeInput** | **RecipeInput**|  | |
| **slug** | [**string**] |  | defaults to undefined|
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
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **scrapeImageUrlApiRecipesSlugImagePost**
> any scrapeImageUrlApiRecipesSlugImagePost(scrapeRecipe)


### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration,
    ScrapeRecipe
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let slug: string; // (default to undefined)
let scrapeRecipe: ScrapeRecipe; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.scrapeImageUrlApiRecipesSlugImagePost(
    slug,
    scrapeRecipe,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **scrapeRecipe** | **ScrapeRecipe**|  | |
| **slug** | [**string**] |  | defaults to undefined|
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
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **suggestRecipesApiRecipesSuggestionsGet**
> RecipeSuggestionResponse suggestRecipesApiRecipesSuggestionsGet()


### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let foods: Array<string>; // (optional) (default to undefined)
let tools: Array<string>; // (optional) (default to undefined)
let orderBy: string; // (optional) (default to undefined)
let orderByNullPosition: OrderByNullPosition; // (optional) (default to undefined)
let orderDirection: OrderDirection; // (optional) (default to undefined)
let queryFilter: string; // (optional) (default to undefined)
let paginationSeed: string; // (optional) (default to undefined)
let limit: number; // (optional) (default to 10)
let maxMissingFoods: number; // (optional) (default to 5)
let maxMissingTools: number; // (optional) (default to 5)
let includeFoodsOnHand: boolean; // (optional) (default to true)
let includeToolsOnHand: boolean; // (optional) (default to true)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.suggestRecipesApiRecipesSuggestionsGet(
    foods,
    tools,
    orderBy,
    orderByNullPosition,
    orderDirection,
    queryFilter,
    paginationSeed,
    limit,
    maxMissingFoods,
    maxMissingTools,
    includeFoodsOnHand,
    includeToolsOnHand,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **foods** | **Array&lt;string&gt;** |  | (optional) defaults to undefined|
| **tools** | **Array&lt;string&gt;** |  | (optional) defaults to undefined|
| **orderBy** | [**string**] |  | (optional) defaults to undefined|
| **orderByNullPosition** | **OrderByNullPosition** |  | (optional) defaults to undefined|
| **orderDirection** | **OrderDirection** |  | (optional) defaults to undefined|
| **queryFilter** | [**string**] |  | (optional) defaults to undefined|
| **paginationSeed** | [**string**] |  | (optional) defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to 10|
| **maxMissingFoods** | [**number**] |  | (optional) defaults to 5|
| **maxMissingTools** | [**number**] |  | (optional) defaults to 5|
| **includeFoodsOnHand** | [**boolean**] |  | (optional) defaults to true|
| **includeToolsOnHand** | [**boolean**] |  | (optional) defaults to true|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**RecipeSuggestionResponse**

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

# **testParseRecipeUrlApiRecipesTestScrapeUrlPost**
> any testParseRecipeUrlApiRecipesTestScrapeUrlPost(scrapeRecipeTest)


### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration,
    ScrapeRecipeTest
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let scrapeRecipeTest: ScrapeRecipeTest; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.testParseRecipeUrlApiRecipesTestScrapeUrlPost(
    scrapeRecipeTest,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **scrapeRecipeTest** | **ScrapeRecipeTest**|  | |
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
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateLastMadeApiRecipesSlugLastMadePatch**
> any updateLastMadeApiRecipesSlugLastMadePatch(recipeLastMade)

Update a recipe\'s last made timestamp

### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration,
    RecipeLastMade
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let slug: string; // (default to undefined)
let recipeLastMade: RecipeLastMade; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateLastMadeApiRecipesSlugLastMadePatch(
    slug,
    recipeLastMade,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **recipeLastMade** | **RecipeLastMade**|  | |
| **slug** | [**string**] |  | defaults to undefined|
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
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateManyApiRecipesPut**
> any updateManyApiRecipesPut(recipeInput)


### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let recipeInput: Array<RecipeInput>; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateManyApiRecipesPut(
    recipeInput,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **recipeInput** | **Array<RecipeInput>**|  | |
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
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateOneApiRecipesSlugPut**
> any updateOneApiRecipesSlugPut(recipeInput)

Updates a recipe by existing slug and data.

### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration,
    RecipeInput
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let slug: string; // (default to undefined)
let recipeInput: RecipeInput; //
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateOneApiRecipesSlugPut(
    slug,
    recipeInput,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **recipeInput** | **RecipeInput**|  | |
| **slug** | [**string**] |  | defaults to undefined|
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
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateRecipeImageApiRecipesSlugImagePut**
> UpdateImageResponse updateRecipeImageApiRecipesSlugImagePut()


### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let slug: string; // (default to undefined)
let image: File; // (default to undefined)
let extension: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateRecipeImageApiRecipesSlugImagePut(
    slug,
    image,
    extension,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **slug** | [**string**] |  | defaults to undefined|
| **image** | [**File**] |  | defaults to undefined|
| **extension** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**UpdateImageResponse**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **uploadRecipeAssetApiRecipesSlugAssetsPost**
> RecipeAsset uploadRecipeAssetApiRecipesSlugAssetsPost()

Upload a file to store as a recipe asset

### Example

```typescript
import {
    RecipeCRUDApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new RecipeCRUDApi(configuration);

let slug: string; // (default to undefined)
let name: string; // (default to undefined)
let icon: string; // (default to undefined)
let extension: string; // (default to undefined)
let file: File; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.uploadRecipeAssetApiRecipesSlugAssetsPost(
    slug,
    name,
    icon,
    extension,
    file,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **slug** | [**string**] |  | defaults to undefined|
| **name** | [**string**] |  | defaults to undefined|
| **icon** | [**string**] |  | defaults to undefined|
| **extension** | [**string**] |  | defaults to undefined|
| **file** | [**File**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**RecipeAsset**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

