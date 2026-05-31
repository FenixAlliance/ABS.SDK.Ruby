# OpenapiClient::MarketingAreasApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_marketing_area_async**](MarketingAreasApi.md#create_marketing_area_async) | **POST** /api/v2/MarketingService/MarketingAreas | Create a marketing area |
| [**delete_marketing_area_async**](MarketingAreasApi.md#delete_marketing_area_async) | **DELETE** /api/v2/MarketingService/MarketingAreas/{marketingAreaId} | Delete a marketing area |
| [**get_marketing_area_by_id_async**](MarketingAreasApi.md#get_marketing_area_by_id_async) | **GET** /api/v2/MarketingService/MarketingAreas/{marketingAreaId} | Get marketing area by ID |
| [**get_marketing_areas_async**](MarketingAreasApi.md#get_marketing_areas_async) | **GET** /api/v2/MarketingService/MarketingAreas | Get marketing areas |
| [**get_marketing_areas_count_async**](MarketingAreasApi.md#get_marketing_areas_count_async) | **GET** /api/v2/MarketingService/MarketingAreas/Count | Count marketing areas |
| [**update_marketing_area_async**](MarketingAreasApi.md#update_marketing_area_async) | **PUT** /api/v2/MarketingService/MarketingAreas/{marketingAreaId} | Update a marketing area |


## create_marketing_area_async

> <EmptyEnvelope> create_marketing_area_async(tenant_id, opts)

Create a marketing area

Creates a new marketing area for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingAreasApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  marketing_area_create_dto: OpenapiClient::MarketingAreaCreateDto.new({name: 'name_example'}) # MarketingAreaCreateDto | 
}

begin
  # Create a marketing area
  result = api_instance.create_marketing_area_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingAreasApi->create_marketing_area_async: #{e}"
end
```

#### Using the create_marketing_area_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_marketing_area_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a marketing area
  data, status_code, headers = api_instance.create_marketing_area_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingAreasApi->create_marketing_area_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **marketing_area_create_dto** | [**MarketingAreaCreateDto**](MarketingAreaCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_marketing_area_async

> <EmptyEnvelope> delete_marketing_area_async(tenant_id, marketing_area_id, opts)

Delete a marketing area

Deletes a marketing area for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingAreasApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
marketing_area_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a marketing area
  result = api_instance.delete_marketing_area_async(tenant_id, marketing_area_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingAreasApi->delete_marketing_area_async: #{e}"
end
```

#### Using the delete_marketing_area_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_marketing_area_async_with_http_info(tenant_id, marketing_area_id, opts)

```ruby
begin
  # Delete a marketing area
  data, status_code, headers = api_instance.delete_marketing_area_async_with_http_info(tenant_id, marketing_area_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingAreasApi->delete_marketing_area_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **marketing_area_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_marketing_area_by_id_async

> <MarketingAreaDtoEnvelope> get_marketing_area_by_id_async(tenant_id, marketing_area_id, opts)

Get marketing area by ID

Retrieves a specific marketing area by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingAreasApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
marketing_area_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get marketing area by ID
  result = api_instance.get_marketing_area_by_id_async(tenant_id, marketing_area_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingAreasApi->get_marketing_area_by_id_async: #{e}"
end
```

#### Using the get_marketing_area_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MarketingAreaDtoEnvelope>, Integer, Hash)> get_marketing_area_by_id_async_with_http_info(tenant_id, marketing_area_id, opts)

```ruby
begin
  # Get marketing area by ID
  data, status_code, headers = api_instance.get_marketing_area_by_id_async_with_http_info(tenant_id, marketing_area_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MarketingAreaDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingAreasApi->get_marketing_area_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **marketing_area_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MarketingAreaDtoEnvelope**](MarketingAreaDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_marketing_areas_async

> <MarketingAreaDtoListEnvelope> get_marketing_areas_async(tenant_id, opts)

Get marketing areas

Retrieves marketing areas for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingAreasApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get marketing areas
  result = api_instance.get_marketing_areas_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingAreasApi->get_marketing_areas_async: #{e}"
end
```

#### Using the get_marketing_areas_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MarketingAreaDtoListEnvelope>, Integer, Hash)> get_marketing_areas_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get marketing areas
  data, status_code, headers = api_instance.get_marketing_areas_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MarketingAreaDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingAreasApi->get_marketing_areas_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MarketingAreaDtoListEnvelope**](MarketingAreaDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_marketing_areas_count_async

> <Int32Envelope> get_marketing_areas_count_async(tenant_id, opts)

Count marketing areas

Counts marketing areas for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingAreasApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count marketing areas
  result = api_instance.get_marketing_areas_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingAreasApi->get_marketing_areas_count_async: #{e}"
end
```

#### Using the get_marketing_areas_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_marketing_areas_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count marketing areas
  data, status_code, headers = api_instance.get_marketing_areas_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingAreasApi->get_marketing_areas_count_async_with_http_info: #{e}"
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


## update_marketing_area_async

> <EmptyEnvelope> update_marketing_area_async(tenant_id, marketing_area_id, opts)

Update a marketing area

Updates an existing marketing area for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingAreasApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
marketing_area_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  marketing_area_update_dto: OpenapiClient::MarketingAreaUpdateDto.new # MarketingAreaUpdateDto | 
}

begin
  # Update a marketing area
  result = api_instance.update_marketing_area_async(tenant_id, marketing_area_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingAreasApi->update_marketing_area_async: #{e}"
end
```

#### Using the update_marketing_area_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_marketing_area_async_with_http_info(tenant_id, marketing_area_id, opts)

```ruby
begin
  # Update a marketing area
  data, status_code, headers = api_instance.update_marketing_area_async_with_http_info(tenant_id, marketing_area_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingAreasApi->update_marketing_area_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **marketing_area_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **marketing_area_update_dto** | [**MarketingAreaUpdateDto**](MarketingAreaUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

