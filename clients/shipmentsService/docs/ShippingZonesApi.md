# OpenapiClient::ShippingZonesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_shipping_zone_async**](ShippingZonesApi.md#create_shipping_zone_async) | **POST** /api/v2/ShipmentsService/ShippingZones | Create a shipping zone |
| [**delete_shipping_zone_async**](ShippingZonesApi.md#delete_shipping_zone_async) | **DELETE** /api/v2/ShipmentsService/ShippingZones/{zoneId} | Delete a shipping zone |
| [**get_shipping_zone_by_id_async**](ShippingZonesApi.md#get_shipping_zone_by_id_async) | **GET** /api/v2/ShipmentsService/ShippingZones/{zoneId} | Get shipping zone by ID |
| [**get_shipping_zones_async**](ShippingZonesApi.md#get_shipping_zones_async) | **GET** /api/v2/ShipmentsService/ShippingZones | Get all shipping zones |
| [**get_shipping_zones_count_async**](ShippingZonesApi.md#get_shipping_zones_count_async) | **GET** /api/v2/ShipmentsService/ShippingZones/Count | Get shipping zones count |
| [**patch_shipping_zone_async**](ShippingZonesApi.md#patch_shipping_zone_async) | **PATCH** /api/v2/ShipmentsService/ShippingZones/{zoneId} | Patch a shipping zone |
| [**update_shipping_zone_async**](ShippingZonesApi.md#update_shipping_zone_async) | **PUT** /api/v2/ShipmentsService/ShippingZones/{zoneId} | Update a shipping zone |


## create_shipping_zone_async

> create_shipping_zone_async(tenant_id, opts)

Create a shipping zone

Creates a new shipping zone.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingZonesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipping_zone_create_dto: OpenapiClient::ShippingZoneCreateDto.new({name: 'name_example'}) # ShippingZoneCreateDto | 
}

begin
  # Create a shipping zone
  api_instance.create_shipping_zone_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingZonesApi->create_shipping_zone_async: #{e}"
end
```

#### Using the create_shipping_zone_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_shipping_zone_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a shipping zone
  data, status_code, headers = api_instance.create_shipping_zone_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingZonesApi->create_shipping_zone_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipping_zone_create_dto** | [**ShippingZoneCreateDto**](ShippingZoneCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_shipping_zone_async

> delete_shipping_zone_async(tenant_id, zone_id, opts)

Delete a shipping zone

Deletes a shipping zone.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingZonesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
zone_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a shipping zone
  api_instance.delete_shipping_zone_async(tenant_id, zone_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingZonesApi->delete_shipping_zone_async: #{e}"
end
```

#### Using the delete_shipping_zone_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_shipping_zone_async_with_http_info(tenant_id, zone_id, opts)

```ruby
begin
  # Delete a shipping zone
  data, status_code, headers = api_instance.delete_shipping_zone_async_with_http_info(tenant_id, zone_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingZonesApi->delete_shipping_zone_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **zone_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shipping_zone_by_id_async

> <ShippingZoneDtoEnvelope> get_shipping_zone_by_id_async(tenant_id, zone_id, opts)

Get shipping zone by ID

Retrieves a specific shipping zone.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingZonesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
zone_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get shipping zone by ID
  result = api_instance.get_shipping_zone_by_id_async(tenant_id, zone_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingZonesApi->get_shipping_zone_by_id_async: #{e}"
end
```

#### Using the get_shipping_zone_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShippingZoneDtoEnvelope>, Integer, Hash)> get_shipping_zone_by_id_async_with_http_info(tenant_id, zone_id, opts)

```ruby
begin
  # Get shipping zone by ID
  data, status_code, headers = api_instance.get_shipping_zone_by_id_async_with_http_info(tenant_id, zone_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShippingZoneDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingZonesApi->get_shipping_zone_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **zone_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShippingZoneDtoEnvelope**](ShippingZoneDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shipping_zones_async

> <ShippingZoneDtoListEnvelope> get_shipping_zones_async(tenant_id, opts)

Get all shipping zones

Retrieves all shipping zones for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingZonesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipping_zone_dto_collection_query_parameters: OpenapiClient::ShippingZoneDtoCollectionQueryParameters.new # ShippingZoneDtoCollectionQueryParameters | 
}

begin
  # Get all shipping zones
  result = api_instance.get_shipping_zones_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingZonesApi->get_shipping_zones_async: #{e}"
end
```

#### Using the get_shipping_zones_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShippingZoneDtoListEnvelope>, Integer, Hash)> get_shipping_zones_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all shipping zones
  data, status_code, headers = api_instance.get_shipping_zones_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShippingZoneDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingZonesApi->get_shipping_zones_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipping_zone_dto_collection_query_parameters** | [**ShippingZoneDtoCollectionQueryParameters**](ShippingZoneDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ShippingZoneDtoListEnvelope**](ShippingZoneDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_shipping_zones_count_async

> <Int32Envelope> get_shipping_zones_count_async(tenant_id, opts)

Get shipping zones count

Returns the count of shipping zones.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingZonesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipping_zone_dto_collection_query_parameters: OpenapiClient::ShippingZoneDtoCollectionQueryParameters.new # ShippingZoneDtoCollectionQueryParameters | 
}

begin
  # Get shipping zones count
  result = api_instance.get_shipping_zones_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingZonesApi->get_shipping_zones_count_async: #{e}"
end
```

#### Using the get_shipping_zones_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_shipping_zones_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get shipping zones count
  data, status_code, headers = api_instance.get_shipping_zones_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingZonesApi->get_shipping_zones_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipping_zone_dto_collection_query_parameters** | [**ShippingZoneDtoCollectionQueryParameters**](ShippingZoneDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_shipping_zone_async

> <EmptyEnvelope> patch_shipping_zone_async(tenant_id, zone_id, opts)

Patch a shipping zone

Partially updates an existing shipping zone using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingZonesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
zone_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a shipping zone
  result = api_instance.patch_shipping_zone_async(tenant_id, zone_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingZonesApi->patch_shipping_zone_async: #{e}"
end
```

#### Using the patch_shipping_zone_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_shipping_zone_async_with_http_info(tenant_id, zone_id, opts)

```ruby
begin
  # Patch a shipping zone
  data, status_code, headers = api_instance.patch_shipping_zone_async_with_http_info(tenant_id, zone_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingZonesApi->patch_shipping_zone_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **zone_id** | **String** |  |  |
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


## update_shipping_zone_async

> update_shipping_zone_async(tenant_id, zone_id, opts)

Update a shipping zone

Updates an existing shipping zone.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingZonesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
zone_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipping_zone_update_dto: OpenapiClient::ShippingZoneUpdateDto.new # ShippingZoneUpdateDto | 
}

begin
  # Update a shipping zone
  api_instance.update_shipping_zone_async(tenant_id, zone_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingZonesApi->update_shipping_zone_async: #{e}"
end
```

#### Using the update_shipping_zone_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_shipping_zone_async_with_http_info(tenant_id, zone_id, opts)

```ruby
begin
  # Update a shipping zone
  data, status_code, headers = api_instance.update_shipping_zone_async_with_http_info(tenant_id, zone_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingZonesApi->update_shipping_zone_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **zone_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipping_zone_update_dto** | [**ShippingZoneUpdateDto**](ShippingZoneUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

