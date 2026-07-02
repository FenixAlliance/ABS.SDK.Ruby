# OpenapiClient::SeawayBillsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**add_seaway_bill_line_async**](SeawayBillsApi.md#add_seaway_bill_line_async) | **POST** /api/v2/LogisticsService/SeawayBills/{billId}/Lines | Add a line to seaway bill |
| [**cancel_seaway_bill_async**](SeawayBillsApi.md#cancel_seaway_bill_async) | **POST** /api/v2/LogisticsService/SeawayBills/{billId}/Cancel | Cancel a seaway bill |
| [**create_seaway_bill_async**](SeawayBillsApi.md#create_seaway_bill_async) | **POST** /api/v2/LogisticsService/SeawayBills | Create a seaway bill |
| [**delete_seaway_bill_async**](SeawayBillsApi.md#delete_seaway_bill_async) | **DELETE** /api/v2/LogisticsService/SeawayBills/{billId} | Delete a seaway bill |
| [**get_seaway_bill_by_id_async**](SeawayBillsApi.md#get_seaway_bill_by_id_async) | **GET** /api/v2/LogisticsService/SeawayBills/{billId} | Get seaway bill by ID |
| [**get_seaway_bill_lines_async**](SeawayBillsApi.md#get_seaway_bill_lines_async) | **GET** /api/v2/LogisticsService/SeawayBills/{billId}/Lines | Get seaway bill lines |
| [**get_seaway_bill_lines_count_async**](SeawayBillsApi.md#get_seaway_bill_lines_count_async) | **GET** /api/v2/LogisticsService/SeawayBills/{billId}/Lines/Count | Get seaway bill lines count |
| [**get_seaway_bills_async**](SeawayBillsApi.md#get_seaway_bills_async) | **GET** /api/v2/LogisticsService/SeawayBills | Get all seaway bills |
| [**get_seaway_bills_count_async**](SeawayBillsApi.md#get_seaway_bills_count_async) | **GET** /api/v2/LogisticsService/SeawayBills/Count | Get seaway bills count |
| [**issue_seaway_bill_async**](SeawayBillsApi.md#issue_seaway_bill_async) | **POST** /api/v2/LogisticsService/SeawayBills/{billId}/Issue | Issue a seaway bill |
| [**mark_seaway_bill_arrived_async**](SeawayBillsApi.md#mark_seaway_bill_arrived_async) | **POST** /api/v2/LogisticsService/SeawayBills/{billId}/MarkArrived | Mark seaway bill arrived |
| [**mark_seaway_bill_in_transit_async**](SeawayBillsApi.md#mark_seaway_bill_in_transit_async) | **POST** /api/v2/LogisticsService/SeawayBills/{billId}/MarkInTransit | Mark seaway bill in transit |
| [**patch_seaway_bill_async**](SeawayBillsApi.md#patch_seaway_bill_async) | **PATCH** /api/v2/LogisticsService/SeawayBills/{billId} | Patch a seaway bill |
| [**patch_seaway_bill_line_async**](SeawayBillsApi.md#patch_seaway_bill_line_async) | **PATCH** /api/v2/LogisticsService/SeawayBills/{billId}/Lines/{lineId} | Patch a seaway bill line |
| [**release_seaway_bill_async**](SeawayBillsApi.md#release_seaway_bill_async) | **POST** /api/v2/LogisticsService/SeawayBills/{billId}/Release | Release a seaway bill |
| [**remove_seaway_bill_line_async**](SeawayBillsApi.md#remove_seaway_bill_line_async) | **DELETE** /api/v2/LogisticsService/SeawayBills/{billId}/Lines/{lineId} | Remove a seaway bill line |
| [**update_seaway_bill_async**](SeawayBillsApi.md#update_seaway_bill_async) | **PUT** /api/v2/LogisticsService/SeawayBills/{billId} | Update a seaway bill |
| [**update_seaway_bill_line_async**](SeawayBillsApi.md#update_seaway_bill_line_async) | **PUT** /api/v2/LogisticsService/SeawayBills/{billId}/Lines/{lineId} | Update a seaway bill line |


## add_seaway_bill_line_async

> <EmptyEnvelope> add_seaway_bill_line_async(tenant_id, bill_id, opts)

Add a line to seaway bill

Adds a new line to a seaway bill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SeawayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  waybill_line_create_dto: OpenapiClient::WaybillLineCreateDto.new # WaybillLineCreateDto | 
}

begin
  # Add a line to seaway bill
  result = api_instance.add_seaway_bill_line_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->add_seaway_bill_line_async: #{e}"
end
```

#### Using the add_seaway_bill_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> add_seaway_bill_line_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Add a line to seaway bill
  data, status_code, headers = api_instance.add_seaway_bill_line_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->add_seaway_bill_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_id** | **String** |  |  |
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


## cancel_seaway_bill_async

> <EmptyEnvelope> cancel_seaway_bill_async(tenant_id, bill_id, opts)

Cancel a seaway bill

Cancels a seaway bill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SeawayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Cancel a seaway bill
  result = api_instance.cancel_seaway_bill_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->cancel_seaway_bill_async: #{e}"
end
```

#### Using the cancel_seaway_bill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> cancel_seaway_bill_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Cancel a seaway bill
  data, status_code, headers = api_instance.cancel_seaway_bill_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->cancel_seaway_bill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_seaway_bill_async

> <EmptyEnvelope> create_seaway_bill_async(tenant_id, opts)

Create a seaway bill

Creates a new seaway bill for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SeawayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  seaway_bill_create_dto: OpenapiClient::SeawayBillCreateDto.new # SeawayBillCreateDto | 
}

begin
  # Create a seaway bill
  result = api_instance.create_seaway_bill_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->create_seaway_bill_async: #{e}"
end
```

#### Using the create_seaway_bill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_seaway_bill_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a seaway bill
  data, status_code, headers = api_instance.create_seaway_bill_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->create_seaway_bill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **seaway_bill_create_dto** | [**SeawayBillCreateDto**](SeawayBillCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_seaway_bill_async

> <EmptyEnvelope> delete_seaway_bill_async(tenant_id, bill_id, opts)

Delete a seaway bill

Deletes a seaway bill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SeawayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a seaway bill
  result = api_instance.delete_seaway_bill_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->delete_seaway_bill_async: #{e}"
end
```

#### Using the delete_seaway_bill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_seaway_bill_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Delete a seaway bill
  data, status_code, headers = api_instance.delete_seaway_bill_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->delete_seaway_bill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_seaway_bill_by_id_async

> <SeawayBillDtoEnvelope> get_seaway_bill_by_id_async(tenant_id, bill_id, opts)

Get seaway bill by ID

Retrieves a specific seaway bill by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SeawayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get seaway bill by ID
  result = api_instance.get_seaway_bill_by_id_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->get_seaway_bill_by_id_async: #{e}"
end
```

#### Using the get_seaway_bill_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SeawayBillDtoEnvelope>, Integer, Hash)> get_seaway_bill_by_id_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Get seaway bill by ID
  data, status_code, headers = api_instance.get_seaway_bill_by_id_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SeawayBillDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->get_seaway_bill_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SeawayBillDtoEnvelope**](SeawayBillDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_seaway_bill_lines_async

> <WaybillLineDtoListEnvelope> get_seaway_bill_lines_async(tenant_id, bill_id, opts)

Get seaway bill lines

Retrieves all lines for a specific seaway bill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SeawayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get seaway bill lines
  result = api_instance.get_seaway_bill_lines_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->get_seaway_bill_lines_async: #{e}"
end
```

#### Using the get_seaway_bill_lines_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WaybillLineDtoListEnvelope>, Integer, Hash)> get_seaway_bill_lines_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Get seaway bill lines
  data, status_code, headers = api_instance.get_seaway_bill_lines_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WaybillLineDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->get_seaway_bill_lines_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WaybillLineDtoListEnvelope**](WaybillLineDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_seaway_bill_lines_count_async

> <Int32Envelope> get_seaway_bill_lines_count_async(tenant_id, bill_id, opts)

Get seaway bill lines count

Returns the count of lines for a specific seaway bill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SeawayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get seaway bill lines count
  result = api_instance.get_seaway_bill_lines_count_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->get_seaway_bill_lines_count_async: #{e}"
end
```

#### Using the get_seaway_bill_lines_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_seaway_bill_lines_count_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Get seaway bill lines count
  data, status_code, headers = api_instance.get_seaway_bill_lines_count_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->get_seaway_bill_lines_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_seaway_bills_async

> <SeawayBillDtoListEnvelope> get_seaway_bills_async(tenant_id, opts)

Get all seaway bills

Retrieves all seaway bills for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SeawayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all seaway bills
  result = api_instance.get_seaway_bills_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->get_seaway_bills_async: #{e}"
end
```

#### Using the get_seaway_bills_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SeawayBillDtoListEnvelope>, Integer, Hash)> get_seaway_bills_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all seaway bills
  data, status_code, headers = api_instance.get_seaway_bills_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SeawayBillDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->get_seaway_bills_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SeawayBillDtoListEnvelope**](SeawayBillDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_seaway_bills_count_async

> <Int32Envelope> get_seaway_bills_count_async(tenant_id, opts)

Get seaway bills count

Returns the count of seaway bills for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SeawayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get seaway bills count
  result = api_instance.get_seaway_bills_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->get_seaway_bills_count_async: #{e}"
end
```

#### Using the get_seaway_bills_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_seaway_bills_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get seaway bills count
  data, status_code, headers = api_instance.get_seaway_bills_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->get_seaway_bills_count_async_with_http_info: #{e}"
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


## issue_seaway_bill_async

> <EmptyEnvelope> issue_seaway_bill_async(tenant_id, bill_id, opts)

Issue a seaway bill

Issues a seaway bill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SeawayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Issue a seaway bill
  result = api_instance.issue_seaway_bill_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->issue_seaway_bill_async: #{e}"
end
```

#### Using the issue_seaway_bill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> issue_seaway_bill_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Issue a seaway bill
  data, status_code, headers = api_instance.issue_seaway_bill_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->issue_seaway_bill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## mark_seaway_bill_arrived_async

> <EmptyEnvelope> mark_seaway_bill_arrived_async(tenant_id, bill_id, opts)

Mark seaway bill arrived

Marks a seaway bill as arrived.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SeawayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Mark seaway bill arrived
  result = api_instance.mark_seaway_bill_arrived_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->mark_seaway_bill_arrived_async: #{e}"
end
```

#### Using the mark_seaway_bill_arrived_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> mark_seaway_bill_arrived_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Mark seaway bill arrived
  data, status_code, headers = api_instance.mark_seaway_bill_arrived_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->mark_seaway_bill_arrived_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## mark_seaway_bill_in_transit_async

> <EmptyEnvelope> mark_seaway_bill_in_transit_async(tenant_id, bill_id, opts)

Mark seaway bill in transit

Marks a seaway bill as in transit.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SeawayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Mark seaway bill in transit
  result = api_instance.mark_seaway_bill_in_transit_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->mark_seaway_bill_in_transit_async: #{e}"
end
```

#### Using the mark_seaway_bill_in_transit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> mark_seaway_bill_in_transit_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Mark seaway bill in transit
  data, status_code, headers = api_instance.mark_seaway_bill_in_transit_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->mark_seaway_bill_in_transit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_seaway_bill_async

> <EmptyEnvelope> patch_seaway_bill_async(tenant_id, bill_id, opts)

Patch a seaway bill

Partially updates an existing seaway bill using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SeawayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a seaway bill
  result = api_instance.patch_seaway_bill_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->patch_seaway_bill_async: #{e}"
end
```

#### Using the patch_seaway_bill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_seaway_bill_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Patch a seaway bill
  data, status_code, headers = api_instance.patch_seaway_bill_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->patch_seaway_bill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_id** | **String** |  |  |
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


## patch_seaway_bill_line_async

> <EmptyEnvelope> patch_seaway_bill_line_async(tenant_id, bill_id, line_id, opts)

Patch a seaway bill line

Partially updates a line on a seaway bill using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SeawayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a seaway bill line
  result = api_instance.patch_seaway_bill_line_async(tenant_id, bill_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->patch_seaway_bill_line_async: #{e}"
end
```

#### Using the patch_seaway_bill_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_seaway_bill_line_async_with_http_info(tenant_id, bill_id, line_id, opts)

```ruby
begin
  # Patch a seaway bill line
  data, status_code, headers = api_instance.patch_seaway_bill_line_async_with_http_info(tenant_id, bill_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->patch_seaway_bill_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_id** | **String** |  |  |
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


## release_seaway_bill_async

> <EmptyEnvelope> release_seaway_bill_async(tenant_id, bill_id, opts)

Release a seaway bill

Releases a seaway bill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SeawayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Release a seaway bill
  result = api_instance.release_seaway_bill_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->release_seaway_bill_async: #{e}"
end
```

#### Using the release_seaway_bill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> release_seaway_bill_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Release a seaway bill
  data, status_code, headers = api_instance.release_seaway_bill_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->release_seaway_bill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_seaway_bill_line_async

> <EmptyEnvelope> remove_seaway_bill_line_async(tenant_id, bill_id, line_id, opts)

Remove a seaway bill line

Removes a line from a seaway bill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SeawayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove a seaway bill line
  result = api_instance.remove_seaway_bill_line_async(tenant_id, bill_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->remove_seaway_bill_line_async: #{e}"
end
```

#### Using the remove_seaway_bill_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> remove_seaway_bill_line_async_with_http_info(tenant_id, bill_id, line_id, opts)

```ruby
begin
  # Remove a seaway bill line
  data, status_code, headers = api_instance.remove_seaway_bill_line_async_with_http_info(tenant_id, bill_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->remove_seaway_bill_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_id** | **String** |  |  |
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


## update_seaway_bill_async

> <EmptyEnvelope> update_seaway_bill_async(tenant_id, bill_id, opts)

Update a seaway bill

Updates an existing seaway bill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SeawayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  seaway_bill_update_dto: OpenapiClient::SeawayBillUpdateDto.new # SeawayBillUpdateDto | 
}

begin
  # Update a seaway bill
  result = api_instance.update_seaway_bill_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->update_seaway_bill_async: #{e}"
end
```

#### Using the update_seaway_bill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_seaway_bill_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Update a seaway bill
  data, status_code, headers = api_instance.update_seaway_bill_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->update_seaway_bill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **seaway_bill_update_dto** | [**SeawayBillUpdateDto**](SeawayBillUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_seaway_bill_line_async

> <EmptyEnvelope> update_seaway_bill_line_async(tenant_id, bill_id, line_id, opts)

Update a seaway bill line

Updates an existing line on a seaway bill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SeawayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  waybill_line_update_dto: OpenapiClient::WaybillLineUpdateDto.new # WaybillLineUpdateDto | 
}

begin
  # Update a seaway bill line
  result = api_instance.update_seaway_bill_line_async(tenant_id, bill_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->update_seaway_bill_line_async: #{e}"
end
```

#### Using the update_seaway_bill_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_seaway_bill_line_async_with_http_info(tenant_id, bill_id, line_id, opts)

```ruby
begin
  # Update a seaway bill line
  data, status_code, headers = api_instance.update_seaway_bill_line_async_with_http_info(tenant_id, bill_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SeawayBillsApi->update_seaway_bill_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_id** | **String** |  |  |
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

