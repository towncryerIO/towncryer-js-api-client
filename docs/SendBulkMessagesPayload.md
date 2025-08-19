# SendBulkMessagesPayload


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**emails** | [**Array&lt;SendEmailPayload&gt;**](SendEmailPayload.md) |  | [optional] [default to undefined]
**pushNotifications** | [**Array&lt;SendPushNotificationPayload&gt;**](SendPushNotificationPayload.md) |  | [optional] [default to undefined]
**smses** | [**Array&lt;SendSMSPayload&gt;**](SendSMSPayload.md) |  | [optional] [default to undefined]

## Example

```typescript
import { SendBulkMessagesPayload } from '@towncryer-dev/towncryer-sdk-api-client';

const instance: SendBulkMessagesPayload = {
    emails,
    pushNotifications,
    smses,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
