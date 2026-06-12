# OpenapiClient::RailWaybillsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**add_rail_waybill_line_async**](RailWaybillsApi.md#add_rail_waybill_line_async) | **POST** /api/v2/LogisticsService/RailWaybills/{waybillId}/Lines | Add a line to rail waybill |
| [**cancel_rail_waybill_async**](RailWaybillsApi.md#cancel_rail_waybill_async) | **POST** /api/v2/LogisticsService/RailWaybills/{waybillId}/Cancel | Cancel a rail waybill |
| [**create_rail_waybill_async**](RailWaybillsApi.md#create_rail_waybill_async) | **POST** /api/v2/LogisticsService/RailWaybills | Create a rail waybill |
| [**delete_rail_waybill_async**](RailWaybillsApi.md#delete_rail_waybill_async) | **DELETE** /api/v2/LogisticsService/RailWaybills/{waybillId} | Delete a rail waybill |
| [**get_rail_waybill_by_id_async**](RailWaybillsApi.md#get_rail_waybill_by_id_async) | **GET** /api/v2/LogisticsService/RailWaybills/{waybillId} | Get rail waybill by ID |
| [**get_rail_waybill_lines_async**](RailWaybillsApi.md#get_rail_waybill_lines_async) | **GET** /api/v2/LogisticsService/RailWaybills/{waybillId}/Lines | Get rail waybill lines |
| [**get_rail_waybill_lines_count_async**](RailWaybillsApi.md#get_rail_waybill_lines_count_async) | **GET** /api/v2/LogisticsService/RailWaybills/{waybillId}/Lines/Count | Get rail waybill lines count |
| [**get_rail_waybills_async**](RailWaybillsApi.md#get_rail_waybills_async) | **GET** /api/v2/LogisticsService/RailWaybills | Get all rail waybills |
| [**get_rail_waybills_count_async**](RailWaybillsApi.md#get_rail_waybills_count_async) | **GET** /api/v2/LogisticsService/RailWaybills/Count | Get rail waybills count |
| [**issue_rail_waybill_async**](RailWaybillsApi.md#issue_rail_waybill_async) | **POST** /api/v2/LogisticsService/RailWaybills/{waybillId}/Issue | Issue a rail waybill |
| [**mark_rail_waybill_delivered_async**](RailWaybillsApi.md#mark_rail_waybill_delivered_async) | **POST** /api/v2/LogisticsService/RailWaybills/{waybillId}/MarkDelivered | Mark rail waybill delivered |
| [**mark_rail_waybill_in_transit_async**](RailWaybillsApi.md#mark_rail_waybill_in_transit_async) | **POST** /api/v2/LogisticsService/RailWaybills/{waybillId}/MarkInTransit | Mark rail waybill in transit |
| [**patch_rail_waybill_async**](RailWaybillsApi.md#patch_rail_waybill_async) | **PATCH** /api/v2/LogisticsService/RailWaybills/{waybillId} | Patch a rail waybill |
| [**patch_rail_waybill_line_async**](RailWaybillsApi.md#patch_rail_waybill_line_async) | **PATCH** /api/v2/LogisticsService/RailWaybills/{waybillId}/Lines/{lineId} | Patch a rail waybill line |
| [**remove_rail_waybill_line_async**](RailWaybillsApi.md#remove_rail_waybill_line_async) | **DELETE** /api/v2/LogisticsService/RailWaybills/{waybillId}/Lines/{lineId} | Remove a rail waybill line |
| [**update_rail_waybill_async**](RailWaybillsApi.md#update_rail_waybill_async) | **PUT** /api/v2/LogisticsService/RailWaybills/{waybillId} | Update a rail waybill |
| [**update_rail_waybill_line_async**](RailWaybillsApi.md#update_rail_waybill_line_async) | **PUT** /api/v2/LogisticsService/RailWaybills/{waybillId}/Lines/{lineId} | Update a rail waybill line |


## add_rail_waybill_line_async

> <EmptyEnvelope> add_rail_waybill_line_async(tenant_id, waybill_id, opts)

Add a line to rail waybill

Adds a new line to a rail waybill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RailWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  waybill_line_create_dto: OpenapiClient::WaybillLineCreateDto.new # WaybillLineCreateDto | 
}

begin
  # Add a line to rail waybill
  result = api_instance.add_rail_waybill_line_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->add_rail_waybill_line_async: #{e}"
end
```

#### Using the add_rail_waybill_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> add_rail_waybill_line_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Add a line to rail waybill
  data, status_code, headers = api_instance.add_rail_waybill_line_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->add_rail_waybill_line_async_with_http_info: #{e}"
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


## cancel_rail_waybill_async

> <EmptyEnvelope> cancel_rail_waybill_async(tenant_id, waybill_id, opts)

Cancel a rail waybill

Cancels a rail waybill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RailWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Cancel a rail waybill
  result = api_instance.cancel_rail_waybill_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->cancel_rail_waybill_async: #{e}"
end
```

#### Using the cancel_rail_waybill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> cancel_rail_waybill_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Cancel a rail waybill
  data, status_code, headers = api_instance.cancel_rail_waybill_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->cancel_rail_waybill_async_with_http_info: #{e}"
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


## create_rail_waybill_async

> <EmptyEnvelope> create_rail_waybill_async(tenant_id, opts)

Create a rail waybill

Creates a new rail waybill for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RailWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  rail_waybill_create_dto: OpenapiClient::RailWaybillCreateDto.new # RailWaybillCreateDto | 
}

begin
  # Create a rail waybill
  result = api_instance.create_rail_waybill_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->create_rail_waybill_async: #{e}"
end
```

#### Using the create_rail_waybill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_rail_waybill_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a rail waybill
  data, status_code, headers = api_instance.create_rail_waybill_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->create_rail_waybill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **rail_waybill_create_dto** | [**RailWaybillCreateDto**](RailWaybillCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_rail_waybill_async

> <EmptyEnvelope> delete_rail_waybill_async(tenant_id, waybill_id, opts)

Delete a rail waybill

Deletes a rail waybill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RailWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a rail waybill
  result = api_instance.delete_rail_waybill_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->delete_rail_waybill_async: #{e}"
end
```

#### Using the delete_rail_waybill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_rail_waybill_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Delete a rail waybill
  data, status_code, headers = api_instance.delete_rail_waybill_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->delete_rail_waybill_async_with_http_info: #{e}"
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


## get_rail_waybill_by_id_async

> <RailWaybillDtoEnvelope> get_rail_waybill_by_id_async(tenant_id, waybill_id, opts)

Get rail waybill by ID

Retrieves a specific rail waybill by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RailWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get rail waybill by ID
  result = api_instance.get_rail_waybill_by_id_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->get_rail_waybill_by_id_async: #{e}"
end
```

#### Using the get_rail_waybill_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<RailWaybillDtoEnvelope>, Integer, Hash)> get_rail_waybill_by_id_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Get rail waybill by ID
  data, status_code, headers = api_instance.get_rail_waybill_by_id_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <RailWaybillDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->get_rail_waybill_by_id_async_with_http_info: #{e}"
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

[**RailWaybillDtoEnvelope**](RailWaybillDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_rail_waybill_lines_async

> <WaybillLineDtoListEnvelope> get_rail_waybill_lines_async(tenant_id, waybill_id, opts)

Get rail waybill lines

Retrieves all lines for a specific rail waybill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RailWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get rail waybill lines
  result = api_instance.get_rail_waybill_lines_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->get_rail_waybill_lines_async: #{e}"
end
```

#### Using the get_rail_waybill_lines_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WaybillLineDtoListEnvelope>, Integer, Hash)> get_rail_waybill_lines_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Get rail waybill lines
  data, status_code, headers = api_instance.get_rail_waybill_lines_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WaybillLineDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->get_rail_waybill_lines_async_with_http_info: #{e}"
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


## get_rail_waybill_lines_count_async

> <Int32Envelope> get_rail_waybill_lines_count_async(tenant_id, waybill_id, opts)

Get rail waybill lines count

Returns the count of lines for a specific rail waybill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RailWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get rail waybill lines count
  result = api_instance.get_rail_waybill_lines_count_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->get_rail_waybill_lines_count_async: #{e}"
end
```

#### Using the get_rail_waybill_lines_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_rail_waybill_lines_count_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Get rail waybill lines count
  data, status_code, headers = api_instance.get_rail_waybill_lines_count_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->get_rail_waybill_lines_count_async_with_http_info: #{e}"
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


## get_rail_waybills_async

> <RailWaybillDtoListEnvelope> get_rail_waybills_async(tenant_id, opts)

Get all rail waybills

Retrieves all rail waybills for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RailWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all rail waybills
  result = api_instance.get_rail_waybills_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->get_rail_waybills_async: #{e}"
end
```

#### Using the get_rail_waybills_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<RailWaybillDtoListEnvelope>, Integer, Hash)> get_rail_waybills_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all rail waybills
  data, status_code, headers = api_instance.get_rail_waybills_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <RailWaybillDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->get_rail_waybills_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**RailWaybillDtoListEnvelope**](RailWaybillDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_rail_waybills_count_async

> <Int32Envelope> get_rail_waybills_count_async(tenant_id, opts)

Get rail waybills count

Returns the count of rail waybills for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RailWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get rail waybills count
  result = api_instance.get_rail_waybills_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->get_rail_waybills_count_async: #{e}"
end
```

#### Using the get_rail_waybills_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_rail_waybills_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get rail waybills count
  data, status_code, headers = api_instance.get_rail_waybills_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->get_rail_waybills_count_async_with_http_info: #{e}"
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


## issue_rail_waybill_async

> <EmptyEnvelope> issue_rail_waybill_async(tenant_id, waybill_id, opts)

Issue a rail waybill

Issues a rail waybill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RailWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Issue a rail waybill
  result = api_instance.issue_rail_waybill_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->issue_rail_waybill_async: #{e}"
end
```

#### Using the issue_rail_waybill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> issue_rail_waybill_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Issue a rail waybill
  data, status_code, headers = api_instance.issue_rail_waybill_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->issue_rail_waybill_async_with_http_info: #{e}"
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


## mark_rail_waybill_delivered_async

> <EmptyEnvelope> mark_rail_waybill_delivered_async(tenant_id, waybill_id, opts)

Mark rail waybill delivered

Marks a rail waybill as delivered.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RailWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Mark rail waybill delivered
  result = api_instance.mark_rail_waybill_delivered_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->mark_rail_waybill_delivered_async: #{e}"
end
```

#### Using the mark_rail_waybill_delivered_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> mark_rail_waybill_delivered_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Mark rail waybill delivered
  data, status_code, headers = api_instance.mark_rail_waybill_delivered_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->mark_rail_waybill_delivered_async_with_http_info: #{e}"
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


## mark_rail_waybill_in_transit_async

> <EmptyEnvelope> mark_rail_waybill_in_transit_async(tenant_id, waybill_id, opts)

Mark rail waybill in transit

Marks a rail waybill as in transit.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RailWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Mark rail waybill in transit
  result = api_instance.mark_rail_waybill_in_transit_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->mark_rail_waybill_in_transit_async: #{e}"
end
```

#### Using the mark_rail_waybill_in_transit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> mark_rail_waybill_in_transit_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Mark rail waybill in transit
  data, status_code, headers = api_instance.mark_rail_waybill_in_transit_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->mark_rail_waybill_in_transit_async_with_http_info: #{e}"
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


## patch_rail_waybill_async

> <EmptyEnvelope> patch_rail_waybill_async(tenant_id, waybill_id, opts)

Patch a rail waybill

Partially updates an existing rail waybill using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RailWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a rail waybill
  result = api_instance.patch_rail_waybill_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->patch_rail_waybill_async: #{e}"
end
```

#### Using the patch_rail_waybill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_rail_waybill_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Patch a rail waybill
  data, status_code, headers = api_instance.patch_rail_waybill_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->patch_rail_waybill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **waybill_id** | **String** |  |  |
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


## patch_rail_waybill_line_async

> <EmptyEnvelope> patch_rail_waybill_line_async(tenant_id, waybill_id, line_id, opts)

Patch a rail waybill line

Partially updates a line on a rail waybill using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RailWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a rail waybill line
  result = api_instance.patch_rail_waybill_line_async(tenant_id, waybill_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->patch_rail_waybill_line_async: #{e}"
end
```

#### Using the patch_rail_waybill_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_rail_waybill_line_async_with_http_info(tenant_id, waybill_id, line_id, opts)

```ruby
begin
  # Patch a rail waybill line
  data, status_code, headers = api_instance.patch_rail_waybill_line_async_with_http_info(tenant_id, waybill_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->patch_rail_waybill_line_async_with_http_info: #{e}"
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
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## remove_rail_waybill_line_async

> <EmptyEnvelope> remove_rail_waybill_line_async(tenant_id, waybill_id, line_id, opts)

Remove a rail waybill line

Removes a line from a rail waybill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RailWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove a rail waybill line
  result = api_instance.remove_rail_waybill_line_async(tenant_id, waybill_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->remove_rail_waybill_line_async: #{e}"
end
```

#### Using the remove_rail_waybill_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> remove_rail_waybill_line_async_with_http_info(tenant_id, waybill_id, line_id, opts)

```ruby
begin
  # Remove a rail waybill line
  data, status_code, headers = api_instance.remove_rail_waybill_line_async_with_http_info(tenant_id, waybill_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->remove_rail_waybill_line_async_with_http_info: #{e}"
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


## update_rail_waybill_async

> <EmptyEnvelope> update_rail_waybill_async(tenant_id, waybill_id, opts)

Update a rail waybill

Updates an existing rail waybill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RailWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  rail_waybill_update_dto: OpenapiClient::RailWaybillUpdateDto.new # RailWaybillUpdateDto | 
}

begin
  # Update a rail waybill
  result = api_instance.update_rail_waybill_async(tenant_id, waybill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->update_rail_waybill_async: #{e}"
end
```

#### Using the update_rail_waybill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_rail_waybill_async_with_http_info(tenant_id, waybill_id, opts)

```ruby
begin
  # Update a rail waybill
  data, status_code, headers = api_instance.update_rail_waybill_async_with_http_info(tenant_id, waybill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->update_rail_waybill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **waybill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **rail_waybill_update_dto** | [**RailWaybillUpdateDto**](RailWaybillUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_rail_waybill_line_async

> <EmptyEnvelope> update_rail_waybill_line_async(tenant_id, waybill_id, line_id, opts)

Update a rail waybill line

Updates an existing line on a rail waybill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RailWaybillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
waybill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  waybill_line_update_dto: OpenapiClient::WaybillLineUpdateDto.new # WaybillLineUpdateDto | 
}

begin
  # Update a rail waybill line
  result = api_instance.update_rail_waybill_line_async(tenant_id, waybill_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->update_rail_waybill_line_async: #{e}"
end
```

#### Using the update_rail_waybill_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_rail_waybill_line_async_with_http_info(tenant_id, waybill_id, line_id, opts)

```ruby
begin
  # Update a rail waybill line
  data, status_code, headers = api_instance.update_rail_waybill_line_async_with_http_info(tenant_id, waybill_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RailWaybillsApi->update_rail_waybill_line_async_with_http_info: #{e}"
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

