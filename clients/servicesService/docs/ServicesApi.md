# OpenapiClient::ServicesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_service_async**](ServicesApi.md#create_service_async) | **POST** /api/v2/ServicesService/Services | Create a service |
| [**delete_service_async**](ServicesApi.md#delete_service_async) | **DELETE** /api/v2/ServicesService/Services/{serviceId} | Delete a service |
| [**get_service_by_id_async**](ServicesApi.md#get_service_by_id_async) | **GET** /api/v2/ServicesService/Services/{serviceId} | Get a service by ID |
| [**get_services_async**](ServicesApi.md#get_services_async) | **GET** /api/v2/ServicesService/Services | Get all services |
| [**get_services_count_async**](ServicesApi.md#get_services_count_async) | **GET** /api/v2/ServicesService/Services/Count | Get services count |
| [**patch_service_async**](ServicesApi.md#patch_service_async) | **PATCH** /api/v2/ServicesService/Services/{serviceId} | Patch a service |
| [**update_service_async**](ServicesApi.md#update_service_async) | **PUT** /api/v2/ServicesService/Services/{serviceId} | Update a service |


## create_service_async

> <Envelope> create_service_async(tenant_id, opts)

Create a service

Creates a new service for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  service_create_dto: OpenapiClient::ServiceCreateDto.new # ServiceCreateDto | 
}

begin
  # Create a service
  result = api_instance.create_service_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServicesApi->create_service_async: #{e}"
end
```

#### Using the create_service_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> create_service_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a service
  data, status_code, headers = api_instance.create_service_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServicesApi->create_service_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **service_create_dto** | [**ServiceCreateDto**](ServiceCreateDto.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_service_async

> <Envelope> delete_service_async(tenant_id, service_id, opts)

Delete a service

Deletes a service by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a service
  result = api_instance.delete_service_async(tenant_id, service_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServicesApi->delete_service_async: #{e}"
end
```

#### Using the delete_service_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> delete_service_async_with_http_info(tenant_id, service_id, opts)

```ruby
begin
  # Delete a service
  data, status_code, headers = api_instance.delete_service_async_with_http_info(tenant_id, service_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServicesApi->delete_service_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_service_by_id_async

> <ServiceDtoEnvelope> get_service_by_id_async(tenant_id, service_id, opts)

Get a service by ID

Retrieves a service by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a service by ID
  result = api_instance.get_service_by_id_async(tenant_id, service_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServicesApi->get_service_by_id_async: #{e}"
end
```

#### Using the get_service_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ServiceDtoEnvelope>, Integer, Hash)> get_service_by_id_async_with_http_info(tenant_id, service_id, opts)

```ruby
begin
  # Get a service by ID
  data, status_code, headers = api_instance.get_service_by_id_async_with_http_info(tenant_id, service_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ServiceDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServicesApi->get_service_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ServiceDtoEnvelope**](ServiceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_services_async

> <ServiceDtoIReadOnlyListEnvelope> get_services_async(tenant_id, opts)

Get all services

Retrieves all services for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all services
  result = api_instance.get_services_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServicesApi->get_services_async: #{e}"
end
```

#### Using the get_services_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ServiceDtoIReadOnlyListEnvelope>, Integer, Hash)> get_services_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all services
  data, status_code, headers = api_instance.get_services_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ServiceDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServicesApi->get_services_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ServiceDtoIReadOnlyListEnvelope**](ServiceDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_services_count_async

> <Int32Envelope> get_services_count_async(tenant_id, opts)

Get services count

Returns the count of services for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get services count
  result = api_instance.get_services_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServicesApi->get_services_count_async: #{e}"
end
```

#### Using the get_services_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_services_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get services count
  data, status_code, headers = api_instance.get_services_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServicesApi->get_services_count_async_with_http_info: #{e}"
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


## patch_service_async

> <Envelope> patch_service_async(tenant_id, service_id, opts)

Patch a service

Partially updates an existing service using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a service
  result = api_instance.patch_service_async(tenant_id, service_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServicesApi->patch_service_async: #{e}"
end
```

#### Using the patch_service_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> patch_service_async_with_http_info(tenant_id, service_id, opts)

```ruby
begin
  # Patch a service
  data, status_code, headers = api_instance.patch_service_async_with_http_info(tenant_id, service_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServicesApi->patch_service_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_service_async

> <Envelope> update_service_async(tenant_id, service_id, opts)

Update a service

Updates an existing service.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  service_update_dto: OpenapiClient::ServiceUpdateDto.new # ServiceUpdateDto | 
}

begin
  # Update a service
  result = api_instance.update_service_async(tenant_id, service_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServicesApi->update_service_async: #{e}"
end
```

#### Using the update_service_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> update_service_async_with_http_info(tenant_id, service_id, opts)

```ruby
begin
  # Update a service
  data, status_code, headers = api_instance.update_service_async_with_http_info(tenant_id, service_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServicesApi->update_service_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **service_update_dto** | [**ServiceUpdateDto**](ServiceUpdateDto.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

