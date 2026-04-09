# OpenapiClient::ServiceLevelsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_all_service_levels_async**](ServiceLevelsApi.md#count_all_service_levels_async) | **GET** /api/v2/ServicesService/ServiceLevels/Count | Get all service levels count |
| [**create_service_level_async**](ServiceLevelsApi.md#create_service_level_async) | **POST** /api/v2/ServicesService/Services/{serviceId}/ServiceLevels | Create a service level |
| [**delete_service_level_async**](ServiceLevelsApi.md#delete_service_level_async) | **DELETE** /api/v2/ServicesService/Services/{serviceId}/ServiceLevels/{serviceLevelId} | Delete a service level |
| [**get_all_service_levels_async**](ServiceLevelsApi.md#get_all_service_levels_async) | **GET** /api/v2/ServicesService/ServiceLevels | Get all service levels |
| [**get_service_level_by_id_async**](ServiceLevelsApi.md#get_service_level_by_id_async) | **GET** /api/v2/ServicesService/Services/{serviceId}/ServiceLevels/{serviceLevelId} | Get a service level by ID |
| [**get_service_levels_async**](ServiceLevelsApi.md#get_service_levels_async) | **GET** /api/v2/ServicesService/Services/{serviceId}/ServiceLevels | Get all service levels |
| [**get_service_levels_count_async**](ServiceLevelsApi.md#get_service_levels_count_async) | **GET** /api/v2/ServicesService/Services/{serviceId}/ServiceLevels/Count | Get service levels count |
| [**update_service_level_async**](ServiceLevelsApi.md#update_service_level_async) | **PUT** /api/v2/ServicesService/Services/{serviceId}/ServiceLevels/{serviceLevelId} | Update a service level |


## count_all_service_levels_async

> <Int32Envelope> count_all_service_levels_async(tenant_id, opts)

Get all service levels count

Returns the count of all service levels for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceLevelsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all service levels count
  result = api_instance.count_all_service_levels_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelsApi->count_all_service_levels_async: #{e}"
end
```

#### Using the count_all_service_levels_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_all_service_levels_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all service levels count
  data, status_code, headers = api_instance.count_all_service_levels_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelsApi->count_all_service_levels_async_with_http_info: #{e}"
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


## create_service_level_async

> <Envelope> create_service_level_async(tenant_id, service_id, opts)

Create a service level

Creates a new service level for the specified service.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceLevelsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  service_level_create_dto: OpenapiClient::ServiceLevelCreateDto.new # ServiceLevelCreateDto | 
}

begin
  # Create a service level
  result = api_instance.create_service_level_async(tenant_id, service_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelsApi->create_service_level_async: #{e}"
end
```

#### Using the create_service_level_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> create_service_level_async_with_http_info(tenant_id, service_id, opts)

```ruby
begin
  # Create a service level
  data, status_code, headers = api_instance.create_service_level_async_with_http_info(tenant_id, service_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelsApi->create_service_level_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **service_level_create_dto** | [**ServiceLevelCreateDto**](ServiceLevelCreateDto.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_service_level_async

> <Envelope> delete_service_level_async(tenant_id, service_id, service_level_id, opts)

Delete a service level

Deletes a service level by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceLevelsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_level_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a service level
  result = api_instance.delete_service_level_async(tenant_id, service_id, service_level_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelsApi->delete_service_level_async: #{e}"
end
```

#### Using the delete_service_level_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> delete_service_level_async_with_http_info(tenant_id, service_id, service_level_id, opts)

```ruby
begin
  # Delete a service level
  data, status_code, headers = api_instance.delete_service_level_async_with_http_info(tenant_id, service_id, service_level_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelsApi->delete_service_level_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_id** | **String** |  |  |
| **service_level_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_all_service_levels_async

> <ServiceLevelDtoIReadOnlyListEnvelope> get_all_service_levels_async(tenant_id, opts)

Get all service levels

Retrieves all service levels for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceLevelsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all service levels
  result = api_instance.get_all_service_levels_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelsApi->get_all_service_levels_async: #{e}"
end
```

#### Using the get_all_service_levels_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ServiceLevelDtoIReadOnlyListEnvelope>, Integer, Hash)> get_all_service_levels_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all service levels
  data, status_code, headers = api_instance.get_all_service_levels_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ServiceLevelDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelsApi->get_all_service_levels_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ServiceLevelDtoIReadOnlyListEnvelope**](ServiceLevelDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_service_level_by_id_async

> <ServiceLevelDtoEnvelope> get_service_level_by_id_async(tenant_id, service_id, service_level_id, opts)

Get a service level by ID

Retrieves a service level by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceLevelsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_level_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a service level by ID
  result = api_instance.get_service_level_by_id_async(tenant_id, service_id, service_level_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelsApi->get_service_level_by_id_async: #{e}"
end
```

#### Using the get_service_level_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ServiceLevelDtoEnvelope>, Integer, Hash)> get_service_level_by_id_async_with_http_info(tenant_id, service_id, service_level_id, opts)

```ruby
begin
  # Get a service level by ID
  data, status_code, headers = api_instance.get_service_level_by_id_async_with_http_info(tenant_id, service_id, service_level_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ServiceLevelDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelsApi->get_service_level_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_id** | **String** |  |  |
| **service_level_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ServiceLevelDtoEnvelope**](ServiceLevelDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_service_levels_async

> <ServiceLevelDtoIReadOnlyListEnvelope> get_service_levels_async(tenant_id, service_id, opts)

Get all service levels

Retrieves all service levels for the specified service.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceLevelsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all service levels
  result = api_instance.get_service_levels_async(tenant_id, service_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelsApi->get_service_levels_async: #{e}"
end
```

#### Using the get_service_levels_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ServiceLevelDtoIReadOnlyListEnvelope>, Integer, Hash)> get_service_levels_async_with_http_info(tenant_id, service_id, opts)

```ruby
begin
  # Get all service levels
  data, status_code, headers = api_instance.get_service_levels_async_with_http_info(tenant_id, service_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ServiceLevelDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelsApi->get_service_levels_async_with_http_info: #{e}"
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

[**ServiceLevelDtoIReadOnlyListEnvelope**](ServiceLevelDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_service_levels_count_async

> <Int32Envelope> get_service_levels_count_async(tenant_id, service_id, opts)

Get service levels count

Returns the count of service levels for the specified service.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceLevelsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get service levels count
  result = api_instance.get_service_levels_count_async(tenant_id, service_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelsApi->get_service_levels_count_async: #{e}"
end
```

#### Using the get_service_levels_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_service_levels_count_async_with_http_info(tenant_id, service_id, opts)

```ruby
begin
  # Get service levels count
  data, status_code, headers = api_instance.get_service_levels_count_async_with_http_info(tenant_id, service_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelsApi->get_service_levels_count_async_with_http_info: #{e}"
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

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_service_level_async

> <Envelope> update_service_level_async(tenant_id, service_id, service_level_id, opts)

Update a service level

Updates an existing service level.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceLevelsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_level_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  service_level_update_dto: OpenapiClient::ServiceLevelUpdateDto.new # ServiceLevelUpdateDto | 
}

begin
  # Update a service level
  result = api_instance.update_service_level_async(tenant_id, service_id, service_level_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelsApi->update_service_level_async: #{e}"
end
```

#### Using the update_service_level_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> update_service_level_async_with_http_info(tenant_id, service_id, service_level_id, opts)

```ruby
begin
  # Update a service level
  data, status_code, headers = api_instance.update_service_level_async_with_http_info(tenant_id, service_id, service_level_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelsApi->update_service_level_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_id** | **String** |  |  |
| **service_level_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **service_level_update_dto** | [**ServiceLevelUpdateDto**](ServiceLevelUpdateDto.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

