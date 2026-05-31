# OpenapiClient::RoadWaybillsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**add_road_waybill_line_async**](RoadWaybillsApi.md#add_road_waybill_line_async) | **POST** /api/v2/LogisticsService/RoadWaybills/{waybillId}/Lines | Add a line to road waybill |
| [**cancel_road_waybill_async**](RoadWaybillsApi.md#cancel_road_waybill_async) | **POST** /api/v2/LogisticsService/RoadWaybills/{waybillId}/Cancel | Cancel a road waybill |
| [**create_road_waybill_async**](RoadWaybillsApi.md#create_road_waybill_async) | **POST** /api/v2/LogisticsService/RoadWaybills | Create a road waybill |
| [**delete_road_waybill_async**](RoadWaybillsApi.md#delete_road_waybill_async) | **DELETE** /api/v2/LogisticsService/RoadWaybills/{waybillId} | Delete a road waybill |
| [**dispute_road_waybill_async**](RoadWaybillsApi.md#dispute_road_waybill_async) | **POST** /api/v2/LogisticsService/RoadWaybills/{waybillId}/Dispute | Dispute a road waybill |
| [**get_road_waybill_by_id_async**](RoadWaybillsApi.md#get_road_waybill_by_id_async) | **GET** /api/v2/LogisticsService/RoadWaybills/{waybillId} | Get road waybill by ID |
| [**get_road_waybill_lines_async**](RoadWaybillsApi.md#get_road_waybill_lines_async) | **GET** /api/v2/LogisticsService/RoadWaybills/{waybillId}/Lines | Get road waybill lines |
| [**get_road_waybill_lines_count_async**](RoadWaybillsApi.md#get_road_waybill_lines_count_async) | **GET** /api/v2/LogisticsService/RoadWaybills/{waybillId}/Lines/Count | Get road waybill lines count |
| [**get_road_waybills_async**](RoadWaybillsApi.md#get_road_waybills_async) | **GET** /api/v2/LogisticsService/RoadWaybills | Get all road waybills |
| [**get_road_waybills_count_async**](RoadWaybillsApi.md#get_road_waybills_count_async) | **GET** /api/v2/LogisticsService/RoadWaybills/Count | Get road waybills count |
| [**issue_road_waybill_async**](RoadWaybillsApi.md#issue_road_waybill_async) | **POST** /api/v2/LogisticsService/RoadWaybills/{waybillId}/Issue | Issue a road waybill |
| [**mark_road_waybill_delivered_async**](RoadWaybillsApi.md#mark_road_waybill_delivered_async) | **POST** /api/v2/LogisticsService/RoadWaybills/{waybillId}/MarkDelivered | Mark road waybill delivered |
| [**mark_road_waybill_in_transit_async**](RoadWaybillsApi.md#mark_road_waybill_in_transit_async) | **POST** /api/v2/LogisticsService/RoadWaybills/{waybillId}/MarkInTransit | Mark road waybill in transit |
| [**remove_road_waybill_line_async**](RoadWaybillsApi.md#remove_road_waybill_line_async) | **DELETE** /api/v2/LogisticsService/RoadWaybills/{waybillId}/Lines/{lineId} | Remove a road waybill line |
| [**update_road_waybill_async**](RoadWaybillsApi.md#update_road_waybill_async) | **PUT** /api/v2/LogisticsService/RoadWaybills/{waybillId} | Update a road waybill |
| [**update_road_waybill_line_async**](RoadWaybillsApi.md#update_road_waybill_line_async) | **PUT** /api/v2/LogisticsService/RoadWaybills/{waybillId}/Lines/{lineId} | Update a road waybill line |


## add_road_waybill_line_async

> <EmptyEnvelope> add_road_waybill_line_async(tenant_id, waybill_id, opts)

Add a line to road waybill

Adds a new line to a road waybill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoadWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  waybill_line_create_dto: OpenapiClient::WaybillLineCreateDto.new # WaybillLineCreateDto | 
}

begin
  # Add a line to road waybill
  result = api_instance.add_road_waybill_line_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->add_road_waybill_line_async: #{e}"
end
```

#### Using the add_road_waybill_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> add_road_waybill_line_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Add a line to road waybill
  data, status_code, headers = api_instance.add_road_waybill_line_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->add_road_waybill_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **waybill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **waybill_line_create_dto** | [**WaybillLineCreateDto**](WaybillLineCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## cancel_road_waybill_async

> <EmptyEnvelope> cancel_road_waybill_async(tenant_id, waybill_id, opts)

Cancel a road waybill

Cancels a road waybill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoadWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Cancel a road waybill
  result = api_instance.cancel_road_waybill_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->cancel_road_waybill_async: #{e}"
end
```

#### Using the cancel_road_waybill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> cancel_road_waybill_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Cancel a road waybill
  data, status_code, headers = api_instance.cancel_road_waybill_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->cancel_road_waybill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **waybill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_road_waybill_async

> <EmptyEnvelope> create_road_waybill_async(tenant_id, opts)

Create a road waybill

Creates a new road waybill for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoadWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  road_waybill_create_dto: OpenapiClient::RoadWaybillCreateDto.new # RoadWaybillCreateDto | 
}

begin
  # Create a road waybill
  result = api_instance.create_road_waybill_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->create_road_waybill_async: #{e}"
end
```

#### Using the create_road_waybill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_road_waybill_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a road waybill
  data, status_code, headers = api_instance.create_road_waybill_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->create_road_waybill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **road_waybill_create_dto** | [**RoadWaybillCreateDto**](RoadWaybillCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_road_waybill_async

> <EmptyEnvelope> delete_road_waybill_async(tenant_id, waybill_id, opts)

Delete a road waybill

Deletes a road waybill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoadWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a road waybill
  result = api_instance.delete_road_waybill_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->delete_road_waybill_async: #{e}"
end
```

#### Using the delete_road_waybill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_road_waybill_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Delete a road waybill
  data, status_code, headers = api_instance.delete_road_waybill_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->delete_road_waybill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **waybill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## dispute_road_waybill_async

> <EmptyEnvelope> dispute_road_waybill_async(tenant_id, waybill_id, opts)

Dispute a road waybill

Disputes a road waybill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoadWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Dispute a road waybill
  result = api_instance.dispute_road_waybill_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->dispute_road_waybill_async: #{e}"
end
```

#### Using the dispute_road_waybill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> dispute_road_waybill_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Dispute a road waybill
  data, status_code, headers = api_instance.dispute_road_waybill_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->dispute_road_waybill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **waybill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_road_waybill_by_id_async

> <RoadWaybillDtoEnvelope> get_road_waybill_by_id_async(tenant_id, waybill_id, opts)

Get road waybill by ID

Retrieves a specific road waybill by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoadWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get road waybill by ID
  result = api_instance.get_road_waybill_by_id_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->get_road_waybill_by_id_async: #{e}"
end
```

#### Using the get_road_waybill_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<RoadWaybillDtoEnvelope>, Integer, Hash)> get_road_waybill_by_id_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Get road waybill by ID
  data, status_code, headers = api_instance.get_road_waybill_by_id_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <RoadWaybillDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->get_road_waybill_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **waybill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**RoadWaybillDtoEnvelope**](RoadWaybillDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_road_waybill_lines_async

> <WaybillLineDtoListEnvelope> get_road_waybill_lines_async(tenant_id, waybill_id, opts)

Get road waybill lines

Retrieves all lines for a specific road waybill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoadWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get road waybill lines
  result = api_instance.get_road_waybill_lines_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->get_road_waybill_lines_async: #{e}"
end
```

#### Using the get_road_waybill_lines_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WaybillLineDtoListEnvelope>, Integer, Hash)> get_road_waybill_lines_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Get road waybill lines
  data, status_code, headers = api_instance.get_road_waybill_lines_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WaybillLineDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->get_road_waybill_lines_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **waybill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WaybillLineDtoListEnvelope**](WaybillLineDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_road_waybill_lines_count_async

> <Int32Envelope> get_road_waybill_lines_count_async(tenant_id, waybill_id, opts)

Get road waybill lines count

Returns the count of lines for a specific road waybill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoadWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get road waybill lines count
  result = api_instance.get_road_waybill_lines_count_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->get_road_waybill_lines_count_async: #{e}"
end
```

#### Using the get_road_waybill_lines_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_road_waybill_lines_count_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Get road waybill lines count
  data, status_code, headers = api_instance.get_road_waybill_lines_count_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->get_road_waybill_lines_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **waybill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_road_waybills_async

> <RoadWaybillDtoListEnvelope> get_road_waybills_async(tenant_id, opts)

Get all road waybills

Retrieves all road waybills for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoadWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all road waybills
  result = api_instance.get_road_waybills_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->get_road_waybills_async: #{e}"
end
```

#### Using the get_road_waybills_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<RoadWaybillDtoListEnvelope>, Integer, Hash)> get_road_waybills_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all road waybills
  data, status_code, headers = api_instance.get_road_waybills_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <RoadWaybillDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->get_road_waybills_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**RoadWaybillDtoListEnvelope**](RoadWaybillDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_road_waybills_count_async

> <Int32Envelope> get_road_waybills_count_async(tenant_id, opts)

Get road waybills count

Returns the count of road waybills for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoadWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get road waybills count
  result = api_instance.get_road_waybills_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->get_road_waybills_count_async: #{e}"
end
```

#### Using the get_road_waybills_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_road_waybills_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get road waybills count
  data, status_code, headers = api_instance.get_road_waybills_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->get_road_waybills_count_async_with_http_info: #{e}"
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


## issue_road_waybill_async

> <EmptyEnvelope> issue_road_waybill_async(tenant_id, waybill_id, opts)

Issue a road waybill

Issues a road waybill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoadWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Issue a road waybill
  result = api_instance.issue_road_waybill_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->issue_road_waybill_async: #{e}"
end
```

#### Using the issue_road_waybill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> issue_road_waybill_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Issue a road waybill
  data, status_code, headers = api_instance.issue_road_waybill_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->issue_road_waybill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **waybill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## mark_road_waybill_delivered_async

> <EmptyEnvelope> mark_road_waybill_delivered_async(tenant_id, waybill_id, opts)

Mark road waybill delivered

Marks a road waybill as delivered.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoadWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Mark road waybill delivered
  result = api_instance.mark_road_waybill_delivered_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->mark_road_waybill_delivered_async: #{e}"
end
```

#### Using the mark_road_waybill_delivered_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> mark_road_waybill_delivered_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Mark road waybill delivered
  data, status_code, headers = api_instance.mark_road_waybill_delivered_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->mark_road_waybill_delivered_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **waybill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## mark_road_waybill_in_transit_async

> <EmptyEnvelope> mark_road_waybill_in_transit_async(tenant_id, waybill_id, opts)

Mark road waybill in transit

Marks a road waybill as in transit.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoadWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Mark road waybill in transit
  result = api_instance.mark_road_waybill_in_transit_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->mark_road_waybill_in_transit_async: #{e}"
end
```

#### Using the mark_road_waybill_in_transit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> mark_road_waybill_in_transit_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Mark road waybill in transit
  data, status_code, headers = api_instance.mark_road_waybill_in_transit_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->mark_road_waybill_in_transit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **waybill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_road_waybill_line_async

> <EmptyEnvelope> remove_road_waybill_line_async(tenant_id, waybill_id, line_id, opts)

Remove a road waybill line

Removes a line from a road waybill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoadWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove a road waybill line
  result = api_instance.remove_road_waybill_line_async(tenant_id, waybill_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->remove_road_waybill_line_async: #{e}"
end
```

#### Using the remove_road_waybill_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> remove_road_waybill_line_async_with_http_info(tenant_id, waybill_id, line_id, opts)

```ruby
begin
  # Remove a road waybill line
  data, status_code, headers = api_instance.remove_road_waybill_line_async_with_http_info(tenant_id, waybill_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->remove_road_waybill_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **waybill_id** | **String** |  |  |
| **line_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_road_waybill_async

> <EmptyEnvelope> update_road_waybill_async(tenant_id, waybill_id, opts)

Update a road waybill

Updates an existing road waybill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoadWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  road_waybill_update_dto: OpenapiClient::RoadWaybillUpdateDto.new # RoadWaybillUpdateDto | 
}

begin
  # Update a road waybill
  result = api_instance.update_road_waybill_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->update_road_waybill_async: #{e}"
end
```

#### Using the update_road_waybill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_road_waybill_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Update a road waybill
  data, status_code, headers = api_instance.update_road_waybill_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->update_road_waybill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **waybill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **road_waybill_update_dto** | [**RoadWaybillUpdateDto**](RoadWaybillUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_road_waybill_line_async

> <EmptyEnvelope> update_road_waybill_line_async(tenant_id, waybill_id, line_id, opts)

Update a road waybill line

Updates an existing line on a road waybill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoadWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  waybill_line_update_dto: OpenapiClient::WaybillLineUpdateDto.new # WaybillLineUpdateDto | 
}

begin
  # Update a road waybill line
  result = api_instance.update_road_waybill_line_async(tenant_id, waybill_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->update_road_waybill_line_async: #{e}"
end
```

#### Using the update_road_waybill_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_road_waybill_line_async_with_http_info(tenant_id, waybill_id, line_id, opts)

```ruby
begin
  # Update a road waybill line
  data, status_code, headers = api_instance.update_road_waybill_line_async_with_http_info(tenant_id, waybill_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoadWaybillsApi->update_road_waybill_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **waybill_id** | **String** |  |  |
| **line_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **waybill_line_update_dto** | [**WaybillLineUpdateDto**](WaybillLineUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

