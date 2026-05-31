# OpenapiClient::WarrantyRequestsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_warranty_request_async**](WarrantyRequestsApi.md#create_warranty_request_async) | **POST** /api/v2/SupportService/WarrantyRequests | Create a warranty request |
| [**delete_warranty_request_async**](WarrantyRequestsApi.md#delete_warranty_request_async) | **DELETE** /api/v2/SupportService/WarrantyRequests/{warrantyRequestId} | Delete a warranty request |
| [**get_warranty_request_async**](WarrantyRequestsApi.md#get_warranty_request_async) | **GET** /api/v2/SupportService/WarrantyRequests/{warrantyRequestId} | Retrieve a warranty request by ID |
| [**get_warranty_requests_async**](WarrantyRequestsApi.md#get_warranty_requests_async) | **GET** /api/v2/SupportService/WarrantyRequests | Retrieve warranty requests |
| [**get_warranty_requests_count_async**](WarrantyRequestsApi.md#get_warranty_requests_count_async) | **GET** /api/v2/SupportService/WarrantyRequests/Count | Get warranty requests count |
| [**update_warranty_request_async**](WarrantyRequestsApi.md#update_warranty_request_async) | **PUT** /api/v2/SupportService/WarrantyRequests/{warrantyRequestId} | Update a warranty request |


## create_warranty_request_async

> <EmptyEnvelope> create_warranty_request_async(tenant_id, opts)

Create a warranty request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarrantyRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  warranty_request_create_dto: OpenapiClient::WarrantyRequestCreateDto.new({title: 'title_example'}) # WarrantyRequestCreateDto | 
}

begin
  # Create a warranty request
  result = api_instance.create_warranty_request_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyRequestsApi->create_warranty_request_async: #{e}"
end
```

#### Using the create_warranty_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_warranty_request_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a warranty request
  data, status_code, headers = api_instance.create_warranty_request_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyRequestsApi->create_warranty_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **warranty_request_create_dto** | [**WarrantyRequestCreateDto**](WarrantyRequestCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_warranty_request_async

> <EmptyEnvelope> delete_warranty_request_async(tenant_id, warranty_request_id, opts)

Delete a warranty request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarrantyRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
warranty_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a warranty request
  result = api_instance.delete_warranty_request_async(tenant_id, warranty_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyRequestsApi->delete_warranty_request_async: #{e}"
end
```

#### Using the delete_warranty_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_warranty_request_async_with_http_info(tenant_id, warranty_request_id, opts)

```ruby
begin
  # Delete a warranty request
  data, status_code, headers = api_instance.delete_warranty_request_async_with_http_info(tenant_id, warranty_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyRequestsApi->delete_warranty_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **warranty_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_warranty_request_async

> <WarrantyRequestDtoEnvelope> get_warranty_request_async(tenant_id, warranty_request_id, opts)

Retrieve a warranty request by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarrantyRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
warranty_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a warranty request by ID
  result = api_instance.get_warranty_request_async(tenant_id, warranty_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyRequestsApi->get_warranty_request_async: #{e}"
end
```

#### Using the get_warranty_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WarrantyRequestDtoEnvelope>, Integer, Hash)> get_warranty_request_async_with_http_info(tenant_id, warranty_request_id, opts)

```ruby
begin
  # Retrieve a warranty request by ID
  data, status_code, headers = api_instance.get_warranty_request_async_with_http_info(tenant_id, warranty_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WarrantyRequestDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyRequestsApi->get_warranty_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **warranty_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WarrantyRequestDtoEnvelope**](WarrantyRequestDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_warranty_requests_async

> <WarrantyRequestDtoListEnvelope> get_warranty_requests_async(tenant_id, opts)

Retrieve warranty requests

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarrantyRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve warranty requests
  result = api_instance.get_warranty_requests_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyRequestsApi->get_warranty_requests_async: #{e}"
end
```

#### Using the get_warranty_requests_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WarrantyRequestDtoListEnvelope>, Integer, Hash)> get_warranty_requests_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve warranty requests
  data, status_code, headers = api_instance.get_warranty_requests_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WarrantyRequestDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyRequestsApi->get_warranty_requests_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WarrantyRequestDtoListEnvelope**](WarrantyRequestDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_warranty_requests_count_async

> <Int32Envelope> get_warranty_requests_count_async(tenant_id, opts)

Get warranty requests count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarrantyRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get warranty requests count
  result = api_instance.get_warranty_requests_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyRequestsApi->get_warranty_requests_count_async: #{e}"
end
```

#### Using the get_warranty_requests_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_warranty_requests_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get warranty requests count
  data, status_code, headers = api_instance.get_warranty_requests_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyRequestsApi->get_warranty_requests_count_async_with_http_info: #{e}"
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


## update_warranty_request_async

> <EmptyEnvelope> update_warranty_request_async(tenant_id, warranty_request_id, opts)

Update a warranty request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarrantyRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
warranty_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  warranty_request_update_dto: OpenapiClient::WarrantyRequestUpdateDto.new # WarrantyRequestUpdateDto | 
}

begin
  # Update a warranty request
  result = api_instance.update_warranty_request_async(tenant_id, warranty_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyRequestsApi->update_warranty_request_async: #{e}"
end
```

#### Using the update_warranty_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_warranty_request_async_with_http_info(tenant_id, warranty_request_id, opts)

```ruby
begin
  # Update a warranty request
  data, status_code, headers = api_instance.update_warranty_request_async_with_http_info(tenant_id, warranty_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyRequestsApi->update_warranty_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **warranty_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **warranty_request_update_dto** | [**WarrantyRequestUpdateDto**](WarrantyRequestUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

