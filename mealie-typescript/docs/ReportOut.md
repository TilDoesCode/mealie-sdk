# ReportOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**timestamp** | **string** |  | [optional] [default to undefined]
**category** | [**ReportCategory**](ReportCategory.md) |  | [default to undefined]
**groupId** | **string** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**status** | [**ReportSummaryStatus**](ReportSummaryStatus.md) |  | [optional] [default to undefined]
**id** | **string** |  | [default to undefined]
**entries** | [**Array&lt;ReportEntryOut&gt;**](ReportEntryOut.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ReportOut } from 'mealie-typescript';

const instance: ReportOut = {
    timestamp,
    category,
    groupId,
    name,
    status,
    id,
    entries,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
