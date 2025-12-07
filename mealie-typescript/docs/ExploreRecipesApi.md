# ExploreRecipesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getAllApiExploreGroupsGroupSlugRecipesGet**](#getallapiexploregroupsgroupslugrecipesget) | **GET** /api/explore/groups/{group_slug}/recipes | Get All|
|[**getRecipeApiExploreGroupsGroupSlugRecipesRecipeSlugGet**](#getrecipeapiexploregroupsgroupslugrecipesrecipeslugget) | **GET** /api/explore/groups/{group_slug}/recipes/{recipe_slug} | Get Recipe|
|[**suggestRecipesApiExploreGroupsGroupSlugRecipesSuggestionsGet**](#suggestrecipesapiexploregroupsgroupslugrecipessuggestionsget) | **GET** /api/explore/groups/{group_slug}/recipes/suggestions | Suggest Recipes|

# **getAllApiExploreGroupsGroupSlugRecipesGet**
> PaginationBaseRecipeSummary getAllApiExploreGroupsGroupSlugRecipesGet()


### Example

```typescript
import {
    ExploreRecipesApi,
    Configuration,
    Cookbook1
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new ExploreRecipesApi(configuration);

let groupSlug: string; // (default to undefined)
let categories: Array<GetAllApiRecipesGetTagsParameterInner>; // (optional) (default to undefined)
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
let cookbook: Cookbook1; // (optional) (default to undefined)
let requireAllCategories: boolean; // (optional) (default to false)
let requireAllTags: boolean; // (optional) (default to false)
let requireAllTools: boolean; // (optional) (default to false)
let requireAllFoods: boolean; // (optional) (default to false)
let search: string; // (optional) (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllApiExploreGroupsGroupSlugRecipesGet(
    groupSlug,
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
| **groupSlug** | [**string**] |  | defaults to undefined|
| **categories** | **Array&lt;GetAllApiRecipesGetTagsParameterInner&gt;** |  | (optional) defaults to undefined|
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
| **cookbook** | **Cookbook1** |  | (optional) defaults to undefined|
| **requireAllCategories** | [**boolean**] |  | (optional) defaults to false|
| **requireAllTags** | [**boolean**] |  | (optional) defaults to false|
| **requireAllTools** | [**boolean**] |  | (optional) defaults to false|
| **requireAllFoods** | [**boolean**] |  | (optional) defaults to false|
| **search** | [**string**] |  | (optional) defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**PaginationBaseRecipeSummary**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getRecipeApiExploreGroupsGroupSlugRecipesRecipeSlugGet**
> RecipeOutput getRecipeApiExploreGroupsGroupSlugRecipesRecipeSlugGet()


### Example

```typescript
import {
    ExploreRecipesApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new ExploreRecipesApi(configuration);

let recipeSlug: string; // (default to undefined)
let groupSlug: string; // (default to undefined)
let acceptLanguage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getRecipeApiExploreGroupsGroupSlugRecipesRecipeSlugGet(
    recipeSlug,
    groupSlug,
    acceptLanguage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **recipeSlug** | [**string**] |  | defaults to undefined|
| **groupSlug** | [**string**] |  | defaults to undefined|
| **acceptLanguage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**RecipeOutput**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **suggestRecipesApiExploreGroupsGroupSlugRecipesSuggestionsGet**
> RecipeSuggestionResponse suggestRecipesApiExploreGroupsGroupSlugRecipesSuggestionsGet()


### Example

```typescript
import {
    ExploreRecipesApi,
    Configuration
} from 'mealie-typescript';

const configuration = new Configuration();
const apiInstance = new ExploreRecipesApi(configuration);

let groupSlug: string; // (default to undefined)
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

const { status, data } = await apiInstance.suggestRecipesApiExploreGroupsGroupSlugRecipesSuggestionsGet(
    groupSlug,
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
| **groupSlug** | [**string**] |  | defaults to undefined|
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

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

