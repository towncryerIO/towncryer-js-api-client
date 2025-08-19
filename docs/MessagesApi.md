# MessagesApi

All URIs are relative to *http://localhost:8888/api/v1*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getCustomerMessagesStats**](#getcustomermessagesstats) | **GET** /customers/{customerId}/messages/stats | Get customer\&#39;s messages stats|
|[**listMessagesByCustomerAndChannel**](#listmessagesbycustomerandchannel) | **GET** /customers/{customerId}/messages | List customer\&#39;s messages filtering by channel|
|[**markMessageAsRead**](#markmessageasread) | **PUT** /messages/{id}/read | Mark Message As Read|
|[**sendMessage**](#sendmessage) | **POST** /messages | Send Message|

# **getCustomerMessagesStats**
> MessagesStats getCustomerMessagesStats()

Get customer\'s messages stats while optionally filtering by channel

### Example

```typescript
import {
    MessagesApi,
    Configuration
} from '@towncryer-dev/towncryer-sdk-api-client';

const configuration = new Configuration();
const apiInstance = new MessagesApi(configuration);

let customerId: string; //Customer ID (default to undefined)
let channel: string; //Channel (optional) (default to undefined)

const { status, data } = await apiInstance.getCustomerMessagesStats(
    customerId,
    channel
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer ID | defaults to undefined|
| **channel** | [**string**] | Channel | (optional) defaults to undefined|


### Return type

**MessagesStats**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |
|**400** | Bad Request |  -  |
|**401** | Unauthorized |  -  |
|**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **listMessagesByCustomerAndChannel**
> PaginatePage listMessagesByCustomerAndChannel()

List customer\'s messages while optionally filtering by channel

### Example

```typescript
import {
    MessagesApi,
    Configuration
} from '@towncryer-dev/towncryer-sdk-api-client';

const configuration = new Configuration();
const apiInstance = new MessagesApi(configuration);

let customerId: string; //Customer ID (default to undefined)
let channel: string; //Channel (optional) (default to undefined)
let page: number; //Page number (optional) (default to undefined)
let size: number; //Page size (optional) (default to undefined)

const { status, data } = await apiInstance.listMessagesByCustomerAndChannel(
    customerId,
    channel,
    page,
    size
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer ID | defaults to undefined|
| **channel** | [**string**] | Channel | (optional) defaults to undefined|
| **page** | [**number**] | Page number | (optional) defaults to undefined|
| **size** | [**number**] | Page size | (optional) defaults to undefined|


### Return type

**PaginatePage**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |
|**400** | Bad Request |  -  |
|**401** | Unauthorized |  -  |
|**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **markMessageAsRead**
> ApiResponse markMessageAsRead()

Marks a message as read

### Example

```typescript
import {
    MessagesApi,
    Configuration
} from '@towncryer-dev/towncryer-sdk-api-client';

const configuration = new Configuration();
const apiInstance = new MessagesApi(configuration);

let id: string; //Message ID (default to undefined)

const { status, data } = await apiInstance.markMessageAsRead(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | Message ID | defaults to undefined|


### Return type

**ApiResponse**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |
|**400** | Bad Request |  -  |
|**401** | Unauthorized |  -  |
|**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **sendMessage**
> ScheduleInfo sendMessage(request)

Sends a message

### Example

```typescript
import {
    MessagesApi,
    Configuration,
    SendBulkMessagesPayload
} from '@towncryer-dev/towncryer-sdk-api-client';

const configuration = new Configuration();
const apiInstance = new MessagesApi(configuration);

let request: SendBulkMessagesPayload; //Send bulk messages payload

const { status, data } = await apiInstance.sendMessage(
    request
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **request** | **SendBulkMessagesPayload**| Send bulk messages payload | |


### Return type

**ScheduleInfo**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |
|**400** | Bad Request |  -  |
|**401** | Unauthorized |  -  |
|**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

