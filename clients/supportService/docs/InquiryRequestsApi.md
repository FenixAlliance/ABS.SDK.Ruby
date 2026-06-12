# OpenapiClient::InquiryRequestsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_inquiry_request_async**](InquiryRequestsApi.md#create_inquiry_request_async) | **POST** /api/v2/SupportService/InquiryRequests | Create an inquiry request |
| [**delete_inquiry_request_async**](InquiryRequestsApi.md#delete_inquiry_request_async) | **DELETE** /api/v2/SupportService/InquiryRequests/{inquiryRequestId} | Delete an inquiry request |
| [**get_inquiry_request_async**](InquiryRequestsApi.md#get_inquiry_request_async) | **GET** /api/v2/SupportService/InquiryRequests/{inquiryRequestId} | Retrieve an inquiry request by ID |
| [**get_inquiry_requests_async**](InquiryRequestsApi.md#get_inquiry_requests_async) | **GET** /api/v2/SupportService/InquiryRequests | Retrieve inquiry requests |
| [**get_inquiry_requests_count_async**](InquiryRequestsApi.md#get_inquiry_requests_count_async) | **GET** /api/v2/SupportService/InquiryRequests/Count | Get inquiry requests count |
| [**patch_inquiry_request_async**](InquiryRequestsApi.md#patch_inquiry_request_async) | **PATCH** /api/v2/SupportService/InquiryRequests/{inquiryRequestId} | Patch an inquiry request |
| [**update_inquiry_request_async**](InquiryRequestsApi.md#update_inquiry_request_async) | **PUT** /api/v2/SupportService/InquiryRequests/{inquiryRequestId} | Update an inquiry request |


## create_inquiry_request_async

> <EmptyEnvelope> create_inquiry_request_async(tenant_id, opts)

Create an inquiry request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InquiryRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  inquiry_request_create_dto: OpenapiClient::InquiryRequestCreateDto.new({name: 'name_example', email: 'email_example', message: 'message_example'}) # InquiryRequestCreateDto | 
}

begin
  # Create an inquiry request
  result = api_instance.create_inquiry_request_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InquiryRequestsApi->create_inquiry_request_async: #{e}"
end
```

#### Using the create_inquiry_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_inquiry_request_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create an inquiry request
  data, status_code, headers = api_instance.create_inquiry_request_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InquiryRequestsApi->create_inquiry_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **inquiry_request_create_dto** | [**InquiryRequestCreateDto**](InquiryRequestCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_inquiry_request_async

> <EmptyEnvelope> delete_inquiry_request_async(tenant_id, inquiry_request_id, opts)

Delete an inquiry request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InquiryRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
inquiry_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an inquiry request
  result = api_instance.delete_inquiry_request_async(tenant_id, inquiry_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InquiryRequestsApi->delete_inquiry_request_async: #{e}"
end
```

#### Using the delete_inquiry_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_inquiry_request_async_with_http_info(tenant_id, inquiry_request_id, opts)

```ruby
begin
  # Delete an inquiry request
  data, status_code, headers = api_instance.delete_inquiry_request_async_with_http_info(tenant_id, inquiry_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InquiryRequestsApi->delete_inquiry_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **inquiry_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_inquiry_request_async

> <InquiryRequestDtoEnvelope> get_inquiry_request_async(tenant_id, inquiry_request_id, opts)

Retrieve an inquiry request by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InquiryRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
inquiry_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve an inquiry request by ID
  result = api_instance.get_inquiry_request_async(tenant_id, inquiry_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InquiryRequestsApi->get_inquiry_request_async: #{e}"
end
```

#### Using the get_inquiry_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InquiryRequestDtoEnvelope>, Integer, Hash)> get_inquiry_request_async_with_http_info(tenant_id, inquiry_request_id, opts)

```ruby
begin
  # Retrieve an inquiry request by ID
  data, status_code, headers = api_instance.get_inquiry_request_async_with_http_info(tenant_id, inquiry_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InquiryRequestDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InquiryRequestsApi->get_inquiry_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **inquiry_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**InquiryRequestDtoEnvelope**](InquiryRequestDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_inquiry_requests_async

> <InquiryRequestDtoListEnvelope> get_inquiry_requests_async(tenant_id, opts)

Retrieve inquiry requests

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InquiryRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve inquiry requests
  result = api_instance.get_inquiry_requests_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InquiryRequestsApi->get_inquiry_requests_async: #{e}"
end
```

#### Using the get_inquiry_requests_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InquiryRequestDtoListEnvelope>, Integer, Hash)> get_inquiry_requests_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve inquiry requests
  data, status_code, headers = api_instance.get_inquiry_requests_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InquiryRequestDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InquiryRequestsApi->get_inquiry_requests_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**InquiryRequestDtoListEnvelope**](InquiryRequestDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_inquiry_requests_count_async

> <Int32Envelope> get_inquiry_requests_count_async(tenant_id, opts)

Get inquiry requests count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InquiryRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get inquiry requests count
  result = api_instance.get_inquiry_requests_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InquiryRequestsApi->get_inquiry_requests_count_async: #{e}"
end
```

#### Using the get_inquiry_requests_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_inquiry_requests_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get inquiry requests count
  data, status_code, headers = api_instance.get_inquiry_requests_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InquiryRequestsApi->get_inquiry_requests_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_inquiry_request_async

> <EmptyEnvelope> patch_inquiry_request_async(tenant_id, inquiry_request_id, opts)

Patch an inquiry request

Partially updates an existing inquiry request by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InquiryRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
inquiry_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch an inquiry request
  result = api_instance.patch_inquiry_request_async(tenant_id, inquiry_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InquiryRequestsApi->patch_inquiry_request_async: #{e}"
end
```

#### Using the patch_inquiry_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_inquiry_request_async_with_http_info(tenant_id, inquiry_request_id, opts)

```ruby
begin
  # Patch an inquiry request
  data, status_code, headers = api_instance.patch_inquiry_request_async_with_http_info(tenant_id, inquiry_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InquiryRequestsApi->patch_inquiry_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **inquiry_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_inquiry_request_async

> <EmptyEnvelope> update_inquiry_request_async(tenant_id, inquiry_request_id, opts)

Update an inquiry request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InquiryRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
inquiry_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  inquiry_request_update_dto: OpenapiClient::InquiryRequestUpdateDto.new # InquiryRequestUpdateDto | 
}

begin
  # Update an inquiry request
  result = api_instance.update_inquiry_request_async(tenant_id, inquiry_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InquiryRequestsApi->update_inquiry_request_async: #{e}"
end
```

#### Using the update_inquiry_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_inquiry_request_async_with_http_info(tenant_id, inquiry_request_id, opts)

```ruby
begin
  # Update an inquiry request
  data, status_code, headers = api_instance.update_inquiry_request_async_with_http_info(tenant_id, inquiry_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InquiryRequestsApi->update_inquiry_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **inquiry_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **inquiry_request_update_dto** | [**InquiryRequestUpdateDto**](InquiryRequestUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

