## @towncryer-dev/towncryer-sdk-api-client@1.0

This generator creates TypeScript/JavaScript client that utilizes [axios](https://github.com/axios/axios). The generated Node module can be used in the following environments:

Environment
* Node.js
* Webpack
* Browserify

Language level
* ES5 - you must have a Promises/A+ library installed
* ES6

Module system
* CommonJS
* ES6 module system

It can be used in both TypeScript and JavaScript. In TypeScript, the definition will be automatically resolved via `package.json`. ([Reference](https://www.typescriptlang.org/docs/handbook/declaration-files/consumption.html))

### Building

To build and compile the typescript sources to javascript use:
```
npm install
npm run build
```

### Publishing

First build the package then run `npm publish`

### Consuming

navigate to the folder of your consuming project and run one of the following commands.

_published:_

```
npm install @towncryer-dev/towncryer-sdk-api-client@1.0 --save
```

_unPublished (not recommended):_

```
npm install PATH_TO_GENERATED_PACKAGE --save
```

### Documentation for API Endpoints

All URIs are relative to *http://localhost:8888/api/v1*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AuthApi* | [**clientAppLogin**](docs/AuthApi.md#clientapplogin) | **POST** /auth/authorize/client | Client App Login
*AuthApi* | [**getShortLivedToken**](docs/AuthApi.md#getshortlivedtoken) | **POST** /auth/authorize | Get Short Lived Token
*AuthApi* | [**refreshShortLivedToken**](docs/AuthApi.md#refreshshortlivedtoken) | **POST** /auth/refresh-token | Refresh Short Lived Token
*CustomersApi* | [**createCustomer**](docs/CustomersApi.md#createcustomer) | **POST** /customers | Create Customer
*EventsApi* | [**accept**](docs/EventsApi.md#accept) | **POST** /events | Accept Event
*MessagesApi* | [**getCustomerMessagesStats**](docs/MessagesApi.md#getcustomermessagesstats) | **GET** /customers/{customerId}/messages/stats | Get customer\&#39;s messages stats
*MessagesApi* | [**listMessagesByCustomerAndChannel**](docs/MessagesApi.md#listmessagesbycustomerandchannel) | **GET** /customers/{customerId}/messages | List customer\&#39;s messages filtering by channel
*MessagesApi* | [**markMessageAsRead**](docs/MessagesApi.md#markmessageasread) | **PUT** /messages/{id}/read | Mark Message As Read
*MessagesApi* | [**sendMessage**](docs/MessagesApi.md#sendmessage) | **POST** /messages | Send Message


### Documentation For Models

 - [APICredentialsLoginPayload](docs/APICredentialsLoginPayload.md)
 - [APICredentialsLoginResponse](docs/APICredentialsLoginResponse.md)
 - [ApiError](docs/ApiError.md)
 - [ApiResponse](docs/ApiResponse.md)
 - [CreateCustomerRequest](docs/CreateCustomerRequest.md)
 - [CustomerIdentityRequest](docs/CustomerIdentityRequest.md)
 - [EmailFrom](docs/EmailFrom.md)
 - [EmailRecipient](docs/EmailRecipient.md)
 - [EntitiesIdentityType](docs/EntitiesIdentityType.md)
 - [EventCustomerRequest](docs/EventCustomerRequest.md)
 - [MessagesStats](docs/MessagesStats.md)
 - [PaginatePage](docs/PaginatePage.md)
 - [PublishEventPayload](docs/PublishEventPayload.md)
 - [RefreshTokenRequest](docs/RefreshTokenRequest.md)
 - [RequestsClientAppLoginPayload](docs/RequestsClientAppLoginPayload.md)
 - [ResponsesClientAppLoginResponsePayload](docs/ResponsesClientAppLoginResponsePayload.md)
 - [ScheduleInfo](docs/ScheduleInfo.md)
 - [SendBulkMessagesPayload](docs/SendBulkMessagesPayload.md)
 - [SendEmailPayload](docs/SendEmailPayload.md)
 - [SendPushNotificationPayload](docs/SendPushNotificationPayload.md)
 - [SendPushNotificationRecipient](docs/SendPushNotificationRecipient.md)
 - [SendSMSPayload](docs/SendSMSPayload.md)
 - [SendSMSRecipient](docs/SendSMSRecipient.md)
 - [TypesChannelCustomerCreatedFrom](docs/TypesChannelCustomerCreatedFrom.md)
 - [TypesJobStatus](docs/TypesJobStatus.md)


<a id="documentation-for-authorization"></a>
## Documentation For Authorization


Authentication schemes defined for the API:
<a id="ApiKeyAuth"></a>
### ApiKeyAuth

- **Type**: API key
- **API key parameter name**: X-API-KEY
- **Location**: HTTP header

<a id="ApiSecretAuth"></a>
### ApiSecretAuth

- **Type**: API key
- **API key parameter name**: X-API-SECRET
- **Location**: HTTP header

<a id="BearerAuth"></a>
### BearerAuth

- **Type**: API key
- **API key parameter name**: Authorization
- **Location**: HTTP header

