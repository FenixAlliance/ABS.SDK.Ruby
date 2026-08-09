# OpenapiClient::ServiceCasesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_service_case_async**](ServiceCasesApi.md#create_service_case_async) | **POST** /api/v2/ServicesService/ServiceCases | Create a service case |
| [**delete_service_case_async**](ServiceCasesApi.md#delete_service_case_async) | **DELETE** /api/v2/ServicesService/ServiceCases/{serviceCaseId} | Delete a service case |
| [**get_service_case_by_id_async**](ServiceCasesApi.md#get_service_case_by_id_async) | **GET** /api/v2/ServicesService/ServiceCases/{serviceCaseId} | Get a service case by ID |
| [**get_service_cases_async**](ServiceCasesApi.md#get_service_cases_async) | **GET** /api/v2/ServicesService/ServiceCases | Get all service cases |
| [**get_service_cases_count_async**](ServiceCasesApi.md#get_service_cases_count_async) | **GET** /api/v2/ServicesService/ServiceCases/Count | Get service cases count |
| [**patch_service_case_async**](ServiceCasesApi.md#patch_service_case_async) | **PATCH** /api/v2/ServicesService/ServiceCases/{serviceCaseId} | Patch a service case |
| [**update_service_case_async**](ServiceCasesApi.md#update_service_case_async) | **PUT** /api/v2/ServicesService/ServiceCases/{serviceCaseId} | Update a service case |


## create_service_case_async

> <Envelope> create_service_case_async(tenant_id, opts)

Create a service case

Creates a new service case for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceCasesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  service_case_create_dto: OpenapiClient::ServiceCaseCreateDto.new # ServiceCaseCreateDto | 
}

begin
  # Create a service case
  result = api_instance.create_service_case_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCasesApi->create_service_case_async: #{e}"
end
```

#### Using the create_service_case_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> create_service_case_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a service case
  data, status_code, headers = api_instance.create_service_case_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCasesApi->create_service_case_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **service_case_create_dto** | [**ServiceCaseCreateDto**](ServiceCaseCreateDto.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_service_case_async

> <Envelope> delete_service_case_async(tenant_id, service_case_id, opts)

Delete a service case

Deletes a service case by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceCasesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_case_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a service case
  result = api_instance.delete_service_case_async(tenant_id, service_case_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCasesApi->delete_service_case_async: #{e}"
end
```

#### Using the delete_service_case_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> delete_service_case_async_with_http_info(tenant_id, service_case_id, opts)

```ruby
begin
  # Delete a service case
  data, status_code, headers = api_instance.delete_service_case_async_with_http_info(tenant_id, service_case_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCasesApi->delete_service_case_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_case_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_service_case_by_id_async

> <ServiceCaseDtoEnvelope> get_service_case_by_id_async(tenant_id, service_case_id, opts)

Get a service case by ID

Retrieves a service case by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceCasesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_case_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a service case by ID
  result = api_instance.get_service_case_by_id_async(tenant_id, service_case_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCasesApi->get_service_case_by_id_async: #{e}"
end
```

#### Using the get_service_case_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ServiceCaseDtoEnvelope>, Integer, Hash)> get_service_case_by_id_async_with_http_info(tenant_id, service_case_id, opts)

```ruby
begin
  # Get a service case by ID
  data, status_code, headers = api_instance.get_service_case_by_id_async_with_http_info(tenant_id, service_case_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ServiceCaseDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCasesApi->get_service_case_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_case_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ServiceCaseDtoEnvelope**](ServiceCaseDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_service_cases_async

> <ServiceCaseDtoIReadOnlyListEnvelope> get_service_cases_async(tenant_id, opts)

Get all service cases

Retrieves all service cases for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceCasesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  service_case_dto_collection_query_parameters: OpenapiClient::ServiceCaseDtoCollectionQueryParameters.new # ServiceCaseDtoCollectionQueryParameters | 
}

begin
  # Get all service cases
  result = api_instance.get_service_cases_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCasesApi->get_service_cases_async: #{e}"
end
```

#### Using the get_service_cases_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ServiceCaseDtoIReadOnlyListEnvelope>, Integer, Hash)> get_service_cases_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all service cases
  data, status_code, headers = api_instance.get_service_cases_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ServiceCaseDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCasesApi->get_service_cases_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **service_case_dto_collection_query_parameters** | [**ServiceCaseDtoCollectionQueryParameters**](ServiceCaseDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ServiceCaseDtoIReadOnlyListEnvelope**](ServiceCaseDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_service_cases_count_async

> <Int32Envelope> get_service_cases_count_async(tenant_id, opts)

Get service cases count

Returns the count of service cases for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceCasesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  service_case_dto_collection_query_parameters: OpenapiClient::ServiceCaseDtoCollectionQueryParameters.new # ServiceCaseDtoCollectionQueryParameters | 
}

begin
  # Get service cases count
  result = api_instance.get_service_cases_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCasesApi->get_service_cases_count_async: #{e}"
end
```

#### Using the get_service_cases_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_service_cases_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get service cases count
  data, status_code, headers = api_instance.get_service_cases_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCasesApi->get_service_cases_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **service_case_dto_collection_query_parameters** | [**ServiceCaseDtoCollectionQueryParameters**](ServiceCaseDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_service_case_async

> <Envelope> patch_service_case_async(tenant_id, service_case_id, opts)

Patch a service case

Partially updates an existing service case using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceCasesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_case_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a service case
  result = api_instance.patch_service_case_async(tenant_id, service_case_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCasesApi->patch_service_case_async: #{e}"
end
```

#### Using the patch_service_case_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> patch_service_case_async_with_http_info(tenant_id, service_case_id, opts)

```ruby
begin
  # Patch a service case
  data, status_code, headers = api_instance.patch_service_case_async_with_http_info(tenant_id, service_case_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCasesApi->patch_service_case_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_case_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_service_case_async

> <Envelope> update_service_case_async(tenant_id, service_case_id, opts)

Update a service case

Updates an existing service case.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceCasesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_case_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  service_case_update_dto: OpenapiClient::ServiceCaseUpdateDto.new # ServiceCaseUpdateDto | 
}

begin
  # Update a service case
  result = api_instance.update_service_case_async(tenant_id, service_case_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCasesApi->update_service_case_async: #{e}"
end
```

#### Using the update_service_case_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> update_service_case_async_with_http_info(tenant_id, service_case_id, opts)

```ruby
begin
  # Update a service case
  data, status_code, headers = api_instance.update_service_case_async_with_http_info(tenant_id, service_case_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceCasesApi->update_service_case_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_case_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **service_case_update_dto** | [**ServiceCaseUpdateDto**](ServiceCaseUpdateDto.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

