# OpenapiClient::AirwayBillsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**add_airway_bill_line_async**](AirwayBillsApi.md#add_airway_bill_line_async) | **POST** /api/v2/LogisticsService/AirwayBills/{billId}/Lines | Add a line to airway bill |
| [**cancel_airway_bill_async**](AirwayBillsApi.md#cancel_airway_bill_async) | **POST** /api/v2/LogisticsService/AirwayBills/{billId}/Cancel | Cancel an airway bill |
| [**create_airway_bill_async**](AirwayBillsApi.md#create_airway_bill_async) | **POST** /api/v2/LogisticsService/AirwayBills | Create an airway bill |
| [**delete_airway_bill_async**](AirwayBillsApi.md#delete_airway_bill_async) | **DELETE** /api/v2/LogisticsService/AirwayBills/{billId} | Delete an airway bill |
| [**get_airway_bill_by_id_async**](AirwayBillsApi.md#get_airway_bill_by_id_async) | **GET** /api/v2/LogisticsService/AirwayBills/{billId} | Get airway bill by ID |
| [**get_airway_bill_lines_async**](AirwayBillsApi.md#get_airway_bill_lines_async) | **GET** /api/v2/LogisticsService/AirwayBills/{billId}/Lines | Get airway bill lines |
| [**get_airway_bill_lines_count_async**](AirwayBillsApi.md#get_airway_bill_lines_count_async) | **GET** /api/v2/LogisticsService/AirwayBills/{billId}/Lines/Count | Get airway bill lines count |
| [**get_airway_bills_async**](AirwayBillsApi.md#get_airway_bills_async) | **GET** /api/v2/LogisticsService/AirwayBills | Get all airway bills |
| [**get_airway_bills_count_async**](AirwayBillsApi.md#get_airway_bills_count_async) | **GET** /api/v2/LogisticsService/AirwayBills/Count | Get airway bills count |
| [**issue_airway_bill_async**](AirwayBillsApi.md#issue_airway_bill_async) | **POST** /api/v2/LogisticsService/AirwayBills/{billId}/Issue | Issue an airway bill |
| [**mark_airway_bill_arrived_async**](AirwayBillsApi.md#mark_airway_bill_arrived_async) | **POST** /api/v2/LogisticsService/AirwayBills/{billId}/MarkArrived | Mark airway bill arrived |
| [**mark_airway_bill_delivered_async**](AirwayBillsApi.md#mark_airway_bill_delivered_async) | **POST** /api/v2/LogisticsService/AirwayBills/{billId}/MarkDelivered | Mark airway bill delivered |
| [**mark_airway_bill_in_transit_async**](AirwayBillsApi.md#mark_airway_bill_in_transit_async) | **POST** /api/v2/LogisticsService/AirwayBills/{billId}/MarkInTransit | Mark airway bill in transit |
| [**remove_airway_bill_line_async**](AirwayBillsApi.md#remove_airway_bill_line_async) | **DELETE** /api/v2/LogisticsService/AirwayBills/{billId}/Lines/{lineId} | Remove an airway bill line |
| [**update_airway_bill_async**](AirwayBillsApi.md#update_airway_bill_async) | **PUT** /api/v2/LogisticsService/AirwayBills/{billId} | Update an airway bill |
| [**update_airway_bill_line_async**](AirwayBillsApi.md#update_airway_bill_line_async) | **PUT** /api/v2/LogisticsService/AirwayBills/{billId}/Lines/{lineId} | Update an airway bill line |


## add_airway_bill_line_async

> <EmptyEnvelope> add_airway_bill_line_async(tenant_id, bill_id, opts)

Add a line to airway bill

Adds a new line to an airway bill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AirwayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  waybill_line_create_dto: OpenapiClient::WaybillLineCreateDto.new # WaybillLineCreateDto | 
}

begin
  # Add a line to airway bill
  result = api_instance.add_airway_bill_line_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->add_airway_bill_line_async: #{e}"
end
```

#### Using the add_airway_bill_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> add_airway_bill_line_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Add a line to airway bill
  data, status_code, headers = api_instance.add_airway_bill_line_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->add_airway_bill_line_async_with_http_info: #{e}"
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


## cancel_airway_bill_async

> <EmptyEnvelope> cancel_airway_bill_async(tenant_id, bill_id, opts)

Cancel an airway bill

Cancels an airway bill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AirwayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Cancel an airway bill
  result = api_instance.cancel_airway_bill_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->cancel_airway_bill_async: #{e}"
end
```

#### Using the cancel_airway_bill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> cancel_airway_bill_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Cancel an airway bill
  data, status_code, headers = api_instance.cancel_airway_bill_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->cancel_airway_bill_async_with_http_info: #{e}"
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


## create_airway_bill_async

> <EmptyEnvelope> create_airway_bill_async(tenant_id, opts)

Create an airway bill

Creates a new airway bill for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AirwayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  airway_bill_create_dto: OpenapiClient::AirwayBillCreateDto.new # AirwayBillCreateDto | 
}

begin
  # Create an airway bill
  result = api_instance.create_airway_bill_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->create_airway_bill_async: #{e}"
end
```

#### Using the create_airway_bill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_airway_bill_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create an airway bill
  data, status_code, headers = api_instance.create_airway_bill_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->create_airway_bill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **airway_bill_create_dto** | [**AirwayBillCreateDto**](AirwayBillCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_airway_bill_async

> <EmptyEnvelope> delete_airway_bill_async(tenant_id, bill_id, opts)

Delete an airway bill

Deletes an airway bill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AirwayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an airway bill
  result = api_instance.delete_airway_bill_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->delete_airway_bill_async: #{e}"
end
```

#### Using the delete_airway_bill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_airway_bill_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Delete an airway bill
  data, status_code, headers = api_instance.delete_airway_bill_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->delete_airway_bill_async_with_http_info: #{e}"
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


## get_airway_bill_by_id_async

> <AirwayBillDtoEnvelope> get_airway_bill_by_id_async(tenant_id, bill_id, opts)

Get airway bill by ID

Retrieves a specific airway bill by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AirwayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get airway bill by ID
  result = api_instance.get_airway_bill_by_id_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->get_airway_bill_by_id_async: #{e}"
end
```

#### Using the get_airway_bill_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AirwayBillDtoEnvelope>, Integer, Hash)> get_airway_bill_by_id_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Get airway bill by ID
  data, status_code, headers = api_instance.get_airway_bill_by_id_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AirwayBillDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->get_airway_bill_by_id_async_with_http_info: #{e}"
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

[**AirwayBillDtoEnvelope**](AirwayBillDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_airway_bill_lines_async

> <WaybillLineDtoListEnvelope> get_airway_bill_lines_async(tenant_id, bill_id, opts)

Get airway bill lines

Retrieves all lines for a specific airway bill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AirwayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get airway bill lines
  result = api_instance.get_airway_bill_lines_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->get_airway_bill_lines_async: #{e}"
end
```

#### Using the get_airway_bill_lines_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WaybillLineDtoListEnvelope>, Integer, Hash)> get_airway_bill_lines_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Get airway bill lines
  data, status_code, headers = api_instance.get_airway_bill_lines_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WaybillLineDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->get_airway_bill_lines_async_with_http_info: #{e}"
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


## get_airway_bill_lines_count_async

> <Int32Envelope> get_airway_bill_lines_count_async(tenant_id, bill_id, opts)

Get airway bill lines count

Returns the count of lines for a specific airway bill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AirwayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get airway bill lines count
  result = api_instance.get_airway_bill_lines_count_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->get_airway_bill_lines_count_async: #{e}"
end
```

#### Using the get_airway_bill_lines_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_airway_bill_lines_count_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Get airway bill lines count
  data, status_code, headers = api_instance.get_airway_bill_lines_count_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->get_airway_bill_lines_count_async_with_http_info: #{e}"
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


## get_airway_bills_async

> <AirwayBillDtoListEnvelope> get_airway_bills_async(tenant_id, opts)

Get all airway bills

Retrieves all airway bills for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AirwayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all airway bills
  result = api_instance.get_airway_bills_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->get_airway_bills_async: #{e}"
end
```

#### Using the get_airway_bills_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AirwayBillDtoListEnvelope>, Integer, Hash)> get_airway_bills_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all airway bills
  data, status_code, headers = api_instance.get_airway_bills_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AirwayBillDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->get_airway_bills_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**AirwayBillDtoListEnvelope**](AirwayBillDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_airway_bills_count_async

> <Int32Envelope> get_airway_bills_count_async(tenant_id, opts)

Get airway bills count

Returns the count of airway bills for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AirwayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get airway bills count
  result = api_instance.get_airway_bills_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->get_airway_bills_count_async: #{e}"
end
```

#### Using the get_airway_bills_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_airway_bills_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get airway bills count
  data, status_code, headers = api_instance.get_airway_bills_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->get_airway_bills_count_async_with_http_info: #{e}"
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


## issue_airway_bill_async

> <EmptyEnvelope> issue_airway_bill_async(tenant_id, bill_id, opts)

Issue an airway bill

Issues an airway bill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AirwayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Issue an airway bill
  result = api_instance.issue_airway_bill_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->issue_airway_bill_async: #{e}"
end
```

#### Using the issue_airway_bill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> issue_airway_bill_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Issue an airway bill
  data, status_code, headers = api_instance.issue_airway_bill_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->issue_airway_bill_async_with_http_info: #{e}"
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


## mark_airway_bill_arrived_async

> <EmptyEnvelope> mark_airway_bill_arrived_async(tenant_id, bill_id, opts)

Mark airway bill arrived

Marks an airway bill as arrived.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AirwayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Mark airway bill arrived
  result = api_instance.mark_airway_bill_arrived_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->mark_airway_bill_arrived_async: #{e}"
end
```

#### Using the mark_airway_bill_arrived_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> mark_airway_bill_arrived_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Mark airway bill arrived
  data, status_code, headers = api_instance.mark_airway_bill_arrived_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->mark_airway_bill_arrived_async_with_http_info: #{e}"
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


## mark_airway_bill_delivered_async

> <EmptyEnvelope> mark_airway_bill_delivered_async(tenant_id, bill_id, opts)

Mark airway bill delivered

Marks an airway bill as delivered.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AirwayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Mark airway bill delivered
  result = api_instance.mark_airway_bill_delivered_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->mark_airway_bill_delivered_async: #{e}"
end
```

#### Using the mark_airway_bill_delivered_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> mark_airway_bill_delivered_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Mark airway bill delivered
  data, status_code, headers = api_instance.mark_airway_bill_delivered_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->mark_airway_bill_delivered_async_with_http_info: #{e}"
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


## mark_airway_bill_in_transit_async

> <EmptyEnvelope> mark_airway_bill_in_transit_async(tenant_id, bill_id, opts)

Mark airway bill in transit

Marks an airway bill as in transit.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AirwayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Mark airway bill in transit
  result = api_instance.mark_airway_bill_in_transit_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->mark_airway_bill_in_transit_async: #{e}"
end
```

#### Using the mark_airway_bill_in_transit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> mark_airway_bill_in_transit_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Mark airway bill in transit
  data, status_code, headers = api_instance.mark_airway_bill_in_transit_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->mark_airway_bill_in_transit_async_with_http_info: #{e}"
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


## remove_airway_bill_line_async

> <EmptyEnvelope> remove_airway_bill_line_async(tenant_id, bill_id, line_id, opts)

Remove an airway bill line

Removes a line from an airway bill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AirwayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove an airway bill line
  result = api_instance.remove_airway_bill_line_async(tenant_id, bill_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->remove_airway_bill_line_async: #{e}"
end
```

#### Using the remove_airway_bill_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> remove_airway_bill_line_async_with_http_info(tenant_id, bill_id, line_id, opts)

```ruby
begin
  # Remove an airway bill line
  data, status_code, headers = api_instance.remove_airway_bill_line_async_with_http_info(tenant_id, bill_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->remove_airway_bill_line_async_with_http_info: #{e}"
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


## update_airway_bill_async

> <EmptyEnvelope> update_airway_bill_async(tenant_id, bill_id, opts)

Update an airway bill

Updates an existing airway bill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AirwayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  airway_bill_update_dto: OpenapiClient::AirwayBillUpdateDto.new # AirwayBillUpdateDto | 
}

begin
  # Update an airway bill
  result = api_instance.update_airway_bill_async(tenant_id, bill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->update_airway_bill_async: #{e}"
end
```

#### Using the update_airway_bill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_airway_bill_async_with_http_info(tenant_id, bill_id, opts)

```ruby
begin
  # Update an airway bill
  data, status_code, headers = api_instance.update_airway_bill_async_with_http_info(tenant_id, bill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->update_airway_bill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **airway_bill_update_dto** | [**AirwayBillUpdateDto**](AirwayBillUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_airway_bill_line_async

> <EmptyEnvelope> update_airway_bill_line_async(tenant_id, bill_id, line_id, opts)

Update an airway bill line

Updates an existing line on an airway bill.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AirwayBillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  waybill_line_update_dto: OpenapiClient::WaybillLineUpdateDto.new # WaybillLineUpdateDto | 
}

begin
  # Update an airway bill line
  result = api_instance.update_airway_bill_line_async(tenant_id, bill_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->update_airway_bill_line_async: #{e}"
end
```

#### Using the update_airway_bill_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_airway_bill_line_async_with_http_info(tenant_id, bill_id, line_id, opts)

```ruby
begin
  # Update an airway bill line
  data, status_code, headers = api_instance.update_airway_bill_line_async_with_http_info(tenant_id, bill_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AirwayBillsApi->update_airway_bill_line_async_with_http_info: #{e}"
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

