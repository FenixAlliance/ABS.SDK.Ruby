# OpenapiClient::ItemRetainSamplesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_item_retain_sample_async**](ItemRetainSamplesApi.md#create_item_retain_sample_async) | **POST** /api/v2/LogisticsService/ItemRetainSamples | Create an item retain sample |
| [**delete_item_retain_sample_async**](ItemRetainSamplesApi.md#delete_item_retain_sample_async) | **DELETE** /api/v2/LogisticsService/ItemRetainSamples/{retainSampleId} | Delete an item retain sample |
| [**get_item_retain_sample_by_id_async**](ItemRetainSamplesApi.md#get_item_retain_sample_by_id_async) | **GET** /api/v2/LogisticsService/ItemRetainSamples/{retainSampleId} | Get item retain sample by ID |
| [**get_item_retain_samples_async**](ItemRetainSamplesApi.md#get_item_retain_samples_async) | **GET** /api/v2/LogisticsService/ItemRetainSamples | Get all item retain samples |
| [**get_item_retain_samples_count_async**](ItemRetainSamplesApi.md#get_item_retain_samples_count_async) | **GET** /api/v2/LogisticsService/ItemRetainSamples/Count | Get item retain samples count |
| [**patch_item_retain_sample_async**](ItemRetainSamplesApi.md#patch_item_retain_sample_async) | **PATCH** /api/v2/LogisticsService/ItemRetainSamples/{retainSampleId} | Patch an item retain sample |
| [**update_item_retain_sample_async**](ItemRetainSamplesApi.md#update_item_retain_sample_async) | **PUT** /api/v2/LogisticsService/ItemRetainSamples/{retainSampleId} | Update an item retain sample |


## create_item_retain_sample_async

> <EmptyEnvelope> create_item_retain_sample_async(tenant_id, opts)

Create an item retain sample

Creates a new item retain sample.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRetainSamplesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_retain_sample_create_dto: OpenapiClient::ItemRetainSampleCreateDto.new({warehouse_id: 'warehouse_id_example', item_id: 'item_id_example'}) # ItemRetainSampleCreateDto | 
}

begin
  # Create an item retain sample
  result = api_instance.create_item_retain_sample_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRetainSamplesApi->create_item_retain_sample_async: #{e}"
end
```

#### Using the create_item_retain_sample_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_item_retain_sample_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create an item retain sample
  data, status_code, headers = api_instance.create_item_retain_sample_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRetainSamplesApi->create_item_retain_sample_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_retain_sample_create_dto** | [**ItemRetainSampleCreateDto**](ItemRetainSampleCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_item_retain_sample_async

> <EmptyEnvelope> delete_item_retain_sample_async(tenant_id, retain_sample_id, opts)

Delete an item retain sample

Deletes an item retain sample.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRetainSamplesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
retain_sample_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an item retain sample
  result = api_instance.delete_item_retain_sample_async(tenant_id, retain_sample_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRetainSamplesApi->delete_item_retain_sample_async: #{e}"
end
```

#### Using the delete_item_retain_sample_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_item_retain_sample_async_with_http_info(tenant_id, retain_sample_id, opts)

```ruby
begin
  # Delete an item retain sample
  data, status_code, headers = api_instance.delete_item_retain_sample_async_with_http_info(tenant_id, retain_sample_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRetainSamplesApi->delete_item_retain_sample_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **retain_sample_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_retain_sample_by_id_async

> <ItemRetainSampleDtoEnvelope> get_item_retain_sample_by_id_async(tenant_id, retain_sample_id, opts)

Get item retain sample by ID

Retrieves a specific item retain sample.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRetainSamplesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
retain_sample_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item retain sample by ID
  result = api_instance.get_item_retain_sample_by_id_async(tenant_id, retain_sample_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRetainSamplesApi->get_item_retain_sample_by_id_async: #{e}"
end
```

#### Using the get_item_retain_sample_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemRetainSampleDtoEnvelope>, Integer, Hash)> get_item_retain_sample_by_id_async_with_http_info(tenant_id, retain_sample_id, opts)

```ruby
begin
  # Get item retain sample by ID
  data, status_code, headers = api_instance.get_item_retain_sample_by_id_async_with_http_info(tenant_id, retain_sample_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemRetainSampleDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRetainSamplesApi->get_item_retain_sample_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **retain_sample_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemRetainSampleDtoEnvelope**](ItemRetainSampleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_retain_samples_async

> <ItemRetainSampleDtoListEnvelope> get_item_retain_samples_async(tenant_id, opts)

Get all item retain samples

Retrieves all item retain samples for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRetainSamplesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all item retain samples
  result = api_instance.get_item_retain_samples_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRetainSamplesApi->get_item_retain_samples_async: #{e}"
end
```

#### Using the get_item_retain_samples_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemRetainSampleDtoListEnvelope>, Integer, Hash)> get_item_retain_samples_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all item retain samples
  data, status_code, headers = api_instance.get_item_retain_samples_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemRetainSampleDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRetainSamplesApi->get_item_retain_samples_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemRetainSampleDtoListEnvelope**](ItemRetainSampleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_retain_samples_count_async

> <Int32Envelope> get_item_retain_samples_count_async(tenant_id, opts)

Get item retain samples count

Returns the count of item retain samples.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRetainSamplesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item retain samples count
  result = api_instance.get_item_retain_samples_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRetainSamplesApi->get_item_retain_samples_count_async: #{e}"
end
```

#### Using the get_item_retain_samples_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_item_retain_samples_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get item retain samples count
  data, status_code, headers = api_instance.get_item_retain_samples_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRetainSamplesApi->get_item_retain_samples_count_async_with_http_info: #{e}"
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


## patch_item_retain_sample_async

> <EmptyEnvelope> patch_item_retain_sample_async(tenant_id, retain_sample_id, opts)

Patch an item retain sample

Applies a JSON Patch document to an item retain sample.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRetainSamplesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
retain_sample_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch an item retain sample
  result = api_instance.patch_item_retain_sample_async(tenant_id, retain_sample_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRetainSamplesApi->patch_item_retain_sample_async: #{e}"
end
```

#### Using the patch_item_retain_sample_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_item_retain_sample_async_with_http_info(tenant_id, retain_sample_id, opts)

```ruby
begin
  # Patch an item retain sample
  data, status_code, headers = api_instance.patch_item_retain_sample_async_with_http_info(tenant_id, retain_sample_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRetainSamplesApi->patch_item_retain_sample_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **retain_sample_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_item_retain_sample_async

> <EmptyEnvelope> update_item_retain_sample_async(tenant_id, retain_sample_id, opts)

Update an item retain sample

Updates an existing item retain sample.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRetainSamplesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
retain_sample_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_retain_sample_update_dto: OpenapiClient::ItemRetainSampleUpdateDto.new # ItemRetainSampleUpdateDto | 
}

begin
  # Update an item retain sample
  result = api_instance.update_item_retain_sample_async(tenant_id, retain_sample_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRetainSamplesApi->update_item_retain_sample_async: #{e}"
end
```

#### Using the update_item_retain_sample_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_item_retain_sample_async_with_http_info(tenant_id, retain_sample_id, opts)

```ruby
begin
  # Update an item retain sample
  data, status_code, headers = api_instance.update_item_retain_sample_async_with_http_info(tenant_id, retain_sample_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRetainSamplesApi->update_item_retain_sample_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **retain_sample_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_retain_sample_update_dto** | [**ItemRetainSampleUpdateDto**](ItemRetainSampleUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

