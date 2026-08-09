# OpenapiClient::ShippingRegionsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_shipping_region_async**](ShippingRegionsApi.md#create_shipping_region_async) | **POST** /api/v2/ShipmentsService/ShippingRegions | Create a shipping region |
| [**delete_shipping_region_async**](ShippingRegionsApi.md#delete_shipping_region_async) | **DELETE** /api/v2/ShipmentsService/ShippingRegions/{regionId} | Delete a shipping region |
| [**get_shipping_region_by_id_async**](ShippingRegionsApi.md#get_shipping_region_by_id_async) | **GET** /api/v2/ShipmentsService/ShippingRegions/{regionId} | Get shipping region by ID |
| [**get_shipping_regions_async**](ShippingRegionsApi.md#get_shipping_regions_async) | **GET** /api/v2/ShipmentsService/ShippingRegions | Get all shipping regions |
| [**get_shipping_regions_count_async**](ShippingRegionsApi.md#get_shipping_regions_count_async) | **GET** /api/v2/ShipmentsService/ShippingRegions/Count | Get shipping regions count |
| [**patch_shipping_region_async**](ShippingRegionsApi.md#patch_shipping_region_async) | **PATCH** /api/v2/ShipmentsService/ShippingRegions/{regionId} | Patch a shipping region |
| [**update_shipping_region_async**](ShippingRegionsApi.md#update_shipping_region_async) | **PUT** /api/v2/ShipmentsService/ShippingRegions/{regionId} | Update a shipping region |


## create_shipping_region_async

> create_shipping_region_async(tenant_id, opts)

Create a shipping region

Creates a new shipping region.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingRegionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipping_region_create_dto: OpenapiClient::ShippingRegionCreateDto.new({name: 'name_example'}) # ShippingRegionCreateDto | 
}

begin
  # Create a shipping region
  api_instance.create_shipping_region_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingRegionsApi->create_shipping_region_async: #{e}"
end
```

#### Using the create_shipping_region_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_shipping_region_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a shipping region
  data, status_code, headers = api_instance.create_shipping_region_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingRegionsApi->create_shipping_region_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipping_region_create_dto** | [**ShippingRegionCreateDto**](ShippingRegionCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_shipping_region_async

> delete_shipping_region_async(tenant_id, region_id, opts)

Delete a shipping region

Deletes a shipping region.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingRegionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
region_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a shipping region
  api_instance.delete_shipping_region_async(tenant_id, region_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingRegionsApi->delete_shipping_region_async: #{e}"
end
```

#### Using the delete_shipping_region_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_shipping_region_async_with_http_info(tenant_id, region_id, opts)

```ruby
begin
  # Delete a shipping region
  data, status_code, headers = api_instance.delete_shipping_region_async_with_http_info(tenant_id, region_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingRegionsApi->delete_shipping_region_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **region_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shipping_region_by_id_async

> <ShippingRegionDtoEnvelope> get_shipping_region_by_id_async(tenant_id, region_id, opts)

Get shipping region by ID

Retrieves a specific shipping region.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingRegionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
region_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get shipping region by ID
  result = api_instance.get_shipping_region_by_id_async(tenant_id, region_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingRegionsApi->get_shipping_region_by_id_async: #{e}"
end
```

#### Using the get_shipping_region_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShippingRegionDtoEnvelope>, Integer, Hash)> get_shipping_region_by_id_async_with_http_info(tenant_id, region_id, opts)

```ruby
begin
  # Get shipping region by ID
  data, status_code, headers = api_instance.get_shipping_region_by_id_async_with_http_info(tenant_id, region_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShippingRegionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingRegionsApi->get_shipping_region_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **region_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShippingRegionDtoEnvelope**](ShippingRegionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shipping_regions_async

> <ShippingRegionDtoListEnvelope> get_shipping_regions_async(tenant_id, opts)

Get all shipping regions

Retrieves all shipping regions for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingRegionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipping_region_dto_collection_query_parameters: OpenapiClient::ShippingRegionDtoCollectionQueryParameters.new # ShippingRegionDtoCollectionQueryParameters | 
}

begin
  # Get all shipping regions
  result = api_instance.get_shipping_regions_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingRegionsApi->get_shipping_regions_async: #{e}"
end
```

#### Using the get_shipping_regions_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShippingRegionDtoListEnvelope>, Integer, Hash)> get_shipping_regions_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all shipping regions
  data, status_code, headers = api_instance.get_shipping_regions_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShippingRegionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingRegionsApi->get_shipping_regions_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipping_region_dto_collection_query_parameters** | [**ShippingRegionDtoCollectionQueryParameters**](ShippingRegionDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ShippingRegionDtoListEnvelope**](ShippingRegionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_shipping_regions_count_async

> <Int32Envelope> get_shipping_regions_count_async(tenant_id, opts)

Get shipping regions count

Returns the count of shipping regions.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingRegionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipping_region_dto_collection_query_parameters: OpenapiClient::ShippingRegionDtoCollectionQueryParameters.new # ShippingRegionDtoCollectionQueryParameters | 
}

begin
  # Get shipping regions count
  result = api_instance.get_shipping_regions_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingRegionsApi->get_shipping_regions_count_async: #{e}"
end
```

#### Using the get_shipping_regions_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_shipping_regions_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get shipping regions count
  data, status_code, headers = api_instance.get_shipping_regions_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingRegionsApi->get_shipping_regions_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipping_region_dto_collection_query_parameters** | [**ShippingRegionDtoCollectionQueryParameters**](ShippingRegionDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_shipping_region_async

> <EmptyEnvelope> patch_shipping_region_async(tenant_id, region_id, opts)

Patch a shipping region

Partially updates an existing shipping region using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingRegionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
region_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a shipping region
  result = api_instance.patch_shipping_region_async(tenant_id, region_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingRegionsApi->patch_shipping_region_async: #{e}"
end
```

#### Using the patch_shipping_region_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_shipping_region_async_with_http_info(tenant_id, region_id, opts)

```ruby
begin
  # Patch a shipping region
  data, status_code, headers = api_instance.patch_shipping_region_async_with_http_info(tenant_id, region_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingRegionsApi->patch_shipping_region_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **region_id** | **String** |  |  |
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


## update_shipping_region_async

> update_shipping_region_async(tenant_id, region_id, opts)

Update a shipping region

Updates an existing shipping region.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingRegionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
region_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipping_region_update_dto: OpenapiClient::ShippingRegionUpdateDto.new # ShippingRegionUpdateDto | 
}

begin
  # Update a shipping region
  api_instance.update_shipping_region_async(tenant_id, region_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingRegionsApi->update_shipping_region_async: #{e}"
end
```

#### Using the update_shipping_region_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_shipping_region_async_with_http_info(tenant_id, region_id, opts)

```ruby
begin
  # Update a shipping region
  data, status_code, headers = api_instance.update_shipping_region_async_with_http_info(tenant_id, region_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingRegionsApi->update_shipping_region_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **region_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipping_region_update_dto** | [**ShippingRegionUpdateDto**](ShippingRegionUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

