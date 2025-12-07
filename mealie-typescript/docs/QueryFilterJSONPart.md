# QueryFilterJSONPart


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**leftParenthesis** | **string** |  | [optional] [default to undefined]
**rightParenthesis** | **string** |  | [optional] [default to undefined]
**logicalOperator** | [**LogicalOperator**](LogicalOperator.md) |  | [optional] [default to undefined]
**attributeName** | **string** |  | [optional] [default to undefined]
**relationalOperator** | [**Relationaloperator**](Relationaloperator.md) |  | [optional] [default to undefined]
**value** | [**Value**](Value.md) |  | [optional] [default to undefined]

## Example

```typescript
import { QueryFilterJSONPart } from 'mealie-typescript';

const instance: QueryFilterJSONPart = {
    leftParenthesis,
    rightParenthesis,
    logicalOperator,
    attributeName,
    relationalOperator,
    value,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
