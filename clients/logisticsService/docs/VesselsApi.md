# OpenapiClient::VesselsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_vessel_async**](VesselsApi.md#create_vessel_async) | **POST** /api/v2/LogisticsService/Vessels | Create a vessel |
| [**delete_vessel_async**](VesselsApi.md#delete_vessel_async) | **DELETE** /api/v2/LogisticsService/Vessels/{vesselId} | Delete a vessel |
| [**get_vessel_by_id_async**](VesselsApi.md#get_vessel_by_id_async) | **GET** /api/v2/LogisticsService/Vessels/{vesselId} | Get vessel by ID |
| [**get_vessels_async**](VesselsApi.md#get_vessels_async) | **GET** /api/v2/LogisticsService/Vessels | Get all vessels |
| [**get_vessels_count_async**](VesselsApi.md#get_vessels_count_async) | **GET** /api/v2/LogisticsService/Vessels/Count | Get vessels count |
| [**patch_vessel_async**](VesselsApi.md#patch_vessel_async) | **PATCH** /api/v2/LogisticsService/Vessels/{vesselId} | Patch a vessel |
| [**update_vessel_async**](VesselsApi.md#update_vessel_async) | **PUT** /api/v2/LogisticsService/Vessels/{vesselId} | Update a vessel |


## create_vessel_async

> <EmptyEnvelope> create_vessel_async(tenant_id, opts)

Create a vessel

Creates a new vessel for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VesselsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  vessel_create_dto: OpenapiClient::VesselCreateDto.new # VesselCreateDto | 
}

begin
  # Create a vessel
  result = api_instance.create_vessel_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VesselsApi->create_vessel_async: #{e}"
end
```

#### Using the create_vessel_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_vessel_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a vessel
  data, status_code, headers = api_instance.create_vessel_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VesselsApi->create_vessel_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **vessel_create_dto** | [**VesselCreateDto**](VesselCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_vessel_async

> <EmptyEnvelope> delete_vessel_async(tenant_id, vessel_id, opts)

Delete a vessel

Deletes a vessel.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VesselsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
vessel_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a vessel
  result = api_instance.delete_vessel_async(tenant_id, vessel_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VesselsApi->delete_vessel_async: #{e}"
end
```

#### Using the delete_vessel_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_vessel_async_with_http_info(tenant_id, vessel_id, opts)

```ruby
begin
  # Delete a vessel
  data, status_code, headers = api_instance.delete_vessel_async_with_http_info(tenant_id, vessel_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VesselsApi->delete_vessel_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **vessel_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_vessel_by_id_async

> <VesselDtoEnvelope> get_vessel_by_id_async(tenant_id, vessel_id, opts)

Get vessel by ID

Retrieves a specific vessel by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VesselsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
vessel_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get vessel by ID
  result = api_instance.get_vessel_by_id_async(tenant_id, vessel_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VesselsApi->get_vessel_by_id_async: #{e}"
end
```

#### Using the get_vessel_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<VesselDtoEnvelope>, Integer, Hash)> get_vessel_by_id_async_with_http_info(tenant_id, vessel_id, opts)

```ruby
begin
  # Get vessel by ID
  data, status_code, headers = api_instance.get_vessel_by_id_async_with_http_info(tenant_id, vessel_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <VesselDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VesselsApi->get_vessel_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **vessel_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**VesselDtoEnvelope**](VesselDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_vessels_async

> <VesselDtoListEnvelope> get_vessels_async(tenant_id, opts)

Get all vessels

Retrieves all vessels for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VesselsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  vessel_dto_collection_query_parameters: OpenapiClient::VesselDtoCollectionQueryParameters.new # VesselDtoCollectionQueryParameters | 
}

begin
  # Get all vessels
  result = api_instance.get_vessels_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VesselsApi->get_vessels_async: #{e}"
end
```

#### Using the get_vessels_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<VesselDtoListEnvelope>, Integer, Hash)> get_vessels_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all vessels
  data, status_code, headers = api_instance.get_vessels_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <VesselDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VesselsApi->get_vessels_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **vessel_dto_collection_query_parameters** | [**VesselDtoCollectionQueryParameters**](VesselDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**VesselDtoListEnvelope**](VesselDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_vessels_count_async

> <Int32Envelope> get_vessels_count_async(tenant_id, opts)

Get vessels count

Returns the count of vessels for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VesselsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  vessel_dto_collection_query_parameters: OpenapiClient::VesselDtoCollectionQueryParameters.new # VesselDtoCollectionQueryParameters | 
}

begin
  # Get vessels count
  result = api_instance.get_vessels_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VesselsApi->get_vessels_count_async: #{e}"
end
```

#### Using the get_vessels_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_vessels_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get vessels count
  data, status_code, headers = api_instance.get_vessels_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VesselsApi->get_vessels_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **vessel_dto_collection_query_parameters** | [**VesselDtoCollectionQueryParameters**](VesselDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_vessel_async

> <EmptyEnvelope> patch_vessel_async(tenant_id, vessel_id, opts)

Patch a vessel

Partially updates an existing vessel using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VesselsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
vessel_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a vessel
  result = api_instance.patch_vessel_async(tenant_id, vessel_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VesselsApi->patch_vessel_async: #{e}"
end
```

#### Using the patch_vessel_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_vessel_async_with_http_info(tenant_id, vessel_id, opts)

```ruby
begin
  # Patch a vessel
  data, status_code, headers = api_instance.patch_vessel_async_with_http_info(tenant_id, vessel_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VesselsApi->patch_vessel_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **vessel_id** | **String** |  |  |
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


## update_vessel_async

> <EmptyEnvelope> update_vessel_async(tenant_id, vessel_id, opts)

Update a vessel

Updates an existing vessel.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VesselsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
vessel_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  vessel_update_dto: OpenapiClient::VesselUpdateDto.new # VesselUpdateDto | 
}

begin
  # Update a vessel
  result = api_instance.update_vessel_async(tenant_id, vessel_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VesselsApi->update_vessel_async: #{e}"
end
```

#### Using the update_vessel_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_vessel_async_with_http_info(tenant_id, vessel_id, opts)

```ruby
begin
  # Update a vessel
  data, status_code, headers = api_instance.update_vessel_async_with_http_info(tenant_id, vessel_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VesselsApi->update_vessel_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **vessel_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **vessel_update_dto** | [**VesselUpdateDto**](VesselUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

