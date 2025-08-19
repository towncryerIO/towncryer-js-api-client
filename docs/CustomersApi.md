# CustomersApi

All URIs are relative to *http://localhost:8888/api/v1*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createCustomer**](#createcustomer) | **POST** /customers | Create Customer|

# **createCustomer**
> ApiResponse createCustomer(request)

Creates a customer

### Example

```typescript
import {
    CustomersApi,
    Configuration,
    CreateCustomerRequest
} from '@towncryer-dev/towncryer-sdk-api-client';

const configuration = new Configuration();
const apiInstance = new CustomersApi(configuration);

let request: CreateCustomerRequest; //Create customer request

const { status, data } = await apiInstance.createCustomer(
    request
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **request** | **CreateCustomerRequest**| Create customer request | |


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
|**200** | OK |  -  |
|**400** | Bad Request |  -  |
|**401** | Unauthorized |  -  |
|**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

