# SendSMSPayload


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | **string** |  | [optional] [default to undefined]
**from** | **string** |  | [default to undefined]
**templateId** | **string** |  | [optional] [default to undefined]
**to** | [**Array&lt;SendSMSRecipient&gt;**](SendSMSRecipient.md) |  | [default to undefined]

## Example

```typescript
import { SendSMSPayload } from '@towncryer-dev/towncryer-sdk-api-client';

const instance: SendSMSPayload = {
    content,
    from,
    templateId,
    to,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
