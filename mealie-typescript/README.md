## mealie-typescript@nightly

This generator creates TypeScript/JavaScript client that utilizes [axios](https://github.com/axios/axios). The generated Node module can be used in the following environments:

Environment
* Node.js
* Webpack
* Browserify

Language level
* ES5 - you must have a Promises/A+ library installed
* ES6

Module system
* CommonJS
* ES6 module system

It can be used in both TypeScript and JavaScript. In TypeScript, the definition will be automatically resolved via `package.json`. ([Reference](https://www.typescriptlang.org/docs/handbook/declaration-files/consumption.html))

### Building

To build and compile the typescript sources to javascript use:
```
npm install
npm run build
```

### Publishing

First build the package then run `npm publish`

### Consuming

navigate to the folder of your consuming project and run one of the following commands.

_published:_

```
npm install mealie-typescript@nightly --save
```

_unPublished (not recommended):_

```
npm install PATH_TO_GENERATED_PACKAGE --save
```

### Documentation for API Endpoints

All URIs are relative to *http://localhost*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AdminAboutApi* | [**checkAppConfigApiAdminAboutCheckGet**](docs/AdminAboutApi.md#checkappconfigapiadminaboutcheckget) | **GET** /api/admin/about/check | Check App Config
*AdminAboutApi* | [**getAppInfoApiAdminAboutGet**](docs/AdminAboutApi.md#getappinfoapiadminaboutget) | **GET** /api/admin/about | Get App Info
*AdminAboutApi* | [**getAppStatisticsApiAdminAboutStatisticsGet**](docs/AdminAboutApi.md#getappstatisticsapiadminaboutstatisticsget) | **GET** /api/admin/about/statistics | Get App Statistics
*AdminBackupsApi* | [**createOneApiAdminBackupsPost**](docs/AdminBackupsApi.md#createoneapiadminbackupspost) | **POST** /api/admin/backups | Create One
*AdminBackupsApi* | [**deleteOneApiAdminBackupsFileNameDelete**](docs/AdminBackupsApi.md#deleteoneapiadminbackupsfilenamedelete) | **DELETE** /api/admin/backups/{file_name} | Delete One
*AdminBackupsApi* | [**getAllApiAdminBackupsGet**](docs/AdminBackupsApi.md#getallapiadminbackupsget) | **GET** /api/admin/backups | Get All
*AdminBackupsApi* | [**getOneApiAdminBackupsFileNameGet**](docs/AdminBackupsApi.md#getoneapiadminbackupsfilenameget) | **GET** /api/admin/backups/{file_name} | Get One
*AdminBackupsApi* | [**importOneApiAdminBackupsFileNameRestorePost**](docs/AdminBackupsApi.md#importoneapiadminbackupsfilenamerestorepost) | **POST** /api/admin/backups/{file_name}/restore | Import One
*AdminBackupsApi* | [**uploadOneApiAdminBackupsUploadPost**](docs/AdminBackupsApi.md#uploadoneapiadminbackupsuploadpost) | **POST** /api/admin/backups/upload | Upload One
*AdminDebugApi* | [**debugOpenaiApiAdminDebugOpenaiPost**](docs/AdminDebugApi.md#debugopenaiapiadmindebugopenaipost) | **POST** /api/admin/debug/openai | Debug Openai
*AdminEmailApi* | [**checkEmailConfigApiAdminEmailGet**](docs/AdminEmailApi.md#checkemailconfigapiadminemailget) | **GET** /api/admin/email | Check Email Config
*AdminEmailApi* | [**sendTestEmailApiAdminEmailPost**](docs/AdminEmailApi.md#sendtestemailapiadminemailpost) | **POST** /api/admin/email | Send Test Email
*AdminMaintenanceApi* | [**cleanImagesApiAdminMaintenanceCleanImagesPost**](docs/AdminMaintenanceApi.md#cleanimagesapiadminmaintenancecleanimagespost) | **POST** /api/admin/maintenance/clean/images | Clean Images
*AdminMaintenanceApi* | [**cleanRecipeFoldersApiAdminMaintenanceCleanRecipeFoldersPost**](docs/AdminMaintenanceApi.md#cleanrecipefoldersapiadminmaintenancecleanrecipefolderspost) | **POST** /api/admin/maintenance/clean/recipe-folders | Clean Recipe Folders
*AdminMaintenanceApi* | [**cleanTempApiAdminMaintenanceCleanTempPost**](docs/AdminMaintenanceApi.md#cleantempapiadminmaintenancecleantemppost) | **POST** /api/admin/maintenance/clean/temp | Clean Temp
*AdminMaintenanceApi* | [**getMaintenanceSummaryApiAdminMaintenanceGet**](docs/AdminMaintenanceApi.md#getmaintenancesummaryapiadminmaintenanceget) | **GET** /api/admin/maintenance | Get Maintenance Summary
*AdminMaintenanceApi* | [**getStorageDetailsApiAdminMaintenanceStorageGet**](docs/AdminMaintenanceApi.md#getstoragedetailsapiadminmaintenancestorageget) | **GET** /api/admin/maintenance/storage | Get Storage Details
*AdminManageGroupsApi* | [**createOneApiAdminGroupsPost**](docs/AdminManageGroupsApi.md#createoneapiadmingroupspost) | **POST** /api/admin/groups | Create One
*AdminManageGroupsApi* | [**deleteOneApiAdminGroupsItemIdDelete**](docs/AdminManageGroupsApi.md#deleteoneapiadmingroupsitemiddelete) | **DELETE** /api/admin/groups/{item_id} | Delete One
*AdminManageGroupsApi* | [**getAllApiAdminGroupsGet**](docs/AdminManageGroupsApi.md#getallapiadmingroupsget) | **GET** /api/admin/groups | Get All
*AdminManageGroupsApi* | [**getOneApiAdminGroupsItemIdGet**](docs/AdminManageGroupsApi.md#getoneapiadmingroupsitemidget) | **GET** /api/admin/groups/{item_id} | Get One
*AdminManageGroupsApi* | [**updateOneApiAdminGroupsItemIdPut**](docs/AdminManageGroupsApi.md#updateoneapiadmingroupsitemidput) | **PUT** /api/admin/groups/{item_id} | Update One
*AdminManageHouseholdsApi* | [**createOneApiAdminHouseholdsPost**](docs/AdminManageHouseholdsApi.md#createoneapiadminhouseholdspost) | **POST** /api/admin/households | Create One
*AdminManageHouseholdsApi* | [**deleteOneApiAdminHouseholdsItemIdDelete**](docs/AdminManageHouseholdsApi.md#deleteoneapiadminhouseholdsitemiddelete) | **DELETE** /api/admin/households/{item_id} | Delete One
*AdminManageHouseholdsApi* | [**getAllApiAdminHouseholdsGet**](docs/AdminManageHouseholdsApi.md#getallapiadminhouseholdsget) | **GET** /api/admin/households | Get All
*AdminManageHouseholdsApi* | [**getOneApiAdminHouseholdsItemIdGet**](docs/AdminManageHouseholdsApi.md#getoneapiadminhouseholdsitemidget) | **GET** /api/admin/households/{item_id} | Get One
*AdminManageHouseholdsApi* | [**updateOneApiAdminHouseholdsItemIdPut**](docs/AdminManageHouseholdsApi.md#updateoneapiadminhouseholdsitemidput) | **PUT** /api/admin/households/{item_id} | Update One
*AdminManageUsersApi* | [**createOneApiAdminUsersPost**](docs/AdminManageUsersApi.md#createoneapiadminuserspost) | **POST** /api/admin/users | Create One
*AdminManageUsersApi* | [**deleteOneApiAdminUsersItemIdDelete**](docs/AdminManageUsersApi.md#deleteoneapiadminusersitemiddelete) | **DELETE** /api/admin/users/{item_id} | Delete One
*AdminManageUsersApi* | [**generateTokenApiAdminUsersPasswordResetTokenPost**](docs/AdminManageUsersApi.md#generatetokenapiadminuserspasswordresettokenpost) | **POST** /api/admin/users/password-reset-token | Generate Token
*AdminManageUsersApi* | [**getAllApiAdminUsersGet**](docs/AdminManageUsersApi.md#getallapiadminusersget) | **GET** /api/admin/users | Get All
*AdminManageUsersApi* | [**getOneApiAdminUsersItemIdGet**](docs/AdminManageUsersApi.md#getoneapiadminusersitemidget) | **GET** /api/admin/users/{item_id} | Get One
*AdminManageUsersApi* | [**unlockUsersApiAdminUsersUnlockPost**](docs/AdminManageUsersApi.md#unlockusersapiadminusersunlockpost) | **POST** /api/admin/users/unlock | Unlock Users
*AdminManageUsersApi* | [**updateOneApiAdminUsersItemIdPut**](docs/AdminManageUsersApi.md#updateoneapiadminusersitemidput) | **PUT** /api/admin/users/{item_id} | Update One
*AppAboutApi* | [**getAppInfoApiAppAboutGet**](docs/AppAboutApi.md#getappinfoapiappaboutget) | **GET** /api/app/about | Get App Info
*AppAboutApi* | [**getAppThemeApiAppAboutThemeGet**](docs/AppAboutApi.md#getappthemeapiappaboutthemeget) | **GET** /api/app/about/theme | Get App Theme
*AppAboutApi* | [**getStartupInfoApiAppAboutStartupInfoGet**](docs/AppAboutApi.md#getstartupinfoapiappaboutstartupinfoget) | **GET** /api/app/about/startup-info | Get Startup Info
*ExploreCategoriesApi* | [**getAllApiExploreGroupsGroupSlugOrganizersCategoriesGet**](docs/ExploreCategoriesApi.md#getallapiexploregroupsgroupslugorganizerscategoriesget) | **GET** /api/explore/groups/{group_slug}/organizers/categories | Get All
*ExploreCategoriesApi* | [**getOneApiExploreGroupsGroupSlugOrganizersCategoriesItemIdGet**](docs/ExploreCategoriesApi.md#getoneapiexploregroupsgroupslugorganizerscategoriesitemidget) | **GET** /api/explore/groups/{group_slug}/organizers/categories/{item_id} | Get One
*ExploreCookbooksApi* | [**getAllApiExploreGroupsGroupSlugCookbooksGet**](docs/ExploreCookbooksApi.md#getallapiexploregroupsgroupslugcookbooksget) | **GET** /api/explore/groups/{group_slug}/cookbooks | Get All
*ExploreCookbooksApi* | [**getOneApiExploreGroupsGroupSlugCookbooksItemIdGet**](docs/ExploreCookbooksApi.md#getoneapiexploregroupsgroupslugcookbooksitemidget) | **GET** /api/explore/groups/{group_slug}/cookbooks/{item_id} | Get One
*ExploreFoodsApi* | [**getAllApiExploreGroupsGroupSlugFoodsGet**](docs/ExploreFoodsApi.md#getallapiexploregroupsgroupslugfoodsget) | **GET** /api/explore/groups/{group_slug}/foods | Get All
*ExploreFoodsApi* | [**getOneApiExploreGroupsGroupSlugFoodsItemIdGet**](docs/ExploreFoodsApi.md#getoneapiexploregroupsgroupslugfoodsitemidget) | **GET** /api/explore/groups/{group_slug}/foods/{item_id} | Get One
*ExploreHouseholdsApi* | [**getAllApiExploreGroupsGroupSlugHouseholdsGet**](docs/ExploreHouseholdsApi.md#getallapiexploregroupsgroupslughouseholdsget) | **GET** /api/explore/groups/{group_slug}/households | Get All
*ExploreHouseholdsApi* | [**getHouseholdApiExploreGroupsGroupSlugHouseholdsHouseholdSlugGet**](docs/ExploreHouseholdsApi.md#gethouseholdapiexploregroupsgroupslughouseholdshouseholdslugget) | **GET** /api/explore/groups/{group_slug}/households/{household_slug} | Get Household
*ExploreRecipesApi* | [**getAllApiExploreGroupsGroupSlugRecipesGet**](docs/ExploreRecipesApi.md#getallapiexploregroupsgroupslugrecipesget) | **GET** /api/explore/groups/{group_slug}/recipes | Get All
*ExploreRecipesApi* | [**getRecipeApiExploreGroupsGroupSlugRecipesRecipeSlugGet**](docs/ExploreRecipesApi.md#getrecipeapiexploregroupsgroupslugrecipesrecipeslugget) | **GET** /api/explore/groups/{group_slug}/recipes/{recipe_slug} | Get Recipe
*ExploreRecipesApi* | [**suggestRecipesApiExploreGroupsGroupSlugRecipesSuggestionsGet**](docs/ExploreRecipesApi.md#suggestrecipesapiexploregroupsgroupslugrecipessuggestionsget) | **GET** /api/explore/groups/{group_slug}/recipes/suggestions | Suggest Recipes
*ExploreTagsApi* | [**getAllApiExploreGroupsGroupSlugOrganizersTagsGet**](docs/ExploreTagsApi.md#getallapiexploregroupsgroupslugorganizerstagsget) | **GET** /api/explore/groups/{group_slug}/organizers/tags | Get All
*ExploreTagsApi* | [**getOneApiExploreGroupsGroupSlugOrganizersTagsItemIdGet**](docs/ExploreTagsApi.md#getoneapiexploregroupsgroupslugorganizerstagsitemidget) | **GET** /api/explore/groups/{group_slug}/organizers/tags/{item_id} | Get One
*ExploreToolsApi* | [**getAllApiExploreGroupsGroupSlugOrganizersToolsGet**](docs/ExploreToolsApi.md#getallapiexploregroupsgroupslugorganizerstoolsget) | **GET** /api/explore/groups/{group_slug}/organizers/tools | Get All
*ExploreToolsApi* | [**getOneApiExploreGroupsGroupSlugOrganizersToolsItemIdGet**](docs/ExploreToolsApi.md#getoneapiexploregroupsgroupslugorganizerstoolsitemidget) | **GET** /api/explore/groups/{group_slug}/organizers/tools/{item_id} | Get One
*GroupsHouseholdsApi* | [**getAllHouseholdsApiGroupsHouseholdsGet**](docs/GroupsHouseholdsApi.md#getallhouseholdsapigroupshouseholdsget) | **GET** /api/groups/households | Get All Households
*GroupsHouseholdsApi* | [**getOneHouseholdApiGroupsHouseholdsHouseholdSlugGet**](docs/GroupsHouseholdsApi.md#getonehouseholdapigroupshouseholdshouseholdslugget) | **GET** /api/groups/households/{household_slug} | Get One Household
*GroupsMigrationsApi* | [**startDataMigrationApiGroupsMigrationsPost**](docs/GroupsMigrationsApi.md#startdatamigrationapigroupsmigrationspost) | **POST** /api/groups/migrations | Start Data Migration
*GroupsMultiPurposeLabelsApi* | [**createOneApiGroupsLabelsPost**](docs/GroupsMultiPurposeLabelsApi.md#createoneapigroupslabelspost) | **POST** /api/groups/labels | Create One
*GroupsMultiPurposeLabelsApi* | [**deleteOneApiGroupsLabelsItemIdDelete**](docs/GroupsMultiPurposeLabelsApi.md#deleteoneapigroupslabelsitemiddelete) | **DELETE** /api/groups/labels/{item_id} | Delete One
*GroupsMultiPurposeLabelsApi* | [**getAllApiGroupsLabelsGet**](docs/GroupsMultiPurposeLabelsApi.md#getallapigroupslabelsget) | **GET** /api/groups/labels | Get All
*GroupsMultiPurposeLabelsApi* | [**getOneApiGroupsLabelsItemIdGet**](docs/GroupsMultiPurposeLabelsApi.md#getoneapigroupslabelsitemidget) | **GET** /api/groups/labels/{item_id} | Get One
*GroupsMultiPurposeLabelsApi* | [**updateOneApiGroupsLabelsItemIdPut**](docs/GroupsMultiPurposeLabelsApi.md#updateoneapigroupslabelsitemidput) | **PUT** /api/groups/labels/{item_id} | Update One
*GroupsReportsApi* | [**deleteOneApiGroupsReportsItemIdDelete**](docs/GroupsReportsApi.md#deleteoneapigroupsreportsitemiddelete) | **DELETE** /api/groups/reports/{item_id} | Delete One
*GroupsReportsApi* | [**getAllApiGroupsReportsGet**](docs/GroupsReportsApi.md#getallapigroupsreportsget) | **GET** /api/groups/reports | Get All
*GroupsReportsApi* | [**getOneApiGroupsReportsItemIdGet**](docs/GroupsReportsApi.md#getoneapigroupsreportsitemidget) | **GET** /api/groups/reports/{item_id} | Get One
*GroupsSeedersApi* | [**seedFoodsApiGroupsSeedersFoodsPost**](docs/GroupsSeedersApi.md#seedfoodsapigroupsseedersfoodspost) | **POST** /api/groups/seeders/foods | Seed Foods
*GroupsSeedersApi* | [**seedLabelsApiGroupsSeedersLabelsPost**](docs/GroupsSeedersApi.md#seedlabelsapigroupsseederslabelspost) | **POST** /api/groups/seeders/labels | Seed Labels
*GroupsSeedersApi* | [**seedUnitsApiGroupsSeedersUnitsPost**](docs/GroupsSeedersApi.md#seedunitsapigroupsseedersunitspost) | **POST** /api/groups/seeders/units | Seed Units
*GroupsSelfServiceApi* | [**getGroupMemberApiGroupsMembersUsernameOrIdGet**](docs/GroupsSelfServiceApi.md#getgroupmemberapigroupsmembersusernameoridget) | **GET** /api/groups/members/{username_or_id} | Get Group Member
*GroupsSelfServiceApi* | [**getGroupMembersApiGroupsMembersGet**](docs/GroupsSelfServiceApi.md#getgroupmembersapigroupsmembersget) | **GET** /api/groups/members | Get Group Members
*GroupsSelfServiceApi* | [**getGroupPreferencesApiGroupsPreferencesGet**](docs/GroupsSelfServiceApi.md#getgrouppreferencesapigroupspreferencesget) | **GET** /api/groups/preferences | Get Group Preferences
*GroupsSelfServiceApi* | [**getLoggedInUserGroupApiGroupsSelfGet**](docs/GroupsSelfServiceApi.md#getloggedinusergroupapigroupsselfget) | **GET** /api/groups/self | Get Logged In User Group
*GroupsSelfServiceApi* | [**getStorageApiGroupsStorageGet**](docs/GroupsSelfServiceApi.md#getstorageapigroupsstorageget) | **GET** /api/groups/storage | Get Storage
*GroupsSelfServiceApi* | [**updateGroupPreferencesApiGroupsPreferencesPut**](docs/GroupsSelfServiceApi.md#updategrouppreferencesapigroupspreferencesput) | **PUT** /api/groups/preferences | Update Group Preferences
*HouseholdsCookbooksApi* | [**createOneApiHouseholdsCookbooksPost**](docs/HouseholdsCookbooksApi.md#createoneapihouseholdscookbookspost) | **POST** /api/households/cookbooks | Create One
*HouseholdsCookbooksApi* | [**deleteOneApiHouseholdsCookbooksItemIdDelete**](docs/HouseholdsCookbooksApi.md#deleteoneapihouseholdscookbooksitemiddelete) | **DELETE** /api/households/cookbooks/{item_id} | Delete One
*HouseholdsCookbooksApi* | [**getAllApiHouseholdsCookbooksGet**](docs/HouseholdsCookbooksApi.md#getallapihouseholdscookbooksget) | **GET** /api/households/cookbooks | Get All
*HouseholdsCookbooksApi* | [**getOneApiHouseholdsCookbooksItemIdGet**](docs/HouseholdsCookbooksApi.md#getoneapihouseholdscookbooksitemidget) | **GET** /api/households/cookbooks/{item_id} | Get One
*HouseholdsCookbooksApi* | [**updateManyApiHouseholdsCookbooksPut**](docs/HouseholdsCookbooksApi.md#updatemanyapihouseholdscookbooksput) | **PUT** /api/households/cookbooks | Update Many
*HouseholdsCookbooksApi* | [**updateOneApiHouseholdsCookbooksItemIdPut**](docs/HouseholdsCookbooksApi.md#updateoneapihouseholdscookbooksitemidput) | **PUT** /api/households/cookbooks/{item_id} | Update One
*HouseholdsEventNotificationsApi* | [**createOneApiHouseholdsEventsNotificationsPost**](docs/HouseholdsEventNotificationsApi.md#createoneapihouseholdseventsnotificationspost) | **POST** /api/households/events/notifications | Create One
*HouseholdsEventNotificationsApi* | [**deleteOneApiHouseholdsEventsNotificationsItemIdDelete**](docs/HouseholdsEventNotificationsApi.md#deleteoneapihouseholdseventsnotificationsitemiddelete) | **DELETE** /api/households/events/notifications/{item_id} | Delete One
*HouseholdsEventNotificationsApi* | [**getAllApiHouseholdsEventsNotificationsGet**](docs/HouseholdsEventNotificationsApi.md#getallapihouseholdseventsnotificationsget) | **GET** /api/households/events/notifications | Get All
*HouseholdsEventNotificationsApi* | [**getOneApiHouseholdsEventsNotificationsItemIdGet**](docs/HouseholdsEventNotificationsApi.md#getoneapihouseholdseventsnotificationsitemidget) | **GET** /api/households/events/notifications/{item_id} | Get One
*HouseholdsEventNotificationsApi* | [**testNotificationApiHouseholdsEventsNotificationsItemIdTestPost**](docs/HouseholdsEventNotificationsApi.md#testnotificationapihouseholdseventsnotificationsitemidtestpost) | **POST** /api/households/events/notifications/{item_id}/test | Test Notification
*HouseholdsEventNotificationsApi* | [**updateOneApiHouseholdsEventsNotificationsItemIdPut**](docs/HouseholdsEventNotificationsApi.md#updateoneapihouseholdseventsnotificationsitemidput) | **PUT** /api/households/events/notifications/{item_id} | Update One
*HouseholdsInvitationsApi* | [**createInviteTokenApiHouseholdsInvitationsPost**](docs/HouseholdsInvitationsApi.md#createinvitetokenapihouseholdsinvitationspost) | **POST** /api/households/invitations | Create Invite Token
*HouseholdsInvitationsApi* | [**emailInvitationApiHouseholdsInvitationsEmailPost**](docs/HouseholdsInvitationsApi.md#emailinvitationapihouseholdsinvitationsemailpost) | **POST** /api/households/invitations/email | Email Invitation
*HouseholdsInvitationsApi* | [**getInviteTokensApiHouseholdsInvitationsGet**](docs/HouseholdsInvitationsApi.md#getinvitetokensapihouseholdsinvitationsget) | **GET** /api/households/invitations | Get Invite Tokens
*HouseholdsMealplanRulesApi* | [**createOneApiHouseholdsMealplansRulesPost**](docs/HouseholdsMealplanRulesApi.md#createoneapihouseholdsmealplansrulespost) | **POST** /api/households/mealplans/rules | Create One
*HouseholdsMealplanRulesApi* | [**deleteOneApiHouseholdsMealplansRulesItemIdDelete**](docs/HouseholdsMealplanRulesApi.md#deleteoneapihouseholdsmealplansrulesitemiddelete) | **DELETE** /api/households/mealplans/rules/{item_id} | Delete One
*HouseholdsMealplanRulesApi* | [**getAllApiHouseholdsMealplansRulesGet**](docs/HouseholdsMealplanRulesApi.md#getallapihouseholdsmealplansrulesget) | **GET** /api/households/mealplans/rules | Get All
*HouseholdsMealplanRulesApi* | [**getOneApiHouseholdsMealplansRulesItemIdGet**](docs/HouseholdsMealplanRulesApi.md#getoneapihouseholdsmealplansrulesitemidget) | **GET** /api/households/mealplans/rules/{item_id} | Get One
*HouseholdsMealplanRulesApi* | [**updateOneApiHouseholdsMealplansRulesItemIdPut**](docs/HouseholdsMealplanRulesApi.md#updateoneapihouseholdsmealplansrulesitemidput) | **PUT** /api/households/mealplans/rules/{item_id} | Update One
*HouseholdsMealplansApi* | [**createOneApiHouseholdsMealplansPost**](docs/HouseholdsMealplansApi.md#createoneapihouseholdsmealplanspost) | **POST** /api/households/mealplans | Create One
*HouseholdsMealplansApi* | [**createRandomMealApiHouseholdsMealplansRandomPost**](docs/HouseholdsMealplansApi.md#createrandommealapihouseholdsmealplansrandompost) | **POST** /api/households/mealplans/random | Create Random Meal
*HouseholdsMealplansApi* | [**deleteOneApiHouseholdsMealplansItemIdDelete**](docs/HouseholdsMealplansApi.md#deleteoneapihouseholdsmealplansitemiddelete) | **DELETE** /api/households/mealplans/{item_id} | Delete One
*HouseholdsMealplansApi* | [**getAllApiHouseholdsMealplansGet**](docs/HouseholdsMealplansApi.md#getallapihouseholdsmealplansget) | **GET** /api/households/mealplans | Get All
*HouseholdsMealplansApi* | [**getOneApiHouseholdsMealplansItemIdGet**](docs/HouseholdsMealplansApi.md#getoneapihouseholdsmealplansitemidget) | **GET** /api/households/mealplans/{item_id} | Get One
*HouseholdsMealplansApi* | [**getTodaysMealsApiHouseholdsMealplansTodayGet**](docs/HouseholdsMealplansApi.md#gettodaysmealsapihouseholdsmealplanstodayget) | **GET** /api/households/mealplans/today | Get Todays Meals
*HouseholdsMealplansApi* | [**updateOneApiHouseholdsMealplansItemIdPut**](docs/HouseholdsMealplansApi.md#updateoneapihouseholdsmealplansitemidput) | **PUT** /api/households/mealplans/{item_id} | Update One
*HouseholdsRecipeActionsApi* | [**createOneApiHouseholdsRecipeActionsPost**](docs/HouseholdsRecipeActionsApi.md#createoneapihouseholdsrecipeactionspost) | **POST** /api/households/recipe-actions | Create One
*HouseholdsRecipeActionsApi* | [**deleteOneApiHouseholdsRecipeActionsItemIdDelete**](docs/HouseholdsRecipeActionsApi.md#deleteoneapihouseholdsrecipeactionsitemiddelete) | **DELETE** /api/households/recipe-actions/{item_id} | Delete One
*HouseholdsRecipeActionsApi* | [**getAllApiHouseholdsRecipeActionsGet**](docs/HouseholdsRecipeActionsApi.md#getallapihouseholdsrecipeactionsget) | **GET** /api/households/recipe-actions | Get All
*HouseholdsRecipeActionsApi* | [**getOneApiHouseholdsRecipeActionsItemIdGet**](docs/HouseholdsRecipeActionsApi.md#getoneapihouseholdsrecipeactionsitemidget) | **GET** /api/households/recipe-actions/{item_id} | Get One
*HouseholdsRecipeActionsApi* | [**triggerActionApiHouseholdsRecipeActionsItemIdTriggerRecipeSlugPost**](docs/HouseholdsRecipeActionsApi.md#triggeractionapihouseholdsrecipeactionsitemidtriggerrecipeslugpost) | **POST** /api/households/recipe-actions/{item_id}/trigger/{recipe_slug} | Trigger Action
*HouseholdsRecipeActionsApi* | [**updateOneApiHouseholdsRecipeActionsItemIdPut**](docs/HouseholdsRecipeActionsApi.md#updateoneapihouseholdsrecipeactionsitemidput) | **PUT** /api/households/recipe-actions/{item_id} | Update One
*HouseholdsSelfServiceApi* | [**getHouseholdMembersApiHouseholdsMembersGet**](docs/HouseholdsSelfServiceApi.md#gethouseholdmembersapihouseholdsmembersget) | **GET** /api/households/members | Get Household Members
*HouseholdsSelfServiceApi* | [**getHouseholdPreferencesApiHouseholdsPreferencesGet**](docs/HouseholdsSelfServiceApi.md#gethouseholdpreferencesapihouseholdspreferencesget) | **GET** /api/households/preferences | Get Household Preferences
*HouseholdsSelfServiceApi* | [**getHouseholdRecipeApiHouseholdsSelfRecipesRecipeSlugGet**](docs/HouseholdsSelfServiceApi.md#gethouseholdrecipeapihouseholdsselfrecipesrecipeslugget) | **GET** /api/households/self/recipes/{recipe_slug} | Get Household Recipe
*HouseholdsSelfServiceApi* | [**getLoggedInUserHouseholdApiHouseholdsSelfGet**](docs/HouseholdsSelfServiceApi.md#getloggedinuserhouseholdapihouseholdsselfget) | **GET** /api/households/self | Get Logged In User Household
*HouseholdsSelfServiceApi* | [**getStatisticsApiHouseholdsStatisticsGet**](docs/HouseholdsSelfServiceApi.md#getstatisticsapihouseholdsstatisticsget) | **GET** /api/households/statistics | Get Statistics
*HouseholdsSelfServiceApi* | [**setMemberPermissionsApiHouseholdsPermissionsPut**](docs/HouseholdsSelfServiceApi.md#setmemberpermissionsapihouseholdspermissionsput) | **PUT** /api/households/permissions | Set Member Permissions
*HouseholdsSelfServiceApi* | [**updateHouseholdPreferencesApiHouseholdsPreferencesPut**](docs/HouseholdsSelfServiceApi.md#updatehouseholdpreferencesapihouseholdspreferencesput) | **PUT** /api/households/preferences | Update Household Preferences
*HouseholdsShoppingListItemsApi* | [**createManyApiHouseholdsShoppingItemsCreateBulkPost**](docs/HouseholdsShoppingListItemsApi.md#createmanyapihouseholdsshoppingitemscreatebulkpost) | **POST** /api/households/shopping/items/create-bulk | Create Many
*HouseholdsShoppingListItemsApi* | [**createOneApiHouseholdsShoppingItemsPost**](docs/HouseholdsShoppingListItemsApi.md#createoneapihouseholdsshoppingitemspost) | **POST** /api/households/shopping/items | Create One
*HouseholdsShoppingListItemsApi* | [**deleteManyApiHouseholdsShoppingItemsDelete**](docs/HouseholdsShoppingListItemsApi.md#deletemanyapihouseholdsshoppingitemsdelete) | **DELETE** /api/households/shopping/items | Delete Many
*HouseholdsShoppingListItemsApi* | [**deleteOneApiHouseholdsShoppingItemsItemIdDelete**](docs/HouseholdsShoppingListItemsApi.md#deleteoneapihouseholdsshoppingitemsitemiddelete) | **DELETE** /api/households/shopping/items/{item_id} | Delete One
*HouseholdsShoppingListItemsApi* | [**getAllApiHouseholdsShoppingItemsGet**](docs/HouseholdsShoppingListItemsApi.md#getallapihouseholdsshoppingitemsget) | **GET** /api/households/shopping/items | Get All
*HouseholdsShoppingListItemsApi* | [**getOneApiHouseholdsShoppingItemsItemIdGet**](docs/HouseholdsShoppingListItemsApi.md#getoneapihouseholdsshoppingitemsitemidget) | **GET** /api/households/shopping/items/{item_id} | Get One
*HouseholdsShoppingListItemsApi* | [**updateManyApiHouseholdsShoppingItemsPut**](docs/HouseholdsShoppingListItemsApi.md#updatemanyapihouseholdsshoppingitemsput) | **PUT** /api/households/shopping/items | Update Many
*HouseholdsShoppingListItemsApi* | [**updateOneApiHouseholdsShoppingItemsItemIdPut**](docs/HouseholdsShoppingListItemsApi.md#updateoneapihouseholdsshoppingitemsitemidput) | **PUT** /api/households/shopping/items/{item_id} | Update One
*HouseholdsShoppingListsApi* | [**addRecipeIngredientsToListApiHouseholdsShoppingListsItemIdRecipePost**](docs/HouseholdsShoppingListsApi.md#addrecipeingredientstolistapihouseholdsshoppinglistsitemidrecipepost) | **POST** /api/households/shopping/lists/{item_id}/recipe | Add Recipe Ingredients To List
*HouseholdsShoppingListsApi* | [**addSingleRecipeIngredientsToListApiHouseholdsShoppingListsItemIdRecipeRecipeIdPost**](docs/HouseholdsShoppingListsApi.md#addsinglerecipeingredientstolistapihouseholdsshoppinglistsitemidreciperecipeidpost) | **POST** /api/households/shopping/lists/{item_id}/recipe/{recipe_id} | Add Single Recipe Ingredients To List
*HouseholdsShoppingListsApi* | [**createOneApiHouseholdsShoppingListsPost**](docs/HouseholdsShoppingListsApi.md#createoneapihouseholdsshoppinglistspost) | **POST** /api/households/shopping/lists | Create One
*HouseholdsShoppingListsApi* | [**deleteOneApiHouseholdsShoppingListsItemIdDelete**](docs/HouseholdsShoppingListsApi.md#deleteoneapihouseholdsshoppinglistsitemiddelete) | **DELETE** /api/households/shopping/lists/{item_id} | Delete One
*HouseholdsShoppingListsApi* | [**getAllApiHouseholdsShoppingListsGet**](docs/HouseholdsShoppingListsApi.md#getallapihouseholdsshoppinglistsget) | **GET** /api/households/shopping/lists | Get All
*HouseholdsShoppingListsApi* | [**getOneApiHouseholdsShoppingListsItemIdGet**](docs/HouseholdsShoppingListsApi.md#getoneapihouseholdsshoppinglistsitemidget) | **GET** /api/households/shopping/lists/{item_id} | Get One
*HouseholdsShoppingListsApi* | [**removeRecipeIngredientsFromListApiHouseholdsShoppingListsItemIdRecipeRecipeIdDeletePost**](docs/HouseholdsShoppingListsApi.md#removerecipeingredientsfromlistapihouseholdsshoppinglistsitemidreciperecipeiddeletepost) | **POST** /api/households/shopping/lists/{item_id}/recipe/{recipe_id}/delete | Remove Recipe Ingredients From List
*HouseholdsShoppingListsApi* | [**updateLabelSettingsApiHouseholdsShoppingListsItemIdLabelSettingsPut**](docs/HouseholdsShoppingListsApi.md#updatelabelsettingsapihouseholdsshoppinglistsitemidlabelsettingsput) | **PUT** /api/households/shopping/lists/{item_id}/label-settings | Update Label Settings
*HouseholdsShoppingListsApi* | [**updateOneApiHouseholdsShoppingListsItemIdPut**](docs/HouseholdsShoppingListsApi.md#updateoneapihouseholdsshoppinglistsitemidput) | **PUT** /api/households/shopping/lists/{item_id} | Update One
*HouseholdsWebhooksApi* | [**createOneApiHouseholdsWebhooksPost**](docs/HouseholdsWebhooksApi.md#createoneapihouseholdswebhookspost) | **POST** /api/households/webhooks | Create One
*HouseholdsWebhooksApi* | [**deleteOneApiHouseholdsWebhooksItemIdDelete**](docs/HouseholdsWebhooksApi.md#deleteoneapihouseholdswebhooksitemiddelete) | **DELETE** /api/households/webhooks/{item_id} | Delete One
*HouseholdsWebhooksApi* | [**getAllApiHouseholdsWebhooksGet**](docs/HouseholdsWebhooksApi.md#getallapihouseholdswebhooksget) | **GET** /api/households/webhooks | Get All
*HouseholdsWebhooksApi* | [**getOneApiHouseholdsWebhooksItemIdGet**](docs/HouseholdsWebhooksApi.md#getoneapihouseholdswebhooksitemidget) | **GET** /api/households/webhooks/{item_id} | Get One
*HouseholdsWebhooksApi* | [**rerunWebhooksApiHouseholdsWebhooksRerunPost**](docs/HouseholdsWebhooksApi.md#rerunwebhooksapihouseholdswebhooksrerunpost) | **POST** /api/households/webhooks/rerun | Rerun Webhooks
*HouseholdsWebhooksApi* | [**testOneApiHouseholdsWebhooksItemIdTestPost**](docs/HouseholdsWebhooksApi.md#testoneapihouseholdswebhooksitemidtestpost) | **POST** /api/households/webhooks/{item_id}/test | Test One
*HouseholdsWebhooksApi* | [**updateOneApiHouseholdsWebhooksItemIdPut**](docs/HouseholdsWebhooksApi.md#updateoneapihouseholdswebhooksitemidput) | **PUT** /api/households/webhooks/{item_id} | Update One
*OrganizerCategoriesApi* | [**createOneApiOrganizersCategoriesPost**](docs/OrganizerCategoriesApi.md#createoneapiorganizerscategoriespost) | **POST** /api/organizers/categories | Create One
*OrganizerCategoriesApi* | [**deleteOneApiOrganizersCategoriesItemIdDelete**](docs/OrganizerCategoriesApi.md#deleteoneapiorganizerscategoriesitemiddelete) | **DELETE** /api/organizers/categories/{item_id} | Delete One
*OrganizerCategoriesApi* | [**getAllApiOrganizersCategoriesGet**](docs/OrganizerCategoriesApi.md#getallapiorganizerscategoriesget) | **GET** /api/organizers/categories | Get All
*OrganizerCategoriesApi* | [**getAllEmptyApiOrganizersCategoriesEmptyGet**](docs/OrganizerCategoriesApi.md#getallemptyapiorganizerscategoriesemptyget) | **GET** /api/organizers/categories/empty | Get All Empty
*OrganizerCategoriesApi* | [**getOneApiOrganizersCategoriesItemIdGet**](docs/OrganizerCategoriesApi.md#getoneapiorganizerscategoriesitemidget) | **GET** /api/organizers/categories/{item_id} | Get One
*OrganizerCategoriesApi* | [**getOneBySlugApiOrganizersCategoriesSlugCategorySlugGet**](docs/OrganizerCategoriesApi.md#getonebyslugapiorganizerscategoriesslugcategoryslugget) | **GET** /api/organizers/categories/slug/{category_slug} | Get One By Slug
*OrganizerCategoriesApi* | [**updateOneApiOrganizersCategoriesItemIdPut**](docs/OrganizerCategoriesApi.md#updateoneapiorganizerscategoriesitemidput) | **PUT** /api/organizers/categories/{item_id} | Update One
*OrganizerTagsApi* | [**createOneApiOrganizersTagsPost**](docs/OrganizerTagsApi.md#createoneapiorganizerstagspost) | **POST** /api/organizers/tags | Create One
*OrganizerTagsApi* | [**deleteRecipeTagApiOrganizersTagsItemIdDelete**](docs/OrganizerTagsApi.md#deleterecipetagapiorganizerstagsitemiddelete) | **DELETE** /api/organizers/tags/{item_id} | Delete Recipe Tag
*OrganizerTagsApi* | [**getAllApiOrganizersTagsGet**](docs/OrganizerTagsApi.md#getallapiorganizerstagsget) | **GET** /api/organizers/tags | Get All
*OrganizerTagsApi* | [**getEmptyTagsApiOrganizersTagsEmptyGet**](docs/OrganizerTagsApi.md#getemptytagsapiorganizerstagsemptyget) | **GET** /api/organizers/tags/empty | Get Empty Tags
*OrganizerTagsApi* | [**getOneApiOrganizersTagsItemIdGet**](docs/OrganizerTagsApi.md#getoneapiorganizerstagsitemidget) | **GET** /api/organizers/tags/{item_id} | Get One
*OrganizerTagsApi* | [**getOneBySlugApiOrganizersTagsSlugTagSlugGet**](docs/OrganizerTagsApi.md#getonebyslugapiorganizerstagsslugtagslugget) | **GET** /api/organizers/tags/slug/{tag_slug} | Get One By Slug
*OrganizerTagsApi* | [**updateOneApiOrganizersTagsItemIdPut**](docs/OrganizerTagsApi.md#updateoneapiorganizerstagsitemidput) | **PUT** /api/organizers/tags/{item_id} | Update One
*OrganizerToolsApi* | [**createOneApiOrganizersToolsPost**](docs/OrganizerToolsApi.md#createoneapiorganizerstoolspost) | **POST** /api/organizers/tools | Create One
*OrganizerToolsApi* | [**deleteOneApiOrganizersToolsItemIdDelete**](docs/OrganizerToolsApi.md#deleteoneapiorganizerstoolsitemiddelete) | **DELETE** /api/organizers/tools/{item_id} | Delete One
*OrganizerToolsApi* | [**getAllApiOrganizersToolsGet**](docs/OrganizerToolsApi.md#getallapiorganizerstoolsget) | **GET** /api/organizers/tools | Get All
*OrganizerToolsApi* | [**getOneApiOrganizersToolsItemIdGet**](docs/OrganizerToolsApi.md#getoneapiorganizerstoolsitemidget) | **GET** /api/organizers/tools/{item_id} | Get One
*OrganizerToolsApi* | [**getOneBySlugApiOrganizersToolsSlugToolSlugGet**](docs/OrganizerToolsApi.md#getonebyslugapiorganizerstoolsslugtoolslugget) | **GET** /api/organizers/tools/slug/{tool_slug} | Get One By Slug
*OrganizerToolsApi* | [**updateOneApiOrganizersToolsItemIdPut**](docs/OrganizerToolsApi.md#updateoneapiorganizerstoolsitemidput) | **PUT** /api/organizers/tools/{item_id} | Update One
*RecipeBulkActionsApi* | [**bulkCategorizeRecipesApiRecipesBulkActionsCategorizePost**](docs/RecipeBulkActionsApi.md#bulkcategorizerecipesapirecipesbulkactionscategorizepost) | **POST** /api/recipes/bulk-actions/categorize | Bulk Categorize Recipes
*RecipeBulkActionsApi* | [**bulkDeleteRecipesApiRecipesBulkActionsDeletePost**](docs/RecipeBulkActionsApi.md#bulkdeleterecipesapirecipesbulkactionsdeletepost) | **POST** /api/recipes/bulk-actions/delete | Bulk Delete Recipes
*RecipeBulkActionsApi* | [**bulkExportRecipesApiRecipesBulkActionsExportPost**](docs/RecipeBulkActionsApi.md#bulkexportrecipesapirecipesbulkactionsexportpost) | **POST** /api/recipes/bulk-actions/export | Bulk Export Recipes
*RecipeBulkActionsApi* | [**bulkSettingsRecipesApiRecipesBulkActionsSettingsPost**](docs/RecipeBulkActionsApi.md#bulksettingsrecipesapirecipesbulkactionssettingspost) | **POST** /api/recipes/bulk-actions/settings | Bulk Settings Recipes
*RecipeBulkActionsApi* | [**bulkTagRecipesApiRecipesBulkActionsTagPost**](docs/RecipeBulkActionsApi.md#bulktagrecipesapirecipesbulkactionstagpost) | **POST** /api/recipes/bulk-actions/tag | Bulk Tag Recipes
*RecipeBulkActionsApi* | [**getExportedDataApiRecipesBulkActionsExportGet**](docs/RecipeBulkActionsApi.md#getexporteddataapirecipesbulkactionsexportget) | **GET** /api/recipes/bulk-actions/export | Get Exported Data
*RecipeBulkActionsApi* | [**getExportedDataTokenApiRecipesBulkActionsExportDownloadGet**](docs/RecipeBulkActionsApi.md#getexporteddatatokenapirecipesbulkactionsexportdownloadget) | **GET** /api/recipes/bulk-actions/export/download | Get Exported Data Token
*RecipeBulkActionsApi* | [**purgeExportDataApiRecipesBulkActionsExportPurgeDelete**](docs/RecipeBulkActionsApi.md#purgeexportdataapirecipesbulkactionsexportpurgedelete) | **DELETE** /api/recipes/bulk-actions/export/purge | Purge Export Data
*RecipeCRUDApi* | [**createOneApiRecipesPost**](docs/RecipeCRUDApi.md#createoneapirecipespost) | **POST** /api/recipes | Create One
*RecipeCRUDApi* | [**createRecipeFromHtmlOrJsonApiRecipesCreateHtmlOrJsonPost**](docs/RecipeCRUDApi.md#createrecipefromhtmlorjsonapirecipescreatehtmlorjsonpost) | **POST** /api/recipes/create/html-or-json | Create Recipe From Html Or Json
*RecipeCRUDApi* | [**createRecipeFromImageApiRecipesCreateImagePost**](docs/RecipeCRUDApi.md#createrecipefromimageapirecipescreateimagepost) | **POST** /api/recipes/create/image | Create Recipe From Image
*RecipeCRUDApi* | [**createRecipeFromZipApiRecipesCreateZipPost**](docs/RecipeCRUDApi.md#createrecipefromzipapirecipescreatezippost) | **POST** /api/recipes/create/zip | Create Recipe From Zip
*RecipeCRUDApi* | [**deleteOneApiRecipesSlugDelete**](docs/RecipeCRUDApi.md#deleteoneapirecipesslugdelete) | **DELETE** /api/recipes/{slug} | Delete One
*RecipeCRUDApi* | [**deleteRecipeImageApiRecipesSlugImageDelete**](docs/RecipeCRUDApi.md#deleterecipeimageapirecipesslugimagedelete) | **DELETE** /api/recipes/{slug}/image | Delete Recipe Image
*RecipeCRUDApi* | [**duplicateOneApiRecipesSlugDuplicatePost**](docs/RecipeCRUDApi.md#duplicateoneapirecipesslugduplicatepost) | **POST** /api/recipes/{slug}/duplicate | Duplicate One
*RecipeCRUDApi* | [**getAllApiRecipesGet**](docs/RecipeCRUDApi.md#getallapirecipesget) | **GET** /api/recipes | Get All
*RecipeCRUDApi* | [**getOneApiRecipesSlugGet**](docs/RecipeCRUDApi.md#getoneapirecipesslugget) | **GET** /api/recipes/{slug} | Get One
*RecipeCRUDApi* | [**parseRecipeUrlApiRecipesCreateUrlPost**](docs/RecipeCRUDApi.md#parserecipeurlapirecipescreateurlpost) | **POST** /api/recipes/create/url | Parse Recipe Url
*RecipeCRUDApi* | [**parseRecipeUrlBulkApiRecipesCreateUrlBulkPost**](docs/RecipeCRUDApi.md#parserecipeurlbulkapirecipescreateurlbulkpost) | **POST** /api/recipes/create/url/bulk | Parse Recipe Url Bulk
*RecipeCRUDApi* | [**patchManyApiRecipesPatch**](docs/RecipeCRUDApi.md#patchmanyapirecipespatch) | **PATCH** /api/recipes | Patch Many
*RecipeCRUDApi* | [**patchOneApiRecipesSlugPatch**](docs/RecipeCRUDApi.md#patchoneapirecipesslugpatch) | **PATCH** /api/recipes/{slug} | Patch One
*RecipeCRUDApi* | [**scrapeImageUrlApiRecipesSlugImagePost**](docs/RecipeCRUDApi.md#scrapeimageurlapirecipesslugimagepost) | **POST** /api/recipes/{slug}/image | Scrape Image Url
*RecipeCRUDApi* | [**suggestRecipesApiRecipesSuggestionsGet**](docs/RecipeCRUDApi.md#suggestrecipesapirecipessuggestionsget) | **GET** /api/recipes/suggestions | Suggest Recipes
*RecipeCRUDApi* | [**testParseRecipeUrlApiRecipesTestScrapeUrlPost**](docs/RecipeCRUDApi.md#testparserecipeurlapirecipestestscrapeurlpost) | **POST** /api/recipes/test-scrape-url | Test Parse Recipe Url
*RecipeCRUDApi* | [**updateLastMadeApiRecipesSlugLastMadePatch**](docs/RecipeCRUDApi.md#updatelastmadeapirecipessluglastmadepatch) | **PATCH** /api/recipes/{slug}/last-made | Update Last Made
*RecipeCRUDApi* | [**updateManyApiRecipesPut**](docs/RecipeCRUDApi.md#updatemanyapirecipesput) | **PUT** /api/recipes | Update Many
*RecipeCRUDApi* | [**updateOneApiRecipesSlugPut**](docs/RecipeCRUDApi.md#updateoneapirecipesslugput) | **PUT** /api/recipes/{slug} | Update One
*RecipeCRUDApi* | [**updateRecipeImageApiRecipesSlugImagePut**](docs/RecipeCRUDApi.md#updaterecipeimageapirecipesslugimageput) | **PUT** /api/recipes/{slug}/image | Update Recipe Image
*RecipeCRUDApi* | [**uploadRecipeAssetApiRecipesSlugAssetsPost**](docs/RecipeCRUDApi.md#uploadrecipeassetapirecipesslugassetspost) | **POST** /api/recipes/{slug}/assets | Upload Recipe Asset
*RecipeCommentsApi* | [**createOneApiCommentsPost**](docs/RecipeCommentsApi.md#createoneapicommentspost) | **POST** /api/comments | Create One
*RecipeCommentsApi* | [**deleteOneApiCommentsItemIdDelete**](docs/RecipeCommentsApi.md#deleteoneapicommentsitemiddelete) | **DELETE** /api/comments/{item_id} | Delete One
*RecipeCommentsApi* | [**getAllApiCommentsGet**](docs/RecipeCommentsApi.md#getallapicommentsget) | **GET** /api/comments | Get All
*RecipeCommentsApi* | [**getOneApiCommentsItemIdGet**](docs/RecipeCommentsApi.md#getoneapicommentsitemidget) | **GET** /api/comments/{item_id} | Get One
*RecipeCommentsApi* | [**getRecipeCommentsApiRecipesSlugCommentsGet**](docs/RecipeCommentsApi.md#getrecipecommentsapirecipesslugcommentsget) | **GET** /api/recipes/{slug}/comments | Get Recipe Comments
*RecipeCommentsApi* | [**updateOneApiCommentsItemIdPut**](docs/RecipeCommentsApi.md#updateoneapicommentsitemidput) | **PUT** /api/comments/{item_id} | Update One
*RecipeExportsApi* | [**getRecipeAsFormatApiRecipesSlugExportsGet**](docs/RecipeExportsApi.md#getrecipeasformatapirecipesslugexportsget) | **GET** /api/recipes/{slug}/exports | Get Recipe As Format
*RecipeExportsApi* | [**getRecipeFormatsAndTemplatesApiRecipesExportsGet**](docs/RecipeExportsApi.md#getrecipeformatsandtemplatesapirecipesexportsget) | **GET** /api/recipes/exports | Get Recipe Formats And Templates
*RecipeImagesAndAssetsApi* | [**deleteRecipeImageApiRecipesSlugImageDelete**](docs/RecipeImagesAndAssetsApi.md#deleterecipeimageapirecipesslugimagedelete) | **DELETE** /api/recipes/{slug}/image | Delete Recipe Image
*RecipeImagesAndAssetsApi* | [**getRecipeAssetApiMediaRecipesRecipeIdAssetsFileNameGet**](docs/RecipeImagesAndAssetsApi.md#getrecipeassetapimediarecipesrecipeidassetsfilenameget) | **GET** /api/media/recipes/{recipe_id}/assets/{file_name} | Get Recipe Asset
*RecipeImagesAndAssetsApi* | [**getRecipeImgApiMediaRecipesRecipeIdImagesFileNameGet**](docs/RecipeImagesAndAssetsApi.md#getrecipeimgapimediarecipesrecipeidimagesfilenameget) | **GET** /api/media/recipes/{recipe_id}/images/{file_name} | Get Recipe Img
*RecipeImagesAndAssetsApi* | [**getRecipeTimelineEventImgApiMediaRecipesRecipeIdImagesTimelineTimelineEventIdFileNameGet**](docs/RecipeImagesAndAssetsApi.md#getrecipetimelineeventimgapimediarecipesrecipeidimagestimelinetimelineeventidfilenameget) | **GET** /api/media/recipes/{recipe_id}/images/timeline/{timeline_event_id}/{file_name} | Get Recipe Timeline Event Img
*RecipeImagesAndAssetsApi* | [**getUserImageApiMediaUsersUserIdFileNameGet**](docs/RecipeImagesAndAssetsApi.md#getuserimageapimediausersuseridfilenameget) | **GET** /api/media/users/{user_id}/{file_name} | Get User Image
*RecipeImagesAndAssetsApi* | [**getValidationTextApiMediaDockerValidateTxtGet**](docs/RecipeImagesAndAssetsApi.md#getvalidationtextapimediadockervalidatetxtget) | **GET** /api/media/docker/validate.txt | Get Validation Text
*RecipeImagesAndAssetsApi* | [**scrapeImageUrlApiRecipesSlugImagePost**](docs/RecipeImagesAndAssetsApi.md#scrapeimageurlapirecipesslugimagepost) | **POST** /api/recipes/{slug}/image | Scrape Image Url
*RecipeImagesAndAssetsApi* | [**updateRecipeImageApiRecipesSlugImagePut**](docs/RecipeImagesAndAssetsApi.md#updaterecipeimageapirecipesslugimageput) | **PUT** /api/recipes/{slug}/image | Update Recipe Image
*RecipeImagesAndAssetsApi* | [**uploadRecipeAssetApiRecipesSlugAssetsPost**](docs/RecipeImagesAndAssetsApi.md#uploadrecipeassetapirecipesslugassetspost) | **POST** /api/recipes/{slug}/assets | Upload Recipe Asset
*RecipeIngredientParserApi* | [**parseIngredientApiParserIngredientPost**](docs/RecipeIngredientParserApi.md#parseingredientapiparseringredientpost) | **POST** /api/parser/ingredient | Parse Ingredient
*RecipeIngredientParserApi* | [**parseIngredientsApiParserIngredientsPost**](docs/RecipeIngredientParserApi.md#parseingredientsapiparseringredientspost) | **POST** /api/parser/ingredients | Parse Ingredients
*RecipeSharedApi* | [**getSharedRecipeApiRecipesSharedTokenIdGet**](docs/RecipeSharedApi.md#getsharedrecipeapirecipessharedtokenidget) | **GET** /api/recipes/shared/{token_id} | Get Shared Recipe
*RecipeSharedApi* | [**getSharedRecipeAsZipApiRecipesSharedTokenIdZipGet**](docs/RecipeSharedApi.md#getsharedrecipeaszipapirecipessharedtokenidzipget) | **GET** /api/recipes/shared/{token_id}/zip | Get Shared Recipe As Zip
*RecipeTimelineApi* | [**createOneApiRecipesTimelineEventsPost**](docs/RecipeTimelineApi.md#createoneapirecipestimelineeventspost) | **POST** /api/recipes/timeline/events | Create One
*RecipeTimelineApi* | [**deleteOneApiRecipesTimelineEventsItemIdDelete**](docs/RecipeTimelineApi.md#deleteoneapirecipestimelineeventsitemiddelete) | **DELETE** /api/recipes/timeline/events/{item_id} | Delete One
*RecipeTimelineApi* | [**getAllApiRecipesTimelineEventsGet**](docs/RecipeTimelineApi.md#getallapirecipestimelineeventsget) | **GET** /api/recipes/timeline/events | Get All
*RecipeTimelineApi* | [**getOneApiRecipesTimelineEventsItemIdGet**](docs/RecipeTimelineApi.md#getoneapirecipestimelineeventsitemidget) | **GET** /api/recipes/timeline/events/{item_id} | Get One
*RecipeTimelineApi* | [**updateEventImageApiRecipesTimelineEventsItemIdImagePut**](docs/RecipeTimelineApi.md#updateeventimageapirecipestimelineeventsitemidimageput) | **PUT** /api/recipes/timeline/events/{item_id}/image | Update Event Image
*RecipeTimelineApi* | [**updateOneApiRecipesTimelineEventsItemIdPut**](docs/RecipeTimelineApi.md#updateoneapirecipestimelineeventsitemidput) | **PUT** /api/recipes/timeline/events/{item_id} | Update One
*RecipesFoodsApi* | [**createOneApiFoodsPost**](docs/RecipesFoodsApi.md#createoneapifoodspost) | **POST** /api/foods | Create One
*RecipesFoodsApi* | [**deleteOneApiFoodsItemIdDelete**](docs/RecipesFoodsApi.md#deleteoneapifoodsitemiddelete) | **DELETE** /api/foods/{item_id} | Delete One
*RecipesFoodsApi* | [**getAllApiFoodsGet**](docs/RecipesFoodsApi.md#getallapifoodsget) | **GET** /api/foods | Get All
*RecipesFoodsApi* | [**getOneApiFoodsItemIdGet**](docs/RecipesFoodsApi.md#getoneapifoodsitemidget) | **GET** /api/foods/{item_id} | Get One
*RecipesFoodsApi* | [**mergeOneApiFoodsMergePut**](docs/RecipesFoodsApi.md#mergeoneapifoodsmergeput) | **PUT** /api/foods/merge | Merge One
*RecipesFoodsApi* | [**updateOneApiFoodsItemIdPut**](docs/RecipesFoodsApi.md#updateoneapifoodsitemidput) | **PUT** /api/foods/{item_id} | Update One
*RecipesUnitsApi* | [**createOneApiUnitsPost**](docs/RecipesUnitsApi.md#createoneapiunitspost) | **POST** /api/units | Create One
*RecipesUnitsApi* | [**deleteOneApiUnitsItemIdDelete**](docs/RecipesUnitsApi.md#deleteoneapiunitsitemiddelete) | **DELETE** /api/units/{item_id} | Delete One
*RecipesUnitsApi* | [**getAllApiUnitsGet**](docs/RecipesUnitsApi.md#getallapiunitsget) | **GET** /api/units | Get All
*RecipesUnitsApi* | [**getOneApiUnitsItemIdGet**](docs/RecipesUnitsApi.md#getoneapiunitsitemidget) | **GET** /api/units/{item_id} | Get One
*RecipesUnitsApi* | [**mergeOneApiUnitsMergePut**](docs/RecipesUnitsApi.md#mergeoneapiunitsmergeput) | **PUT** /api/units/merge | Merge One
*RecipesUnitsApi* | [**updateOneApiUnitsItemIdPut**](docs/RecipesUnitsApi.md#updateoneapiunitsitemidput) | **PUT** /api/units/{item_id} | Update One
*SharedRecipesApi* | [**createOneApiSharedRecipesPost**](docs/SharedRecipesApi.md#createoneapisharedrecipespost) | **POST** /api/shared/recipes | Create One
*SharedRecipesApi* | [**deleteOneApiSharedRecipesItemIdDelete**](docs/SharedRecipesApi.md#deleteoneapisharedrecipesitemiddelete) | **DELETE** /api/shared/recipes/{item_id} | Delete One
*SharedRecipesApi* | [**getAllApiSharedRecipesGet**](docs/SharedRecipesApi.md#getallapisharedrecipesget) | **GET** /api/shared/recipes | Get All
*SharedRecipesApi* | [**getOneApiSharedRecipesItemIdGet**](docs/SharedRecipesApi.md#getoneapisharedrecipesitemidget) | **GET** /api/shared/recipes/{item_id} | Get One
*UsersAuthenticationApi* | [**getTokenApiAuthTokenPost**](docs/UsersAuthenticationApi.md#gettokenapiauthtokenpost) | **POST** /api/auth/token | Get Token
*UsersAuthenticationApi* | [**logoutApiAuthLogoutPost**](docs/UsersAuthenticationApi.md#logoutapiauthlogoutpost) | **POST** /api/auth/logout | Logout
*UsersAuthenticationApi* | [**oauthCallbackApiAuthOauthCallbackGet**](docs/UsersAuthenticationApi.md#oauthcallbackapiauthoauthcallbackget) | **GET** /api/auth/oauth/callback | Oauth Callback
*UsersAuthenticationApi* | [**oauthLoginApiAuthOauthGet**](docs/UsersAuthenticationApi.md#oauthloginapiauthoauthget) | **GET** /api/auth/oauth | Oauth Login
*UsersAuthenticationApi* | [**refreshTokenApiAuthRefreshGet**](docs/UsersAuthenticationApi.md#refreshtokenapiauthrefreshget) | **GET** /api/auth/refresh | Refresh Token
*UsersCRUDApi* | [**getLoggedInUserApiUsersSelfGet**](docs/UsersCRUDApi.md#getloggedinuserapiusersselfget) | **GET** /api/users/self | Get Logged In User
*UsersCRUDApi* | [**getLoggedInUserFavoritesApiUsersSelfFavoritesGet**](docs/UsersCRUDApi.md#getloggedinuserfavoritesapiusersselffavoritesget) | **GET** /api/users/self/favorites | Get Logged In User Favorites
*UsersCRUDApi* | [**getLoggedInUserRatingForRecipeApiUsersSelfRatingsRecipeIdGet**](docs/UsersCRUDApi.md#getloggedinuserratingforrecipeapiusersselfratingsrecipeidget) | **GET** /api/users/self/ratings/{recipe_id} | Get Logged In User Rating For Recipe
*UsersCRUDApi* | [**getLoggedInUserRatingsApiUsersSelfRatingsGet**](docs/UsersCRUDApi.md#getloggedinuserratingsapiusersselfratingsget) | **GET** /api/users/self/ratings | Get Logged In User Ratings
*UsersCRUDApi* | [**updatePasswordApiUsersPasswordPut**](docs/UsersCRUDApi.md#updatepasswordapiuserspasswordput) | **PUT** /api/users/password | Update Password
*UsersCRUDApi* | [**updateUserApiUsersItemIdPut**](docs/UsersCRUDApi.md#updateuserapiusersitemidput) | **PUT** /api/users/{item_id} | Update User
*UsersImagesApi* | [**updateUserImageApiUsersIdImagePost**](docs/UsersImagesApi.md#updateuserimageapiusersidimagepost) | **POST** /api/users/{id}/image | Update User Image
*UsersPasswordsApi* | [**forgotPasswordApiUsersForgotPasswordPost**](docs/UsersPasswordsApi.md#forgotpasswordapiusersforgotpasswordpost) | **POST** /api/users/forgot-password | Forgot Password
*UsersPasswordsApi* | [**resetPasswordApiUsersResetPasswordPost**](docs/UsersPasswordsApi.md#resetpasswordapiusersresetpasswordpost) | **POST** /api/users/reset-password | Reset Password
*UsersRatingsApi* | [**addFavoriteApiUsersIdFavoritesSlugPost**](docs/UsersRatingsApi.md#addfavoriteapiusersidfavoritesslugpost) | **POST** /api/users/{id}/favorites/{slug} | Add Favorite
*UsersRatingsApi* | [**getFavoritesApiUsersIdFavoritesGet**](docs/UsersRatingsApi.md#getfavoritesapiusersidfavoritesget) | **GET** /api/users/{id}/favorites | Get Favorites
*UsersRatingsApi* | [**getRatingsApiUsersIdRatingsGet**](docs/UsersRatingsApi.md#getratingsapiusersidratingsget) | **GET** /api/users/{id}/ratings | Get Ratings
*UsersRatingsApi* | [**removeFavoriteApiUsersIdFavoritesSlugDelete**](docs/UsersRatingsApi.md#removefavoriteapiusersidfavoritesslugdelete) | **DELETE** /api/users/{id}/favorites/{slug} | Remove Favorite
*UsersRatingsApi* | [**setRatingApiUsersIdRatingsSlugPost**](docs/UsersRatingsApi.md#setratingapiusersidratingsslugpost) | **POST** /api/users/{id}/ratings/{slug} | Set Rating
*UsersRegistrationApi* | [**registerNewUserApiUsersRegisterPost**](docs/UsersRegistrationApi.md#registernewuserapiusersregisterpost) | **POST** /api/users/register | Register New User
*UsersTokensApi* | [**createApiTokenApiUsersApiTokensPost**](docs/UsersTokensApi.md#createapitokenapiusersapitokenspost) | **POST** /api/users/api-tokens | Create Api Token
*UsersTokensApi* | [**deleteApiTokenApiUsersApiTokensTokenIdDelete**](docs/UsersTokensApi.md#deleteapitokenapiusersapitokenstokeniddelete) | **DELETE** /api/users/api-tokens/{token_id} | Delete Api Token
*UtilsApi* | [**downloadFileApiUtilsDownloadGet**](docs/UtilsApi.md#downloadfileapiutilsdownloadget) | **GET** /api/utils/download | Download File


### Documentation For Models

 - [AdminAboutInfo](docs/AdminAboutInfo.md)
 - [AllBackups](docs/AllBackups.md)
 - [AppInfo](docs/AppInfo.md)
 - [AppStartupInfo](docs/AppStartupInfo.md)
 - [AppStatistics](docs/AppStatistics.md)
 - [AppTheme](docs/AppTheme.md)
 - [AssignCategories](docs/AssignCategories.md)
 - [AssignSettings](docs/AssignSettings.md)
 - [AssignTags](docs/AssignTags.md)
 - [AuthMethod](docs/AuthMethod.md)
 - [BackupFile](docs/BackupFile.md)
 - [BodyTriggerActionApiHouseholdsRecipeActionsItemIdTriggerRecipeSlugPost](docs/BodyTriggerActionApiHouseholdsRecipeActionsItemIdTriggerRecipeSlugPost.md)
 - [CategoryBase](docs/CategoryBase.md)
 - [CategoryIn](docs/CategoryIn.md)
 - [CategoryOut](docs/CategoryOut.md)
 - [CategorySummary](docs/CategorySummary.md)
 - [ChangePassword](docs/ChangePassword.md)
 - [CheckAppConfig](docs/CheckAppConfig.md)
 - [CookBookPagination](docs/CookBookPagination.md)
 - [Cookbook](docs/Cookbook.md)
 - [Cookbook1](docs/Cookbook1.md)
 - [CookbookHousehold](docs/CookbookHousehold.md)
 - [CreateCookBook](docs/CreateCookBook.md)
 - [CreateGroupRecipeAction](docs/CreateGroupRecipeAction.md)
 - [CreateIngredientFood](docs/CreateIngredientFood.md)
 - [CreateIngredientFoodAlias](docs/CreateIngredientFoodAlias.md)
 - [CreateIngredientUnit](docs/CreateIngredientUnit.md)
 - [CreateIngredientUnitAlias](docs/CreateIngredientUnitAlias.md)
 - [CreateInviteToken](docs/CreateInviteToken.md)
 - [CreatePlanEntry](docs/CreatePlanEntry.md)
 - [CreateRandomEntry](docs/CreateRandomEntry.md)
 - [CreateRecipe](docs/CreateRecipe.md)
 - [CreateRecipeBulk](docs/CreateRecipeBulk.md)
 - [CreateRecipeByUrlBulk](docs/CreateRecipeByUrlBulk.md)
 - [CreateUserRegistration](docs/CreateUserRegistration.md)
 - [CreateWebhook](docs/CreateWebhook.md)
 - [DebugResponse](docs/DebugResponse.md)
 - [DeleteRecipes](docs/DeleteRecipes.md)
 - [DeleteTokenResponse](docs/DeleteTokenResponse.md)
 - [EmailInitationResponse](docs/EmailInitationResponse.md)
 - [EmailInvitation](docs/EmailInvitation.md)
 - [EmailReady](docs/EmailReady.md)
 - [EmailSuccess](docs/EmailSuccess.md)
 - [EmailTest](docs/EmailTest.md)
 - [ExportRecipes](docs/ExportRecipes.md)
 - [ExportTypes](docs/ExportTypes.md)
 - [FileTokenResponse](docs/FileTokenResponse.md)
 - [Food](docs/Food.md)
 - [Food1](docs/Food1.md)
 - [ForgotPassword](docs/ForgotPassword.md)
 - [FormatResponse](docs/FormatResponse.md)
 - [GetAllApiRecipesGetCategoriesParameterInner](docs/GetAllApiRecipesGetCategoriesParameterInner.md)
 - [GetAllApiRecipesGetTagsParameterInner](docs/GetAllApiRecipesGetTagsParameterInner.md)
 - [GroupAdminUpdate](docs/GroupAdminUpdate.md)
 - [GroupBase](docs/GroupBase.md)
 - [GroupDataExport](docs/GroupDataExport.md)
 - [GroupEventNotifierCreate](docs/GroupEventNotifierCreate.md)
 - [GroupEventNotifierOptions](docs/GroupEventNotifierOptions.md)
 - [GroupEventNotifierOptionsOut](docs/GroupEventNotifierOptionsOut.md)
 - [GroupEventNotifierOut](docs/GroupEventNotifierOut.md)
 - [GroupEventNotifierUpdate](docs/GroupEventNotifierUpdate.md)
 - [GroupEventPagination](docs/GroupEventPagination.md)
 - [GroupHouseholdSummary](docs/GroupHouseholdSummary.md)
 - [GroupInDB](docs/GroupInDB.md)
 - [GroupPagination](docs/GroupPagination.md)
 - [GroupRecipeActionOut](docs/GroupRecipeActionOut.md)
 - [GroupRecipeActionPagination](docs/GroupRecipeActionPagination.md)
 - [GroupRecipeActionType](docs/GroupRecipeActionType.md)
 - [GroupStorage](docs/GroupStorage.md)
 - [GroupSummary](docs/GroupSummary.md)
 - [HTTPValidationError](docs/HTTPValidationError.md)
 - [HouseholdCreate](docs/HouseholdCreate.md)
 - [HouseholdInDB](docs/HouseholdInDB.md)
 - [HouseholdPagination](docs/HouseholdPagination.md)
 - [HouseholdRecipeSummary](docs/HouseholdRecipeSummary.md)
 - [HouseholdStatistics](docs/HouseholdStatistics.md)
 - [HouseholdSummary](docs/HouseholdSummary.md)
 - [HouseholdUserSummary](docs/HouseholdUserSummary.md)
 - [ImageType](docs/ImageType.md)
 - [IngredientConfidence](docs/IngredientConfidence.md)
 - [IngredientFoodAlias](docs/IngredientFoodAlias.md)
 - [IngredientFoodInput](docs/IngredientFoodInput.md)
 - [IngredientFoodOutput](docs/IngredientFoodOutput.md)
 - [IngredientFoodPagination](docs/IngredientFoodPagination.md)
 - [IngredientReferences](docs/IngredientReferences.md)
 - [IngredientRequest](docs/IngredientRequest.md)
 - [IngredientUnitAlias](docs/IngredientUnitAlias.md)
 - [IngredientUnitInput](docs/IngredientUnitInput.md)
 - [IngredientUnitOutput](docs/IngredientUnitOutput.md)
 - [IngredientUnitPagination](docs/IngredientUnitPagination.md)
 - [IngredientsRequest](docs/IngredientsRequest.md)
 - [ItemId](docs/ItemId.md)
 - [ItemId1](docs/ItemId1.md)
 - [LogicalOperator](docs/LogicalOperator.md)
 - [LongLiveTokenCreateResponse](docs/LongLiveTokenCreateResponse.md)
 - [LongLiveTokenIn](docs/LongLiveTokenIn.md)
 - [LongLiveTokenOut](docs/LongLiveTokenOut.md)
 - [MaintenanceStorageDetails](docs/MaintenanceStorageDetails.md)
 - [MaintenanceSummary](docs/MaintenanceSummary.md)
 - [MealieSchemaRecipeRecipeCommentsUserBase](docs/MealieSchemaRecipeRecipeCommentsUserBase.md)
 - [MealieSchemaUserUserUserBase](docs/MealieSchemaUserUserUserBase.md)
 - [MergeFood](docs/MergeFood.md)
 - [MergeUnit](docs/MergeUnit.md)
 - [MultiPurposeLabelCreate](docs/MultiPurposeLabelCreate.md)
 - [MultiPurposeLabelOut](docs/MultiPurposeLabelOut.md)
 - [MultiPurposeLabelPagination](docs/MultiPurposeLabelPagination.md)
 - [MultiPurposeLabelSummary](docs/MultiPurposeLabelSummary.md)
 - [MultiPurposeLabelUpdate](docs/MultiPurposeLabelUpdate.md)
 - [Nutrition](docs/Nutrition.md)
 - [OrderByNullPosition](docs/OrderByNullPosition.md)
 - [OrderDirection](docs/OrderDirection.md)
 - [PaginationBaseHouseholdSummary](docs/PaginationBaseHouseholdSummary.md)
 - [PaginationBaseIngredientFood](docs/PaginationBaseIngredientFood.md)
 - [PaginationBaseReadCookBook](docs/PaginationBaseReadCookBook.md)
 - [PaginationBaseRecipeCategory](docs/PaginationBaseRecipeCategory.md)
 - [PaginationBaseRecipeSummary](docs/PaginationBaseRecipeSummary.md)
 - [PaginationBaseRecipeTag](docs/PaginationBaseRecipeTag.md)
 - [PaginationBaseRecipeTool](docs/PaginationBaseRecipeTool.md)
 - [PaginationBaseUserOut](docs/PaginationBaseUserOut.md)
 - [PaginationBaseUserSummary](docs/PaginationBaseUserSummary.md)
 - [ParsedIngredient](docs/ParsedIngredient.md)
 - [PasswordResetToken](docs/PasswordResetToken.md)
 - [PlanEntryPagination](docs/PlanEntryPagination.md)
 - [PlanEntryType](docs/PlanEntryType.md)
 - [PlanRulesCreate](docs/PlanRulesCreate.md)
 - [PlanRulesDay](docs/PlanRulesDay.md)
 - [PlanRulesOut](docs/PlanRulesOut.md)
 - [PlanRulesPagination](docs/PlanRulesPagination.md)
 - [PlanRulesType](docs/PlanRulesType.md)
 - [QueryFilterJSON](docs/QueryFilterJSON.md)
 - [QueryFilterJSONPart](docs/QueryFilterJSONPart.md)
 - [ReadCookBook](docs/ReadCookBook.md)
 - [ReadGroupPreferences](docs/ReadGroupPreferences.md)
 - [ReadHouseholdPreferences](docs/ReadHouseholdPreferences.md)
 - [ReadInviteToken](docs/ReadInviteToken.md)
 - [ReadPlanEntry](docs/ReadPlanEntry.md)
 - [ReadWebhook](docs/ReadWebhook.md)
 - [RecipeAsset](docs/RecipeAsset.md)
 - [RecipeCategory](docs/RecipeCategory.md)
 - [RecipeCategoryPagination](docs/RecipeCategoryPagination.md)
 - [RecipeCommentCreate](docs/RecipeCommentCreate.md)
 - [RecipeCommentOutInput](docs/RecipeCommentOutInput.md)
 - [RecipeCommentOutOutput](docs/RecipeCommentOutOutput.md)
 - [RecipeCommentPagination](docs/RecipeCommentPagination.md)
 - [RecipeCommentUpdate](docs/RecipeCommentUpdate.md)
 - [RecipeDuplicate](docs/RecipeDuplicate.md)
 - [RecipeIngredientInput](docs/RecipeIngredientInput.md)
 - [RecipeIngredientOutput](docs/RecipeIngredientOutput.md)
 - [RecipeInput](docs/RecipeInput.md)
 - [RecipeLastMade](docs/RecipeLastMade.md)
 - [RecipeNote](docs/RecipeNote.md)
 - [RecipeOutput](docs/RecipeOutput.md)
 - [RecipeSettings](docs/RecipeSettings.md)
 - [RecipeShareToken](docs/RecipeShareToken.md)
 - [RecipeShareTokenCreate](docs/RecipeShareTokenCreate.md)
 - [RecipeShareTokenSummary](docs/RecipeShareTokenSummary.md)
 - [RecipeStep](docs/RecipeStep.md)
 - [RecipeSuggestionResponse](docs/RecipeSuggestionResponse.md)
 - [RecipeSuggestionResponseItem](docs/RecipeSuggestionResponseItem.md)
 - [RecipeSummary](docs/RecipeSummary.md)
 - [RecipeTag](docs/RecipeTag.md)
 - [RecipeTagPagination](docs/RecipeTagPagination.md)
 - [RecipeTagResponse](docs/RecipeTagResponse.md)
 - [RecipeTimelineEventIn](docs/RecipeTimelineEventIn.md)
 - [RecipeTimelineEventOut](docs/RecipeTimelineEventOut.md)
 - [RecipeTimelineEventPagination](docs/RecipeTimelineEventPagination.md)
 - [RecipeTimelineEventUpdate](docs/RecipeTimelineEventUpdate.md)
 - [RecipeTool](docs/RecipeTool.md)
 - [RecipeToolCreate](docs/RecipeToolCreate.md)
 - [RecipeToolOut](docs/RecipeToolOut.md)
 - [RecipeToolPagination](docs/RecipeToolPagination.md)
 - [RecipeToolResponse](docs/RecipeToolResponse.md)
 - [RegisteredParser](docs/RegisteredParser.md)
 - [RelationalKeyword](docs/RelationalKeyword.md)
 - [RelationalOperator](docs/RelationalOperator.md)
 - [Relationaloperator](docs/Relationaloperator.md)
 - [ReportCategory](docs/ReportCategory.md)
 - [ReportEntryOut](docs/ReportEntryOut.md)
 - [ReportOut](docs/ReportOut.md)
 - [ReportSummary](docs/ReportSummary.md)
 - [ReportSummaryStatus](docs/ReportSummaryStatus.md)
 - [ResetPassword](docs/ResetPassword.md)
 - [SaveGroupRecipeAction](docs/SaveGroupRecipeAction.md)
 - [ScrapeRecipe](docs/ScrapeRecipe.md)
 - [ScrapeRecipeData](docs/ScrapeRecipeData.md)
 - [ScrapeRecipeTest](docs/ScrapeRecipeTest.md)
 - [SeederConfig](docs/SeederConfig.md)
 - [SetPermissions](docs/SetPermissions.md)
 - [ShoppingListAddRecipeParams](docs/ShoppingListAddRecipeParams.md)
 - [ShoppingListAddRecipeParamsBulk](docs/ShoppingListAddRecipeParamsBulk.md)
 - [ShoppingListCreate](docs/ShoppingListCreate.md)
 - [ShoppingListItemCreate](docs/ShoppingListItemCreate.md)
 - [ShoppingListItemOutInput](docs/ShoppingListItemOutInput.md)
 - [ShoppingListItemOutOutput](docs/ShoppingListItemOutOutput.md)
 - [ShoppingListItemPagination](docs/ShoppingListItemPagination.md)
 - [ShoppingListItemRecipeRefCreate](docs/ShoppingListItemRecipeRefCreate.md)
 - [ShoppingListItemRecipeRefOut](docs/ShoppingListItemRecipeRefOut.md)
 - [ShoppingListItemRecipeRefUpdate](docs/ShoppingListItemRecipeRefUpdate.md)
 - [ShoppingListItemUpdate](docs/ShoppingListItemUpdate.md)
 - [ShoppingListItemUpdateBulk](docs/ShoppingListItemUpdateBulk.md)
 - [ShoppingListItemUpdateRecipeReferencesInner](docs/ShoppingListItemUpdateRecipeReferencesInner.md)
 - [ShoppingListItemsCollectionOut](docs/ShoppingListItemsCollectionOut.md)
 - [ShoppingListMultiPurposeLabelOut](docs/ShoppingListMultiPurposeLabelOut.md)
 - [ShoppingListMultiPurposeLabelUpdate](docs/ShoppingListMultiPurposeLabelUpdate.md)
 - [ShoppingListOut](docs/ShoppingListOut.md)
 - [ShoppingListPagination](docs/ShoppingListPagination.md)
 - [ShoppingListRecipeRefOut](docs/ShoppingListRecipeRefOut.md)
 - [ShoppingListRemoveRecipeParams](docs/ShoppingListRemoveRecipeParams.md)
 - [ShoppingListSummary](docs/ShoppingListSummary.md)
 - [ShoppingListUpdate](docs/ShoppingListUpdate.md)
 - [SuccessResponse](docs/SuccessResponse.md)
 - [SupportedMigrations](docs/SupportedMigrations.md)
 - [TagBase](docs/TagBase.md)
 - [TagIn](docs/TagIn.md)
 - [TagOut](docs/TagOut.md)
 - [TimelineEventImage](docs/TimelineEventImage.md)
 - [TimelineEventType](docs/TimelineEventType.md)
 - [Unit](docs/Unit.md)
 - [Unit1](docs/Unit1.md)
 - [UnlockResults](docs/UnlockResults.md)
 - [UpdateCookBook](docs/UpdateCookBook.md)
 - [UpdateGroupPreferences](docs/UpdateGroupPreferences.md)
 - [UpdateHouseholdAdmin](docs/UpdateHouseholdAdmin.md)
 - [UpdateHouseholdPreferences](docs/UpdateHouseholdPreferences.md)
 - [UpdateImageResponse](docs/UpdateImageResponse.md)
 - [UpdatePlanEntry](docs/UpdatePlanEntry.md)
 - [UserIn](docs/UserIn.md)
 - [UserOut](docs/UserOut.md)
 - [UserPagination](docs/UserPagination.md)
 - [UserRatingOut](docs/UserRatingOut.md)
 - [UserRatingSummary](docs/UserRatingSummary.md)
 - [UserRatingUpdate](docs/UserRatingUpdate.md)
 - [UserRatingsUserRatingOut](docs/UserRatingsUserRatingOut.md)
 - [UserRatingsUserRatingSummary](docs/UserRatingsUserRatingSummary.md)
 - [UserSummary](docs/UserSummary.md)
 - [UsernameOrId](docs/UsernameOrId.md)
 - [ValidationError](docs/ValidationError.md)
 - [ValidationErrorLocInner](docs/ValidationErrorLocInner.md)
 - [Value](docs/Value.md)
 - [WebhookPagination](docs/WebhookPagination.md)
 - [WebhookType](docs/WebhookType.md)


<a id="documentation-for-authorization"></a>
## Documentation For Authorization


Authentication schemes defined for the API:
<a id="OAuth2PasswordBearer"></a>
### OAuth2PasswordBearer

- **Type**: OAuth
- **Flow**: password
- **Authorization URL**: 
- **Scopes**: N/A

