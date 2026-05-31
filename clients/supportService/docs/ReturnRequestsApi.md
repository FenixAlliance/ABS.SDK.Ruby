# OpenapiClient::ReturnRequestsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_return_request_async**](ReturnRequestsApi.md#create_return_request_async) | **POST** /api/v2/SupportService/ReturnRequests | Create a return request |
| [**delete_return_request_async**](ReturnRequestsApi.md#delete_return_request_async) | **DELETE** /api/v2/SupportService/ReturnRequests/{returnRequestId} | Delete a return request |
| [**get_return_request_async**](ReturnRequestsApi.md#get_return_request_async) | **GET** /api/v2/SupportService/ReturnRequests/{returnRequestId} | Retrieve a return request by ID |
| [**get_return_requests_async**](ReturnRequestsApi.md#get_return_requests_async) | **GET** /api/v2/SupportService/ReturnRequests | Retrieve return requests |
| [**get_return_requests_count_async**](ReturnRequestsApi.md#get_return_requests_count_async) | **GET** /api/v2/SupportService/ReturnRequests/Count | Get return requests count |
| [**update_return_request_async**](ReturnRequestsApi.md#update_return_request_async) | **PUT** /api/v2/SupportService/ReturnRequests/{returnRequestId} | Update a return request |


## create_return_request_async

> <EmptyEnvelope> create_return_request_async(tenant_id, opts)

Create a return request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReturnRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  return_request_create_dto: OpenapiClient::ReturnRequestCreateDto.new({title: 'title_example'}) # ReturnRequestCreateDto | 
}

begin
  # Create a return request
  result = api_instance.create_return_request_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnRequestsApi->create_return_request_async: #{e}"
end
```

#### Using the create_return_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_return_request_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a return request
  data, status_code, headers = api_instance.create_return_request_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnRequestsApi->create_return_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **return_request_create_dto** | [**ReturnRequestCreateDto**](ReturnRequestCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_return_request_async

> <EmptyEnvelope> delete_return_request_async(tenant_id, return_request_id, opts)

Delete a return request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReturnRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
return_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a return request
  result = api_instance.delete_return_request_async(tenant_id, return_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnRequestsApi->delete_return_request_async: #{e}"
end
```

#### Using the delete_return_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_return_request_async_with_http_info(tenant_id, return_request_id, opts)

```ruby
begin
  # Delete a return request
  data, status_code, headers = api_instance.delete_return_request_async_with_http_info(tenant_id, return_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnRequestsApi->delete_return_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **return_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_return_request_async

> <ReturnRequestDtoEnvelope> get_return_request_async(tenant_id, return_request_id, opts)

Retrieve a return request by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReturnRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
return_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a return request by ID
  result = api_instance.get_return_request_async(tenant_id, return_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnRequestsApi->get_return_request_async: #{e}"
end
```

#### Using the get_return_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ReturnRequestDtoEnvelope>, Integer, Hash)> get_return_request_async_with_http_info(tenant_id, return_request_id, opts)

```ruby
begin
  # Retrieve a return request by ID
  data, status_code, headers = api_instance.get_return_request_async_with_http_info(tenant_id, return_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ReturnRequestDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnRequestsApi->get_return_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **return_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ReturnRequestDtoEnvelope**](ReturnRequestDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_return_requests_async

> <ReturnRequestDtoListEnvelope> get_return_requests_async(tenant_id, opts)

Retrieve return requests

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReturnRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve return requests
  result = api_instance.get_return_requests_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnRequestsApi->get_return_requests_async: #{e}"
end
```

#### Using the get_return_requests_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ReturnRequestDtoListEnvelope>, Integer, Hash)> get_return_requests_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve return requests
  data, status_code, headers = api_instance.get_return_requests_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ReturnRequestDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnRequestsApi->get_return_requests_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ReturnRequestDtoListEnvelope**](ReturnRequestDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_return_requests_count_async

> <Int32Envelope> get_return_requests_count_async(tenant_id, opts)

Get return requests count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReturnRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get return requests count
  result = api_instance.get_return_requests_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnRequestsApi->get_return_requests_count_async: #{e}"
end
```

#### Using the get_return_requests_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_return_requests_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get return requests count
  data, status_code, headers = api_instance.get_return_requests_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnRequestsApi->get_return_requests_count_async_with_http_info: #{e}"
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


## update_return_request_async

> <EmptyEnvelope> update_return_request_async(tenant_id, return_request_id, opts)

Update a return request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReturnRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
return_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  return_request_update_dto: OpenapiClient::ReturnRequestUpdateDto.new # ReturnRequestUpdateDto | 
}

begin
  # Update a return request
  result = api_instance.update_return_request_async(tenant_id, return_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnRequestsApi->update_return_request_async: #{e}"
end
```

#### Using the update_return_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_return_request_async_with_http_info(tenant_id, return_request_id, opts)

```ruby
begin
  # Update a return request
  data, status_code, headers = api_instance.update_return_request_async_with_http_info(tenant_id, return_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnRequestsApi->update_return_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **return_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **return_request_update_dto** | [**ReturnRequestUpdateDto**](ReturnRequestUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

