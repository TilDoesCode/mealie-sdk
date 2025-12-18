# RecipeTimelineEventOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**recipeId** | **string** |  | [default to undefined]
**userId** | **string** |  | [default to undefined]
**subject** | **string** |  | [default to undefined]
**eventType** | [**TimelineEventType**](TimelineEventType.md) |  | [default to undefined]
**eventMessage** | **string** |  | [optional] [default to undefined]
**image** | [**TimelineEventImage**](TimelineEventImage.md) |  | [optional] [default to undefined]
**timestamp** | **string** |  | [optional] [default to 2025-12-17T04:03:15.942492Z]
**id** | **string** |  | [default to undefined]
**groupId** | **string** |  | [default to undefined]
**householdId** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]

## Example

```typescript
import { RecipeTimelineEventOut } from 'mealie-typescript';

const instance: RecipeTimelineEventOut = {
    recipeId,
    userId,
    subject,
    eventType,
    eventMessage,
    image,
    timestamp,
    id,
    groupId,
    householdId,
    createdAt,
    updatedAt,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
