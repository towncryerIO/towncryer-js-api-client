# SendPushNotificationPayload


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | **string** |  | [optional] [default to undefined]
**data** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**recipients** | [**Array&lt;SendPushNotificationRecipient&gt;**](SendPushNotificationRecipient.md) |  | [default to undefined]
**templateId** | **string** |  | [optional] [default to undefined]
**title** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { SendPushNotificationPayload } from '@towncryer-dev/towncryer-sdk-api-client';

const instance: SendPushNotificationPayload = {
    content,
    data,
    recipients,
    templateId,
    title,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
