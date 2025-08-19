# CreateCustomerRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**externalId** | **string** |  | [optional] [default to undefined]
**firstName** | **string** |  | [optional] [default to undefined]
**identities** | [**Array&lt;CustomerIdentityRequest&gt;**](CustomerIdentityRequest.md) |  | [default to undefined]
**lastName** | **string** |  | [optional] [default to undefined]
**source** | [**TypesChannelCustomerCreatedFrom**](TypesChannelCustomerCreatedFrom.md) |  | [default to undefined]

## Example

```typescript
import { CreateCustomerRequest } from '@towncryer-dev/towncryer-sdk-api-client';

const instance: CreateCustomerRequest = {
    externalId,
    firstName,
    identities,
    lastName,
    source,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
