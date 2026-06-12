# OpenapiClient::ServiceCaseTypesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_service_case_type_async**](ServiceCaseTypesApi.md#create_service_case_type_async) | **POST** /api/v2/ServicesService/ServiceCaseTypes | Create a service case type |
| [**delete_service_case_type_async**](ServiceCaseTypesApi.md#delete_service_case_type_async) | **DELETE** /api/v2/ServicesService/ServiceCaseTypes/{serviceCaseTypeId} | Delete a service case type |
| [**get_service_case_type_by_id_async**](ServiceCaseTypesApi.md#get_service_case_type_by_id_async) | **GET** /api/v2/ServicesService/ServiceCaseTypes/{serviceCaseTypeId} | Get a service case type by ID |
| [**get_service_case_types_async**](ServiceCaseTypesApi.md#get_service_case_types_async) | **GET** /api/v2/ServicesService/ServiceCaseTypes | Get all service case types |
| [**get_service_case_types_count_async**](ServiceCaseTypesApi.md#get_service_case_types_count_async) | **GET** /api/v2/ServicesService/ServiceCaseTypes/Count | Get service case types count |
| [**patch_service_case_type_async**](ServiceCaseTypesApi.md#patch_service_case_type_async) | **PATCH** /api/v2/ServicesService/ServiceCaseTypes/{serviceCaseTypeId} | Patch a service case type |
| [**update_service_case_type_async**](ServiceCaseTypesApi.md#update_service_case_type_async) | **PUT** /api/v2/ServicesService/ServiceCaseTypes/{serviceCaseTypeId} | Update a service case type |


## create_service_case_type_async

> <Envelope> create_service_case_type_async(tenant_id, opts)

Create a service case type

Creates a new service case type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceCaseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  service_case_type_create_dto: OpenapiClient::ServiceCaseTypeCreateDto.new # ServiceCaseTypeCreateDto | 
}

begin
  # Create a service case type
  result = api_instance.create_service_case_type_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCaseTypesApi->create_service_case_type_async: #{e}"
end
```

#### Using the create_service_case_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> create_service_case_type_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a service case type
  data, status_code, headers = api_instance.create_service_case_type_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCaseTypesApi->create_service_case_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **service_case_type_create_dto** | [**ServiceCaseTypeCreateDto**](ServiceCaseTypeCreateDto.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_service_case_type_async

> <Envelope> delete_service_case_type_async(tenant_id, service_case_type_id, opts)

Delete a service case type

Deletes a service case type by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceCaseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_case_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a service case type
  result = api_instance.delete_service_case_type_async(tenant_id, service_case_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCaseTypesApi->delete_service_case_type_async: #{e}"
end
```

#### Using the delete_service_case_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> delete_service_case_type_async_with_http_info(tenant_id, service_case_type_id, opts)

```ruby
begin
  # Delete a service case type
  data, status_code, headers = api_instance.delete_service_case_type_async_with_http_info(tenant_id, service_case_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCaseTypesApi->delete_service_case_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_case_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_service_case_type_by_id_async

> <ServiceCaseTypeDtoEnvelope> get_service_case_type_by_id_async(tenant_id, service_case_type_id, opts)

Get a service case type by ID

Retrieves a service case type by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceCaseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_case_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a service case type by ID
  result = api_instance.get_service_case_type_by_id_async(tenant_id, service_case_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCaseTypesApi->get_service_case_type_by_id_async: #{e}"
end
```

#### Using the get_service_case_type_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ServiceCaseTypeDtoEnvelope>, Integer, Hash)> get_service_case_type_by_id_async_with_http_info(tenant_id, service_case_type_id, opts)

```ruby
begin
  # Get a service case type by ID
  data, status_code, headers = api_instance.get_service_case_type_by_id_async_with_http_info(tenant_id, service_case_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ServiceCaseTypeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCaseTypesApi->get_service_case_type_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_case_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ServiceCaseTypeDtoEnvelope**](ServiceCaseTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_service_case_types_async

> <ServiceCaseTypeDtoIReadOnlyListEnvelope> get_service_case_types_async(tenant_id, opts)

Get all service case types

Retrieves all service case types for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceCaseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all service case types
  result = api_instance.get_service_case_types_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCaseTypesApi->get_service_case_types_async: #{e}"
end
```

#### Using the get_service_case_types_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ServiceCaseTypeDtoIReadOnlyListEnvelope>, Integer, Hash)> get_service_case_types_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all service case types
  data, status_code, headers = api_instance.get_service_case_types_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ServiceCaseTypeDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCaseTypesApi->get_service_case_types_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ServiceCaseTypeDtoIReadOnlyListEnvelope**](ServiceCaseTypeDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_service_case_types_count_async

> <Int32Envelope> get_service_case_types_count_async(tenant_id, opts)

Get service case types count

Returns the count of service case types for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceCaseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get service case types count
  result = api_instance.get_service_case_types_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCaseTypesApi->get_service_case_types_count_async: #{e}"
end
```

#### Using the get_service_case_types_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_service_case_types_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get service case types count
  data, status_code, headers = api_instance.get_service_case_types_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCaseTypesApi->get_service_case_types_count_async_with_http_info: #{e}"
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


## patch_service_case_type_async

> <Envelope> patch_service_case_type_async(tenant_id, service_case_type_id, opts)

Patch a service case type

Partially updates an existing service case type using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceCaseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_case_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a service case type
  result = api_instance.patch_service_case_type_async(tenant_id, service_case_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCaseTypesApi->patch_service_case_type_async: #{e}"
end
```

#### Using the patch_service_case_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> patch_service_case_type_async_with_http_info(tenant_id, service_case_type_id, opts)

```ruby
begin
  # Patch a service case type
  data, status_code, headers = api_instance.patch_service_case_type_async_with_http_info(tenant_id, service_case_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCaseTypesApi->patch_service_case_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_case_type_id** | **String** |  |  |
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


## update_service_case_type_async

> <Envelope> update_service_case_type_async(tenant_id, service_case_type_id, opts)

Update a service case type

Updates an existing service case type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceCaseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_case_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  service_case_type_update_dto: OpenapiClient::ServiceCaseTypeUpdateDto.new # ServiceCaseTypeUpdateDto | 
}

begin
  # Update a service case type
  result = api_instance.update_service_case_type_async(tenant_id, service_case_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCaseTypesApi->update_service_case_type_async: #{e}"
end
```

#### Using the update_service_case_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> update_service_case_type_async_with_http_info(tenant_id, service_case_type_id, opts)

```ruby
begin
  # Update a service case type
  data, status_code, headers = api_instance.update_service_case_type_async_with_http_info(tenant_id, service_case_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCaseTypesApi->update_service_case_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_case_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **service_case_type_update_dto** | [**ServiceCaseTypeUpdateDto**](ServiceCaseTypeUpdateDto.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

