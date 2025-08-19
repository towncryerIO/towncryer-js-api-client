# SendEmailPayload


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | **string** |  | [optional] [default to undefined]
**from** | [**EmailFrom**](EmailFrom.md) |  | [optional] [default to undefined]
**recipients** | [**Array&lt;EmailRecipient&gt;**](EmailRecipient.md) |  | [default to undefined]
**templateId** | **string** |  | [optional] [default to undefined]
**title** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { SendEmailPayload } from '@towncryer-dev/towncryer-sdk-api-client';

const instance: SendEmailPayload = {
    content,
    from,
    recipients,
    templateId,
    title,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
