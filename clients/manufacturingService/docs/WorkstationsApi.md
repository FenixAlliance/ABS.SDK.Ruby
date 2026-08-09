# OpenapiClient::WorkstationsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_workstation_async**](WorkstationsApi.md#create_workstation_async) | **POST** /api/v2/ManufacturingService/Workstations | Create a new workstation |
| [**delete_workstation_async**](WorkstationsApi.md#delete_workstation_async) | **DELETE** /api/v2/ManufacturingService/Workstations/{id} | Delete a workstation |
| [**get_workstation_by_id_async**](WorkstationsApi.md#get_workstation_by_id_async) | **GET** /api/v2/ManufacturingService/Workstations/{id} | Get workstation by ID |
| [**get_workstations_async**](WorkstationsApi.md#get_workstations_async) | **GET** /api/v2/ManufacturingService/Workstations | Get all workstations |
| [**get_workstations_count_async**](WorkstationsApi.md#get_workstations_count_async) | **GET** /api/v2/ManufacturingService/Workstations/Count | Get workstations count |
| [**patch_workstation_async**](WorkstationsApi.md#patch_workstation_async) | **PATCH** /api/v2/ManufacturingService/Workstations/{id} | Patch a workstation |
| [**update_workstation_async**](WorkstationsApi.md#update_workstation_async) | **PUT** /api/v2/ManufacturingService/Workstations/{id} | Update a workstation |


## create_workstation_async

> create_workstation_async(tenant_id, opts)

Create a new workstation

Creates a new workstation for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkstationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  workstation_create_dto: OpenapiClient::WorkstationCreateDto.new({code: 'code_example'}) # WorkstationCreateDto | 
}

begin
  # Create a new workstation
  api_instance.create_workstation_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkstationsApi->create_workstation_async: #{e}"
end
```

#### Using the create_workstation_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_workstation_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new workstation
  data, status_code, headers = api_instance.create_workstation_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkstationsApi->create_workstation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **workstation_create_dto** | [**WorkstationCreateDto**](WorkstationCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_workstation_async

> delete_workstation_async(tenant_id, id, opts)

Delete a workstation

Deletes a workstation for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkstationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a workstation
  api_instance.delete_workstation_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkstationsApi->delete_workstation_async: #{e}"
end
```

#### Using the delete_workstation_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_workstation_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a workstation
  data, status_code, headers = api_instance.delete_workstation_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkstationsApi->delete_workstation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_workstation_by_id_async

> <WorkstationDto> get_workstation_by_id_async(tenant_id, id, opts)

Get workstation by ID

Retrieves a specific workstation by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkstationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get workstation by ID
  result = api_instance.get_workstation_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkstationsApi->get_workstation_by_id_async: #{e}"
end
```

#### Using the get_workstation_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WorkstationDto>, Integer, Hash)> get_workstation_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get workstation by ID
  data, status_code, headers = api_instance.get_workstation_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WorkstationDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkstationsApi->get_workstation_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WorkstationDto**](WorkstationDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_workstations_async

> <WorkstationDtoListEnvelope> get_workstations_async(tenant_id, opts)

Get all workstations

Retrieves all workstations for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkstationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  workstation_dto_collection_query_parameters: OpenapiClient::WorkstationDtoCollectionQueryParameters.new # WorkstationDtoCollectionQueryParameters | 
}

begin
  # Get all workstations
  result = api_instance.get_workstations_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkstationsApi->get_workstations_async: #{e}"
end
```

#### Using the get_workstations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WorkstationDtoListEnvelope>, Integer, Hash)> get_workstations_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all workstations
  data, status_code, headers = api_instance.get_workstations_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WorkstationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkstationsApi->get_workstations_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **workstation_dto_collection_query_parameters** | [**WorkstationDtoCollectionQueryParameters**](WorkstationDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**WorkstationDtoListEnvelope**](WorkstationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_workstations_count_async

> <Int32Envelope> get_workstations_count_async(tenant_id, opts)

Get workstations count

Returns the count of workstations for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkstationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  workstation_dto_collection_query_parameters: OpenapiClient::WorkstationDtoCollectionQueryParameters.new # WorkstationDtoCollectionQueryParameters | 
}

begin
  # Get workstations count
  result = api_instance.get_workstations_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkstationsApi->get_workstations_count_async: #{e}"
end
```

#### Using the get_workstations_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_workstations_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get workstations count
  data, status_code, headers = api_instance.get_workstations_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkstationsApi->get_workstations_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **workstation_dto_collection_query_parameters** | [**WorkstationDtoCollectionQueryParameters**](WorkstationDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_workstation_async

> <EmptyEnvelope> patch_workstation_async(tenant_id, id, opts)

Patch a workstation

Patch a workstation

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkstationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a workstation
  result = api_instance.patch_workstation_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkstationsApi->patch_workstation_async: #{e}"
end
```

#### Using the patch_workstation_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_workstation_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a workstation
  data, status_code, headers = api_instance.patch_workstation_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkstationsApi->patch_workstation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_workstation_async

> update_workstation_async(tenant_id, id, opts)

Update a workstation

Updates an existing workstation for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkstationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  workstation_update_dto: OpenapiClient::WorkstationUpdateDto.new # WorkstationUpdateDto | 
}

begin
  # Update a workstation
  api_instance.update_workstation_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkstationsApi->update_workstation_async: #{e}"
end
```

#### Using the update_workstation_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_workstation_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a workstation
  data, status_code, headers = api_instance.update_workstation_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkstationsApi->update_workstation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **workstation_update_dto** | [**WorkstationUpdateDto**](WorkstationUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

