# OpenapiClient::RefundRequestsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_refund_request_async**](RefundRequestsApi.md#create_refund_request_async) | **POST** /api/v2/SupportService/RefundRequests | Create a refund request |
| [**delete_refund_request_async**](RefundRequestsApi.md#delete_refund_request_async) | **DELETE** /api/v2/SupportService/RefundRequests/{refundRequestId} | Delete a refund request |
| [**get_refund_request_async**](RefundRequestsApi.md#get_refund_request_async) | **GET** /api/v2/SupportService/RefundRequests/{refundRequestId} | Retrieve a refund request by ID |
| [**get_refund_requests_async**](RefundRequestsApi.md#get_refund_requests_async) | **GET** /api/v2/SupportService/RefundRequests | Retrieve refund requests |
| [**get_refund_requests_count_async**](RefundRequestsApi.md#get_refund_requests_count_async) | **GET** /api/v2/SupportService/RefundRequests/Count | Get refund requests count |
| [**update_refund_request_async**](RefundRequestsApi.md#update_refund_request_async) | **PUT** /api/v2/SupportService/RefundRequests/{refundRequestId} | Update a refund request |


## create_refund_request_async

> <EmptyEnvelope> create_refund_request_async(tenant_id, opts)

Create a refund request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RefundRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  refund_request_create_dto: OpenapiClient::RefundRequestCreateDto.new({title: 'title_example'}) # RefundRequestCreateDto | 
}

begin
  # Create a refund request
  result = api_instance.create_refund_request_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundRequestsApi->create_refund_request_async: #{e}"
end
```

#### Using the create_refund_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_refund_request_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a refund request
  data, status_code, headers = api_instance.create_refund_request_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundRequestsApi->create_refund_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **refund_request_create_dto** | [**RefundRequestCreateDto**](RefundRequestCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_refund_request_async

> <EmptyEnvelope> delete_refund_request_async(tenant_id, refund_request_id, opts)

Delete a refund request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RefundRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
refund_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a refund request
  result = api_instance.delete_refund_request_async(tenant_id, refund_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundRequestsApi->delete_refund_request_async: #{e}"
end
```

#### Using the delete_refund_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_refund_request_async_with_http_info(tenant_id, refund_request_id, opts)

```ruby
begin
  # Delete a refund request
  data, status_code, headers = api_instance.delete_refund_request_async_with_http_info(tenant_id, refund_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundRequestsApi->delete_refund_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **refund_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_refund_request_async

> <RefundRequestDtoEnvelope> get_refund_request_async(tenant_id, refund_request_id, opts)

Retrieve a refund request by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RefundRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
refund_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a refund request by ID
  result = api_instance.get_refund_request_async(tenant_id, refund_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundRequestsApi->get_refund_request_async: #{e}"
end
```

#### Using the get_refund_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<RefundRequestDtoEnvelope>, Integer, Hash)> get_refund_request_async_with_http_info(tenant_id, refund_request_id, opts)

```ruby
begin
  # Retrieve a refund request by ID
  data, status_code, headers = api_instance.get_refund_request_async_with_http_info(tenant_id, refund_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <RefundRequestDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundRequestsApi->get_refund_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **refund_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**RefundRequestDtoEnvelope**](RefundRequestDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_refund_requests_async

> <RefundRequestDtoListEnvelope> get_refund_requests_async(tenant_id, opts)

Retrieve refund requests

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RefundRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve refund requests
  result = api_instance.get_refund_requests_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundRequestsApi->get_refund_requests_async: #{e}"
end
```

#### Using the get_refund_requests_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<RefundRequestDtoListEnvelope>, Integer, Hash)> get_refund_requests_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve refund requests
  data, status_code, headers = api_instance.get_refund_requests_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <RefundRequestDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundRequestsApi->get_refund_requests_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**RefundRequestDtoListEnvelope**](RefundRequestDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_refund_requests_count_async

> <Int32Envelope> get_refund_requests_count_async(tenant_id, opts)

Get refund requests count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RefundRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get refund requests count
  result = api_instance.get_refund_requests_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundRequestsApi->get_refund_requests_count_async: #{e}"
end
```

#### Using the get_refund_requests_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_refund_requests_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get refund requests count
  data, status_code, headers = api_instance.get_refund_requests_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundRequestsApi->get_refund_requests_count_async_with_http_info: #{e}"
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


## update_refund_request_async

> <EmptyEnvelope> update_refund_request_async(tenant_id, refund_request_id, opts)

Update a refund request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RefundRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
refund_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  refund_request_update_dto: OpenapiClient::RefundRequestUpdateDto.new # RefundRequestUpdateDto | 
}

begin
  # Update a refund request
  result = api_instance.update_refund_request_async(tenant_id, refund_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundRequestsApi->update_refund_request_async: #{e}"
end
```

#### Using the update_refund_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_refund_request_async_with_http_info(tenant_id, refund_request_id, opts)

```ruby
begin
  # Update a refund request
  data, status_code, headers = api_instance.update_refund_request_async_with_http_info(tenant_id, refund_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundRequestsApi->update_refund_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **refund_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **refund_request_update_dto** | [**RefundRequestUpdateDto**](RefundRequestUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

