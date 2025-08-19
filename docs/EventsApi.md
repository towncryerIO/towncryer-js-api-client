# EventsApi

All URIs are relative to *http://localhost:8888/api/v1*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**accept**](#accept) | **POST** /events | Accept Event|

# **accept**
> ApiResponse accept(request)

Accepts an event

### Example

```typescript
import {
    EventsApi,
    Configuration,
    PublishEventPayload
} from '@towncryer-dev/towncryer-sdk-api-client';

const configuration = new Configuration();
const apiInstance = new EventsApi(configuration);

let request: PublishEventPayload; //Event request

const { status, data } = await apiInstance.accept(
    request
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **request** | **PublishEventPayload**| Event request | |


### Return type

**ApiResponse**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**202** | Accepted |  -  |
|**400** | Bad Request |  -  |
|**401** | Unauthorized |  -  |
|**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

