# OpenapiClient::InvoiceEnumerationRangesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_invoice_enumeration_range_async**](InvoiceEnumerationRangesApi.md#create_invoice_enumeration_range_async) | **POST** /api/v2/AccountingService/InvoiceEnumerationRanges | Create a new invoice enumeration range |
| [**delete_invoice_enumeration_range_async**](InvoiceEnumerationRangesApi.md#delete_invoice_enumeration_range_async) | **DELETE** /api/v2/AccountingService/InvoiceEnumerationRanges/{rangeId} | Delete an invoice enumeration range |
| [**get_invoice_enumeration_range_details_async**](InvoiceEnumerationRangesApi.md#get_invoice_enumeration_range_details_async) | **GET** /api/v2/AccountingService/InvoiceEnumerationRanges/{rangeId} | Get invoice enumeration range by ID |
| [**get_invoice_enumeration_ranges_async**](InvoiceEnumerationRangesApi.md#get_invoice_enumeration_ranges_async) | **GET** /api/v2/AccountingService/InvoiceEnumerationRanges | Get all invoice enumeration ranges |
| [**patch_invoice_enumeration_range_async**](InvoiceEnumerationRangesApi.md#patch_invoice_enumeration_range_async) | **PATCH** /api/v2/AccountingService/InvoiceEnumerationRanges/{rangeId} | Patch an invoice enumeration range |
| [**update_invoice_enumeration_range_async**](InvoiceEnumerationRangesApi.md#update_invoice_enumeration_range_async) | **PUT** /api/v2/AccountingService/InvoiceEnumerationRanges/{rangeId} | Update an invoice enumeration range |


## create_invoice_enumeration_range_async

> <EmptyEnvelope> create_invoice_enumeration_range_async(tenant_id, opts)

Create a new invoice enumeration range

Creates a new invoice enumeration range for the tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoiceEnumerationRangesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  invoice_enumeration_range_create_dto: OpenapiClient::InvoiceEnumerationRangeCreateDto.new({valid_from: Time.now, valid_to: Time.now}) # InvoiceEnumerationRangeCreateDto | 
}

begin
  # Create a new invoice enumeration range
  result = api_instance.create_invoice_enumeration_range_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoiceEnumerationRangesApi->create_invoice_enumeration_range_async: #{e}"
end
```

#### Using the create_invoice_enumeration_range_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_invoice_enumeration_range_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new invoice enumeration range
  data, status_code, headers = api_instance.create_invoice_enumeration_range_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoiceEnumerationRangesApi->create_invoice_enumeration_range_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **invoice_enumeration_range_create_dto** | [**InvoiceEnumerationRangeCreateDto**](InvoiceEnumerationRangeCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_invoice_enumeration_range_async

> <EmptyEnvelope> delete_invoice_enumeration_range_async(tenant_id, range_id, opts)

Delete an invoice enumeration range

Deletes an invoice enumeration range by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoiceEnumerationRangesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
range_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an invoice enumeration range
  result = api_instance.delete_invoice_enumeration_range_async(tenant_id, range_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoiceEnumerationRangesApi->delete_invoice_enumeration_range_async: #{e}"
end
```

#### Using the delete_invoice_enumeration_range_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_invoice_enumeration_range_async_with_http_info(tenant_id, range_id, opts)

```ruby
begin
  # Delete an invoice enumeration range
  data, status_code, headers = api_instance.delete_invoice_enumeration_range_async_with_http_info(tenant_id, range_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoiceEnumerationRangesApi->delete_invoice_enumeration_range_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **range_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoice_enumeration_range_details_async

> <InvoiceEnumerationRangeDtoEnvelope> get_invoice_enumeration_range_details_async(tenant_id, range_id, opts)

Get invoice enumeration range by ID

Retrieves the details of a specific invoice enumeration range.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoiceEnumerationRangesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
range_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get invoice enumeration range by ID
  result = api_instance.get_invoice_enumeration_range_details_async(tenant_id, range_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoiceEnumerationRangesApi->get_invoice_enumeration_range_details_async: #{e}"
end
```

#### Using the get_invoice_enumeration_range_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InvoiceEnumerationRangeDtoEnvelope>, Integer, Hash)> get_invoice_enumeration_range_details_async_with_http_info(tenant_id, range_id, opts)

```ruby
begin
  # Get invoice enumeration range by ID
  data, status_code, headers = api_instance.get_invoice_enumeration_range_details_async_with_http_info(tenant_id, range_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InvoiceEnumerationRangeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoiceEnumerationRangesApi->get_invoice_enumeration_range_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **range_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**InvoiceEnumerationRangeDtoEnvelope**](InvoiceEnumerationRangeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoice_enumeration_ranges_async

> <InvoiceEnumerationRangeDtoListEnvelope> get_invoice_enumeration_ranges_async(tenant_id, opts)

Get all invoice enumeration ranges

Retrieves all invoice enumeration ranges for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoiceEnumerationRangesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all invoice enumeration ranges
  result = api_instance.get_invoice_enumeration_ranges_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoiceEnumerationRangesApi->get_invoice_enumeration_ranges_async: #{e}"
end
```

#### Using the get_invoice_enumeration_ranges_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InvoiceEnumerationRangeDtoListEnvelope>, Integer, Hash)> get_invoice_enumeration_ranges_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all invoice enumeration ranges
  data, status_code, headers = api_instance.get_invoice_enumeration_ranges_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InvoiceEnumerationRangeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoiceEnumerationRangesApi->get_invoice_enumeration_ranges_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**InvoiceEnumerationRangeDtoListEnvelope**](InvoiceEnumerationRangeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_invoice_enumeration_range_async

> <EmptyEnvelope> patch_invoice_enumeration_range_async(tenant_id, range_id, opts)

Patch an invoice enumeration range

Partially updates an invoice enumeration range.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoiceEnumerationRangesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
range_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch an invoice enumeration range
  result = api_instance.patch_invoice_enumeration_range_async(tenant_id, range_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoiceEnumerationRangesApi->patch_invoice_enumeration_range_async: #{e}"
end
```

#### Using the patch_invoice_enumeration_range_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_invoice_enumeration_range_async_with_http_info(tenant_id, range_id, opts)

```ruby
begin
  # Patch an invoice enumeration range
  data, status_code, headers = api_instance.patch_invoice_enumeration_range_async_with_http_info(tenant_id, range_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoiceEnumerationRangesApi->patch_invoice_enumeration_range_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **range_id** | **String** |  |  |
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


## update_invoice_enumeration_range_async

> <EmptyEnvelope> update_invoice_enumeration_range_async(tenant_id, range_id, opts)

Update an invoice enumeration range

Updates an existing invoice enumeration range with the provided data.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoiceEnumerationRangesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
range_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  invoice_enumeration_range_update_dto: OpenapiClient::InvoiceEnumerationRangeUpdateDto.new # InvoiceEnumerationRangeUpdateDto | 
}

begin
  # Update an invoice enumeration range
  result = api_instance.update_invoice_enumeration_range_async(tenant_id, range_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoiceEnumerationRangesApi->update_invoice_enumeration_range_async: #{e}"
end
```

#### Using the update_invoice_enumeration_range_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_invoice_enumeration_range_async_with_http_info(tenant_id, range_id, opts)

```ruby
begin
  # Update an invoice enumeration range
  data, status_code, headers = api_instance.update_invoice_enumeration_range_async_with_http_info(tenant_id, range_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoiceEnumerationRangesApi->update_invoice_enumeration_range_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **range_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **invoice_enumeration_range_update_dto** | [**InvoiceEnumerationRangeUpdateDto**](InvoiceEnumerationRangeUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

