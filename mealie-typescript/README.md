# mealie-typescript

TypeScript/JavaScript client for the [Mealie](https://mealie.io) API.

WARNING: This auto regenerates everday at midnight. It is recommended that you pin your app to a specific version of this package to keep it from breaking when a change to the mealie api is introduced.

The current api specification is taken from: https://demo.mealie.io/openapi.json

## Installation

```bash
npm install mealie-typescript
```

## Usage

```typescript
import { Configuration, RecipeCRUDApi } from 'mealie-typescript';

const config = new Configuration({
  basePath: 'https://your-mealie-instance.com',
  accessToken: 'your-api-token',
});

const recipesApi = new RecipeCRUDApi(config);

// Get all recipes
const recipes = await recipesApi.getAllApiRecipesGet();
console.log(recipes.data);

// Get a specific recipe
const recipe = await recipesApi.getOneApiRecipesSlugGet('my-recipe-slug');
console.log(recipe.data);
```

### Authentication

Mealie uses OAuth2 password flow. You can obtain a token using the `UsersAuthenticationApi`:

```typescript
import { Configuration, UsersAuthenticationApi } from 'mealie-typescript';

const authApi = new UsersAuthenticationApi(new Configuration({
  basePath: 'https://your-mealie-instance.com',
}));

const response = await authApi.getTokenApiAuthTokenPost(
  'your-username',
  'your-password'
);

const token = response.data.access_token;

// Use the token for subsequent requests
const config = new Configuration({
  basePath: 'https://your-mealie-instance.com',
  accessToken: token,
});
```

### Available APIs

The client provides access to all Mealie API endpoints:

- `RecipeCRUDApi` - Create, read, update, delete recipes
- `RecipeCommentsApi` - Manage recipe comments
- `OrganizerCategoriesApi` - Manage recipe categories
- `OrganizerTagsApi` - Manage recipe tags
- `HouseholdsMealplansApi` - Meal planning
- `HouseholdsShoppingListsApi` - Shopping lists
- `UsersAuthenticationApi` - Authentication
- `AdminManageUsersApi` - User management (admin)

See the [docs](./docs) folder for complete API documentation.

## Requirements

- Node.js >= 16
- A running Mealie instance

## License

MIT
