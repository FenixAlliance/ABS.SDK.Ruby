# OpenapiClient::ServiceQueuesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_service_queue_async**](ServiceQueuesApi.md#create_service_queue_async) | **POST** /api/v2/ServicesService/ServiceQueues | Create a service queue |
| [**delete_service_queue_async**](ServiceQueuesApi.md#delete_service_queue_async) | **DELETE** /api/v2/ServicesService/ServiceQueues/{serviceQueueId} | Delete a service queue |
| [**get_service_queue_by_id_async**](ServiceQueuesApi.md#get_service_queue_by_id_async) | **GET** /api/v2/ServicesService/ServiceQueues/{serviceQueueId} | Get a service queue by ID |
| [**get_service_queues_async**](ServiceQueuesApi.md#get_service_queues_async) | **GET** /api/v2/ServicesService/ServiceQueues | Get all service queues |
| [**get_service_queues_count_async**](ServiceQueuesApi.md#get_service_queues_count_async) | **GET** /api/v2/ServicesService/ServiceQueues/Count | Get service queues count |
| [**patch_service_queue_async**](ServiceQueuesApi.md#patch_service_queue_async) | **PATCH** /api/v2/ServicesService/ServiceQueues/{serviceQueueId} | Patch a service queue |
| [**update_service_queue_async**](ServiceQueuesApi.md#update_service_queue_async) | **PUT** /api/v2/ServicesService/ServiceQueues/{serviceQueueId} | Update a service queue |


## create_service_queue_async

> <Envelope> create_service_queue_async(tenant_id, opts)

Create a service queue

Creates a new service queue for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceQueuesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  service_queue_create_dto: OpenapiClient::ServiceQueueCreateDto.new # ServiceQueueCreateDto | 
}

begin
  # Create a service queue
  result = api_instance.create_service_queue_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceQueuesApi->create_service_queue_async: #{e}"
end
```

#### Using the create_service_queue_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> create_service_queue_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a service queue
  data, status_code, headers = api_instance.create_service_queue_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceQueuesApi->create_service_queue_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **service_queue_create_dto** | [**ServiceQueueCreateDto**](ServiceQueueCreateDto.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_service_queue_async

> <Envelope> delete_service_queue_async(tenant_id, service_queue_id, opts)

Delete a service queue

Deletes a service queue by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceQueuesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_queue_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a service queue
  result = api_instance.delete_service_queue_async(tenant_id, service_queue_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceQueuesApi->delete_service_queue_async: #{e}"
end
```

#### Using the delete_service_queue_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> delete_service_queue_async_with_http_info(tenant_id, service_queue_id, opts)

```ruby
begin
  # Delete a service queue
  data, status_code, headers = api_instance.delete_service_queue_async_with_http_info(tenant_id, service_queue_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceQueuesApi->delete_service_queue_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_queue_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_service_queue_by_id_async

> <ServiceQueueDtoEnvelope> get_service_queue_by_id_async(tenant_id, service_queue_id, opts)

Get a service queue by ID

Retrieves a service queue by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceQueuesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_queue_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a service queue by ID
  result = api_instance.get_service_queue_by_id_async(tenant_id, service_queue_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceQueuesApi->get_service_queue_by_id_async: #{e}"
end
```

#### Using the get_service_queue_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ServiceQueueDtoEnvelope>, Integer, Hash)> get_service_queue_by_id_async_with_http_info(tenant_id, service_queue_id, opts)

```ruby
begin
  # Get a service queue by ID
  data, status_code, headers = api_instance.get_service_queue_by_id_async_with_http_info(tenant_id, service_queue_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ServiceQueueDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceQueuesApi->get_service_queue_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_queue_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ServiceQueueDtoEnvelope**](ServiceQueueDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_service_queues_async

> <ServiceQueueDtoIReadOnlyListEnvelope> get_service_queues_async(tenant_id, opts)

Get all service queues

Retrieves all service queues for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceQueuesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  service_queue_dto_collection_query_parameters: OpenapiClient::ServiceQueueDtoCollectionQueryParameters.new # ServiceQueueDtoCollectionQueryParameters | 
}

begin
  # Get all service queues
  result = api_instance.get_service_queues_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceQueuesApi->get_service_queues_async: #{e}"
end
```

#### Using the get_service_queues_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ServiceQueueDtoIReadOnlyListEnvelope>, Integer, Hash)> get_service_queues_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all service queues
  data, status_code, headers = api_instance.get_service_queues_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ServiceQueueDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceQueuesApi->get_service_queues_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **service_queue_dto_collection_query_parameters** | [**ServiceQueueDtoCollectionQueryParameters**](ServiceQueueDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ServiceQueueDtoIReadOnlyListEnvelope**](ServiceQueueDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_service_queues_count_async

> <Int32Envelope> get_service_queues_count_async(tenant_id, opts)

Get service queues count

Returns the count of service queues for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceQueuesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  service_queue_dto_collection_query_parameters: OpenapiClient::ServiceQueueDtoCollectionQueryParameters.new # ServiceQueueDtoCollectionQueryParameters | 
}

begin
  # Get service queues count
  result = api_instance.get_service_queues_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceQueuesApi->get_service_queues_count_async: #{e}"
end
```

#### Using the get_service_queues_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_service_queues_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get service queues count
  data, status_code, headers = api_instance.get_service_queues_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceQueuesApi->get_service_queues_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **service_queue_dto_collection_query_parameters** | [**ServiceQueueDtoCollectionQueryParameters**](ServiceQueueDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_service_queue_async

> <Envelope> patch_service_queue_async(tenant_id, service_queue_id, opts)

Patch a service queue

Partially updates an existing service queue using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceQueuesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_queue_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a service queue
  result = api_instance.patch_service_queue_async(tenant_id, service_queue_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceQueuesApi->patch_service_queue_async: #{e}"
end
```

#### Using the patch_service_queue_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> patch_service_queue_async_with_http_info(tenant_id, service_queue_id, opts)

```ruby
begin
  # Patch a service queue
  data, status_code, headers = api_instance.patch_service_queue_async_with_http_info(tenant_id, service_queue_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceQueuesApi->patch_service_queue_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_queue_id** | **String** |  |  |
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


## update_service_queue_async

> <Envelope> update_service_queue_async(tenant_id, service_queue_id, opts)

Update a service queue

Updates an existing service queue.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceQueuesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_queue_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  service_queue_update_dto: OpenapiClient::ServiceQueueUpdateDto.new # ServiceQueueUpdateDto | 
}

begin
  # Update a service queue
  result = api_instance.update_service_queue_async(tenant_id, service_queue_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceQueuesApi->update_service_queue_async: #{e}"
end
```

#### Using the update_service_queue_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> update_service_queue_async_with_http_info(tenant_id, service_queue_id, opts)

```ruby
begin
  # Update a service queue
  data, status_code, headers = api_instance.update_service_queue_async_with_http_info(tenant_id, service_queue_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceQueuesApi->update_service_queue_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_queue_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **service_queue_update_dto** | [**ServiceQueueUpdateDto**](ServiceQueueUpdateDto.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

