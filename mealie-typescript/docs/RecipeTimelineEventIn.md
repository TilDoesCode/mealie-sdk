# RecipeTimelineEventIn


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**recipeId** | **string** |  | [default to undefined]
**userId** | **string** |  | [optional] [default to undefined]
**subject** | **string** |  | [default to undefined]
**eventType** | [**TimelineEventType**](TimelineEventType.md) |  | [default to undefined]
**eventMessage** | **string** |  | [optional] [default to undefined]
**image** | [**TimelineEventImage**](TimelineEventImage.md) |  | [optional] [default to undefined]
**timestamp** | **string** |  | [optional] [default to 2025-12-28T23:41:18.020568Z]

## Example

```typescript
import { RecipeTimelineEventIn } from 'mealie-typescript';

const instance: RecipeTimelineEventIn = {
    recipeId,
    userId,
    subject,
    eventType,
    eventMessage,
    image,
    timestamp,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
