# CreateWebhook


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **boolean** |  | [optional] [default to true]
**name** | **string** |  | [optional] [default to '']
**url** | **string** |  | [optional] [default to '']
**webhookType** | [**WebhookType**](WebhookType.md) |  | [optional] [default to undefined]
**scheduledTime** | **string** |  | [default to undefined]

## Example

```typescript
import { CreateWebhook } from 'mealie-typescript';

const instance: CreateWebhook = {
    enabled,
    name,
    url,
    webhookType,
    scheduledTime,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
