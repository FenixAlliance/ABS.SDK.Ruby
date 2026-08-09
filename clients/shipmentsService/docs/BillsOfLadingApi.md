# OpenapiClient::BillsOfLadingApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_bill_of_lading_async**](BillsOfLadingApi.md#create_bill_of_lading_async) | **POST** /api/v2/ShipmentsService/BillsOfLading | Create a bill of lading |
| [**create_bill_of_lading_line_async**](BillsOfLadingApi.md#create_bill_of_lading_line_async) | **POST** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId}/Lines | Create a bill of lading line |
| [**delete_bill_of_lading_async**](BillsOfLadingApi.md#delete_bill_of_lading_async) | **DELETE** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId} | Delete a bill of lading |
| [**delete_bill_of_lading_line_async**](BillsOfLadingApi.md#delete_bill_of_lading_line_async) | **DELETE** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId}/Lines/{lineId} | Delete a bill of lading line |
| [**get_bill_of_lading_by_id_async**](BillsOfLadingApi.md#get_bill_of_lading_by_id_async) | **GET** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId} | Get bill of lading by ID |
| [**get_bill_of_lading_line_by_id_async**](BillsOfLadingApi.md#get_bill_of_lading_line_by_id_async) | **GET** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId}/Lines/{lineId} | Get bill of lading line by ID |
| [**get_bill_of_lading_lines_async**](BillsOfLadingApi.md#get_bill_of_lading_lines_async) | **GET** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId}/Lines | Get bill of lading lines |
| [**get_bill_of_lading_lines_count_async**](BillsOfLadingApi.md#get_bill_of_lading_lines_count_async) | **GET** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId}/Lines/Count | Get bill of lading lines count |
| [**get_bills_of_lading_async**](BillsOfLadingApi.md#get_bills_of_lading_async) | **GET** /api/v2/ShipmentsService/BillsOfLading | Get all bills of lading |
| [**get_bills_of_lading_count_async**](BillsOfLadingApi.md#get_bills_of_lading_count_async) | **GET** /api/v2/ShipmentsService/BillsOfLading/Count | Get bills of lading count |
| [**patch_bill_of_lading_async**](BillsOfLadingApi.md#patch_bill_of_lading_async) | **PATCH** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId} | Patch a bill of lading |
| [**patch_bill_of_lading_line_async**](BillsOfLadingApi.md#patch_bill_of_lading_line_async) | **PATCH** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId}/Lines/{lineId} | Patch a bill of lading line |
| [**update_bill_of_lading_async**](BillsOfLadingApi.md#update_bill_of_lading_async) | **PUT** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId} | Update a bill of lading |
| [**update_bill_of_lading_line_async**](BillsOfLadingApi.md#update_bill_of_lading_line_async) | **PUT** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId}/Lines/{lineId} | Update a bill of lading line |


## create_bill_of_lading_async

> <EmptyEnvelope> create_bill_of_lading_async(tenant_id, opts)

Create a bill of lading

Creates a new bill of lading for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillsOfLadingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  bill_of_lading_create_dto: OpenapiClient::BillOfLadingCreateDto.new # BillOfLadingCreateDto | 
}

begin
  # Create a bill of lading
  result = api_instance.create_bill_of_lading_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->create_bill_of_lading_async: #{e}"
end
```

#### Using the create_bill_of_lading_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_bill_of_lading_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a bill of lading
  data, status_code, headers = api_instance.create_bill_of_lading_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->create_bill_of_lading_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **bill_of_lading_create_dto** | [**BillOfLadingCreateDto**](BillOfLadingCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_bill_of_lading_line_async

> <EmptyEnvelope> create_bill_of_lading_line_async(tenant_id, bill_of_lading_id, opts)

Create a bill of lading line

Creates a new line for a bill of lading.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillsOfLadingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_of_lading_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  bill_of_lading_line_create_dto: OpenapiClient::BillOfLadingLineCreateDto.new # BillOfLadingLineCreateDto | 
}

begin
  # Create a bill of lading line
  result = api_instance.create_bill_of_lading_line_async(tenant_id, bill_of_lading_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->create_bill_of_lading_line_async: #{e}"
end
```

#### Using the create_bill_of_lading_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_bill_of_lading_line_async_with_http_info(tenant_id, bill_of_lading_id, opts)

```ruby
begin
  # Create a bill of lading line
  data, status_code, headers = api_instance.create_bill_of_lading_line_async_with_http_info(tenant_id, bill_of_lading_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->create_bill_of_lading_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_of_lading_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **bill_of_lading_line_create_dto** | [**BillOfLadingLineCreateDto**](BillOfLadingLineCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_bill_of_lading_async

> <EmptyEnvelope> delete_bill_of_lading_async(tenant_id, bill_of_lading_id, opts)

Delete a bill of lading

Deletes a bill of lading.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillsOfLadingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_of_lading_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a bill of lading
  result = api_instance.delete_bill_of_lading_async(tenant_id, bill_of_lading_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->delete_bill_of_lading_async: #{e}"
end
```

#### Using the delete_bill_of_lading_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_bill_of_lading_async_with_http_info(tenant_id, bill_of_lading_id, opts)

```ruby
begin
  # Delete a bill of lading
  data, status_code, headers = api_instance.delete_bill_of_lading_async_with_http_info(tenant_id, bill_of_lading_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->delete_bill_of_lading_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_of_lading_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_bill_of_lading_line_async

> <EmptyEnvelope> delete_bill_of_lading_line_async(tenant_id, bill_of_lading_id, line_id, opts)

Delete a bill of lading line

Deletes a line from a bill of lading.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillsOfLadingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_of_lading_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a bill of lading line
  result = api_instance.delete_bill_of_lading_line_async(tenant_id, bill_of_lading_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->delete_bill_of_lading_line_async: #{e}"
end
```

#### Using the delete_bill_of_lading_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_bill_of_lading_line_async_with_http_info(tenant_id, bill_of_lading_id, line_id, opts)

```ruby
begin
  # Delete a bill of lading line
  data, status_code, headers = api_instance.delete_bill_of_lading_line_async_with_http_info(tenant_id, bill_of_lading_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->delete_bill_of_lading_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_of_lading_id** | **String** |  |  |
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


## get_bill_of_lading_by_id_async

> <BillOfLadingDtoEnvelope> get_bill_of_lading_by_id_async(tenant_id, bill_of_lading_id, opts)

Get bill of lading by ID

Retrieves a specific bill of lading by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillsOfLadingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_of_lading_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get bill of lading by ID
  result = api_instance.get_bill_of_lading_by_id_async(tenant_id, bill_of_lading_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->get_bill_of_lading_by_id_async: #{e}"
end
```

#### Using the get_bill_of_lading_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BillOfLadingDtoEnvelope>, Integer, Hash)> get_bill_of_lading_by_id_async_with_http_info(tenant_id, bill_of_lading_id, opts)

```ruby
begin
  # Get bill of lading by ID
  data, status_code, headers = api_instance.get_bill_of_lading_by_id_async_with_http_info(tenant_id, bill_of_lading_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BillOfLadingDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->get_bill_of_lading_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_of_lading_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BillOfLadingDtoEnvelope**](BillOfLadingDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_bill_of_lading_line_by_id_async

> <BillOfLadingLineDtoEnvelope> get_bill_of_lading_line_by_id_async(tenant_id, bill_of_lading_id, line_id, opts)

Get bill of lading line by ID

Retrieves a specific line from a bill of lading.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillsOfLadingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_of_lading_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get bill of lading line by ID
  result = api_instance.get_bill_of_lading_line_by_id_async(tenant_id, bill_of_lading_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->get_bill_of_lading_line_by_id_async: #{e}"
end
```

#### Using the get_bill_of_lading_line_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BillOfLadingLineDtoEnvelope>, Integer, Hash)> get_bill_of_lading_line_by_id_async_with_http_info(tenant_id, bill_of_lading_id, line_id, opts)

```ruby
begin
  # Get bill of lading line by ID
  data, status_code, headers = api_instance.get_bill_of_lading_line_by_id_async_with_http_info(tenant_id, bill_of_lading_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BillOfLadingLineDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->get_bill_of_lading_line_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_of_lading_id** | **String** |  |  |
| **line_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BillOfLadingLineDtoEnvelope**](BillOfLadingLineDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_bill_of_lading_lines_async

> <BillOfLadingLineDtoListEnvelope> get_bill_of_lading_lines_async(tenant_id, bill_of_lading_id, opts)

Get bill of lading lines

Retrieves all lines for a specific bill of lading.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillsOfLadingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_of_lading_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  bill_of_lading_line_dto_collection_query_parameters: OpenapiClient::BillOfLadingLineDtoCollectionQueryParameters.new # BillOfLadingLineDtoCollectionQueryParameters | 
}

begin
  # Get bill of lading lines
  result = api_instance.get_bill_of_lading_lines_async(tenant_id, bill_of_lading_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->get_bill_of_lading_lines_async: #{e}"
end
```

#### Using the get_bill_of_lading_lines_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BillOfLadingLineDtoListEnvelope>, Integer, Hash)> get_bill_of_lading_lines_async_with_http_info(tenant_id, bill_of_lading_id, opts)

```ruby
begin
  # Get bill of lading lines
  data, status_code, headers = api_instance.get_bill_of_lading_lines_async_with_http_info(tenant_id, bill_of_lading_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BillOfLadingLineDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->get_bill_of_lading_lines_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_of_lading_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **bill_of_lading_line_dto_collection_query_parameters** | [**BillOfLadingLineDtoCollectionQueryParameters**](BillOfLadingLineDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**BillOfLadingLineDtoListEnvelope**](BillOfLadingLineDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_bill_of_lading_lines_count_async

> <Int32Envelope> get_bill_of_lading_lines_count_async(tenant_id, bill_of_lading_id, opts)

Get bill of lading lines count

Returns the count of lines for a specific bill of lading.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillsOfLadingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_of_lading_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  bill_of_lading_line_dto_collection_query_parameters: OpenapiClient::BillOfLadingLineDtoCollectionQueryParameters.new # BillOfLadingLineDtoCollectionQueryParameters | 
}

begin
  # Get bill of lading lines count
  result = api_instance.get_bill_of_lading_lines_count_async(tenant_id, bill_of_lading_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->get_bill_of_lading_lines_count_async: #{e}"
end
```

#### Using the get_bill_of_lading_lines_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_bill_of_lading_lines_count_async_with_http_info(tenant_id, bill_of_lading_id, opts)

```ruby
begin
  # Get bill of lading lines count
  data, status_code, headers = api_instance.get_bill_of_lading_lines_count_async_with_http_info(tenant_id, bill_of_lading_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->get_bill_of_lading_lines_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_of_lading_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **bill_of_lading_line_dto_collection_query_parameters** | [**BillOfLadingLineDtoCollectionQueryParameters**](BillOfLadingLineDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_bills_of_lading_async

> <BillOfLadingDtoListEnvelope> get_bills_of_lading_async(tenant_id, opts)

Get all bills of lading

Retrieves all bills of lading for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillsOfLadingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  bill_of_lading_dto_collection_query_parameters: OpenapiClient::BillOfLadingDtoCollectionQueryParameters.new # BillOfLadingDtoCollectionQueryParameters | 
}

begin
  # Get all bills of lading
  result = api_instance.get_bills_of_lading_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->get_bills_of_lading_async: #{e}"
end
```

#### Using the get_bills_of_lading_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BillOfLadingDtoListEnvelope>, Integer, Hash)> get_bills_of_lading_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all bills of lading
  data, status_code, headers = api_instance.get_bills_of_lading_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BillOfLadingDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->get_bills_of_lading_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **bill_of_lading_dto_collection_query_parameters** | [**BillOfLadingDtoCollectionQueryParameters**](BillOfLadingDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**BillOfLadingDtoListEnvelope**](BillOfLadingDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_bills_of_lading_count_async

> <Int32Envelope> get_bills_of_lading_count_async(tenant_id, opts)

Get bills of lading count

Returns the count of bills of lading for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillsOfLadingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  bill_of_lading_dto_collection_query_parameters: OpenapiClient::BillOfLadingDtoCollectionQueryParameters.new # BillOfLadingDtoCollectionQueryParameters | 
}

begin
  # Get bills of lading count
  result = api_instance.get_bills_of_lading_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->get_bills_of_lading_count_async: #{e}"
end
```

#### Using the get_bills_of_lading_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_bills_of_lading_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get bills of lading count
  data, status_code, headers = api_instance.get_bills_of_lading_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->get_bills_of_lading_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **bill_of_lading_dto_collection_query_parameters** | [**BillOfLadingDtoCollectionQueryParameters**](BillOfLadingDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_bill_of_lading_async

> <EmptyEnvelope> patch_bill_of_lading_async(tenant_id, bill_of_lading_id, opts)

Patch a bill of lading

Partially updates an existing bill of lading using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillsOfLadingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_of_lading_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a bill of lading
  result = api_instance.patch_bill_of_lading_async(tenant_id, bill_of_lading_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->patch_bill_of_lading_async: #{e}"
end
```

#### Using the patch_bill_of_lading_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_bill_of_lading_async_with_http_info(tenant_id, bill_of_lading_id, opts)

```ruby
begin
  # Patch a bill of lading
  data, status_code, headers = api_instance.patch_bill_of_lading_async_with_http_info(tenant_id, bill_of_lading_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->patch_bill_of_lading_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_of_lading_id** | **String** |  |  |
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


## patch_bill_of_lading_line_async

> <EmptyEnvelope> patch_bill_of_lading_line_async(tenant_id, bill_of_lading_id, line_id, opts)

Patch a bill of lading line

Partially updates an existing line on a bill of lading using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillsOfLadingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_of_lading_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a bill of lading line
  result = api_instance.patch_bill_of_lading_line_async(tenant_id, bill_of_lading_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->patch_bill_of_lading_line_async: #{e}"
end
```

#### Using the patch_bill_of_lading_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_bill_of_lading_line_async_with_http_info(tenant_id, bill_of_lading_id, line_id, opts)

```ruby
begin
  # Patch a bill of lading line
  data, status_code, headers = api_instance.patch_bill_of_lading_line_async_with_http_info(tenant_id, bill_of_lading_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->patch_bill_of_lading_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_of_lading_id** | **String** |  |  |
| **line_id** | **String** |  |  |
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


## update_bill_of_lading_async

> <EmptyEnvelope> update_bill_of_lading_async(tenant_id, bill_of_lading_id, opts)

Update a bill of lading

Updates an existing bill of lading.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillsOfLadingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_of_lading_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  bill_of_lading_update_dto: OpenapiClient::BillOfLadingUpdateDto.new # BillOfLadingUpdateDto | 
}

begin
  # Update a bill of lading
  result = api_instance.update_bill_of_lading_async(tenant_id, bill_of_lading_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->update_bill_of_lading_async: #{e}"
end
```

#### Using the update_bill_of_lading_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_bill_of_lading_async_with_http_info(tenant_id, bill_of_lading_id, opts)

```ruby
begin
  # Update a bill of lading
  data, status_code, headers = api_instance.update_bill_of_lading_async_with_http_info(tenant_id, bill_of_lading_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->update_bill_of_lading_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_of_lading_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **bill_of_lading_update_dto** | [**BillOfLadingUpdateDto**](BillOfLadingUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_bill_of_lading_line_async

> <EmptyEnvelope> update_bill_of_lading_line_async(tenant_id, bill_of_lading_id, line_id, opts)

Update a bill of lading line

Updates an existing line on a bill of lading.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillsOfLadingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_of_lading_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  bill_of_lading_line_update_dto: OpenapiClient::BillOfLadingLineUpdateDto.new # BillOfLadingLineUpdateDto | 
}

begin
  # Update a bill of lading line
  result = api_instance.update_bill_of_lading_line_async(tenant_id, bill_of_lading_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->update_bill_of_lading_line_async: #{e}"
end
```

#### Using the update_bill_of_lading_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_bill_of_lading_line_async_with_http_info(tenant_id, bill_of_lading_id, line_id, opts)

```ruby
begin
  # Update a bill of lading line
  data, status_code, headers = api_instance.update_bill_of_lading_line_async_with_http_info(tenant_id, bill_of_lading_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillsOfLadingApi->update_bill_of_lading_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_of_lading_id** | **String** |  |  |
| **line_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **bill_of_lading_line_update_dto** | [**BillOfLadingLineUpdateDto**](BillOfLadingLineUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

