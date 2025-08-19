# AuthApi

All URIs are relative to *http://localhost:8888/api/v1*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**clientAppLogin**](#clientapplogin) | **POST** /auth/authorize/client | Client App Login|
|[**getShortLivedToken**](#getshortlivedtoken) | **POST** /auth/authorize | Get Short Lived Token|
|[**refreshShortLivedToken**](#refreshshortlivedtoken) | **POST** /auth/refresh-token | Refresh Short Lived Token|

# **clientAppLogin**
> ResponsesClientAppLoginResponsePayload clientAppLogin(request)

Logs in a client app using client app credentials

### Example

```typescript
import {
    AuthApi,
    Configuration,
    RequestsClientAppLoginPayload
} from '@towncryer-dev/towncryer-sdk-api-client';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

let request: RequestsClientAppLoginPayload; //Client app login request

const { status, data } = await apiInstance.clientAppLogin(
    request
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **request** | **RequestsClientAppLoginPayload**| Client app login request | |


### Return type

**ResponsesClientAppLoginResponsePayload**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |
|**400** | Bad Request |  -  |
|**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getShortLivedToken**
> APICredentialsLoginResponse getShortLivedToken(request)

Gets a short lived token using ApiKey and ApiSecret

### Example

```typescript
import {
    AuthApi,
    Configuration,
    APICredentialsLoginPayload
} from '@towncryer-dev/towncryer-sdk-api-client';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

let request: APICredentialsLoginPayload; //Login request

const { status, data } = await apiInstance.getShortLivedToken(
    request
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **request** | **APICredentialsLoginPayload**| Login request | |


### Return type

**APICredentialsLoginResponse**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |
|**400** | Bad Request |  -  |
|**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **refreshShortLivedToken**
> APICredentialsLoginResponse refreshShortLivedToken(request)

Refreshes a short lived token

### Example

```typescript
import {
    AuthApi,
    Configuration,
    RefreshTokenRequest
} from '@towncryer-dev/towncryer-sdk-api-client';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

let request: RefreshTokenRequest; //Refresh token request

const { status, data } = await apiInstance.refreshShortLivedToken(
    request
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **request** | **RefreshTokenRequest**| Refresh token request | |


### Return type

**APICredentialsLoginResponse**

### Authorization

No authorization required

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

