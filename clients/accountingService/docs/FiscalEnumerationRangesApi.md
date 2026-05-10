# OpenapiClient::FiscalEnumerationRangesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_invoice_enumeration_range**](FiscalEnumerationRangesApi.md#create_invoice_enumeration_range) | **POST** /api/v2/AccountingService/Fiscals/Authorities/EnumerationRanges | Create an invoice enumeration range |
| [**delete_invoice_enumeration_range**](FiscalEnumerationRangesApi.md#delete_invoice_enumeration_range) | **DELETE** /api/v2/AccountingService/Fiscals/Authorities/EnumerationRanges/{enumerationRangeId} | Delete an invoice enumeration range |
| [**get_invoice_enumeration_range**](FiscalEnumerationRangesApi.md#get_invoice_enumeration_range) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/EnumerationRanges/{enumerationRangeId} | Get invoice enumeration range by ID |
| [**get_invoice_enumeration_ranges**](FiscalEnumerationRangesApi.md#get_invoice_enumeration_ranges) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{authorityId}/EnumerationRanges | Get invoice enumeration ranges for an authority |
| [**get_invoice_enumeration_ranges_count**](FiscalEnumerationRangesApi.md#get_invoice_enumeration_ranges_count) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/EnumerationRanges/Count | Get invoice enumeration ranges count |
| [**update_invoice_enumeration_range**](FiscalEnumerationRangesApi.md#update_invoice_enumeration_range) | **PUT** /api/v2/AccountingService/Fiscals/Authorities/EnumerationRanges/{enumerationRangeId} | Update an invoice enumeration range |


## create_invoice_enumeration_range

> <EmptyEnvelope> create_invoice_enumeration_range(tenant_id, opts)

Create an invoice enumeration range

Creates a new invoice enumeration range for a fiscal authority.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalEnumerationRangesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  invoice_enumeration_range_create_dto: OpenapiClient::InvoiceEnumerationRangeCreateDto.new({valid_from: Time.now, valid_to: Time.now}) # InvoiceEnumerationRangeCreateDto | 
}

begin
  # Create an invoice enumeration range
  result = api_instance.create_invoice_enumeration_range(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalEnumerationRangesApi->create_invoice_enumeration_range: #{e}"
end
```

#### Using the create_invoice_enumeration_range_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_invoice_enumeration_range_with_http_info(tenant_id, opts)

```ruby
begin
  # Create an invoice enumeration range
  data, status_code, headers = api_instance.create_invoice_enumeration_range_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalEnumerationRangesApi->create_invoice_enumeration_range_with_http_info: #{e}"
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


## delete_invoice_enumeration_range

> <EmptyEnvelope> delete_invoice_enumeration_range(tenant_id, enumeration_range_id, opts)

Delete an invoice enumeration range

Deletes an invoice enumeration range identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalEnumerationRangesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
enumeration_range_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an invoice enumeration range
  result = api_instance.delete_invoice_enumeration_range(tenant_id, enumeration_range_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalEnumerationRangesApi->delete_invoice_enumeration_range: #{e}"
end
```

#### Using the delete_invoice_enumeration_range_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_invoice_enumeration_range_with_http_info(tenant_id, enumeration_range_id, opts)

```ruby
begin
  # Delete an invoice enumeration range
  data, status_code, headers = api_instance.delete_invoice_enumeration_range_with_http_info(tenant_id, enumeration_range_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalEnumerationRangesApi->delete_invoice_enumeration_range_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **enumeration_range_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoice_enumeration_range

> <InvoiceEnumerationRangeDtoEnvelope> get_invoice_enumeration_range(tenant_id, fiscal_authority_id, enumeration_range_id, opts)

Get invoice enumeration range by ID

Retrieves a specific invoice enumeration range by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalEnumerationRangesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
enumeration_range_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get invoice enumeration range by ID
  result = api_instance.get_invoice_enumeration_range(tenant_id, fiscal_authority_id, enumeration_range_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalEnumerationRangesApi->get_invoice_enumeration_range: #{e}"
end
```

#### Using the get_invoice_enumeration_range_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InvoiceEnumerationRangeDtoEnvelope>, Integer, Hash)> get_invoice_enumeration_range_with_http_info(tenant_id, fiscal_authority_id, enumeration_range_id, opts)

```ruby
begin
  # Get invoice enumeration range by ID
  data, status_code, headers = api_instance.get_invoice_enumeration_range_with_http_info(tenant_id, fiscal_authority_id, enumeration_range_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InvoiceEnumerationRangeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalEnumerationRangesApi->get_invoice_enumeration_range_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_authority_id** | **String** |  |  |
| **enumeration_range_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**InvoiceEnumerationRangeDtoEnvelope**](InvoiceEnumerationRangeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoice_enumeration_ranges

> <InvoiceEnumerationRangeDtoListEnvelope> get_invoice_enumeration_ranges(fiscal_authority_id, authority_id, opts)

Get invoice enumeration ranges for an authority

Retrieves all invoice enumeration ranges for the specified fiscal authority.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalEnumerationRangesApi.new
fiscal_authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
authority_id = 'authority_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get invoice enumeration ranges for an authority
  result = api_instance.get_invoice_enumeration_ranges(fiscal_authority_id, authority_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalEnumerationRangesApi->get_invoice_enumeration_ranges: #{e}"
end
```

#### Using the get_invoice_enumeration_ranges_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InvoiceEnumerationRangeDtoListEnvelope>, Integer, Hash)> get_invoice_enumeration_ranges_with_http_info(fiscal_authority_id, authority_id, opts)

```ruby
begin
  # Get invoice enumeration ranges for an authority
  data, status_code, headers = api_instance.get_invoice_enumeration_ranges_with_http_info(fiscal_authority_id, authority_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InvoiceEnumerationRangeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalEnumerationRangesApi->get_invoice_enumeration_ranges_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **fiscal_authority_id** | **String** |  |  |
| **authority_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**InvoiceEnumerationRangeDtoListEnvelope**](InvoiceEnumerationRangeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoice_enumeration_ranges_count

> <Int32Envelope> get_invoice_enumeration_ranges_count(fiscal_authority_id, opts)

Get invoice enumeration ranges count

Returns the total count of invoice enumeration ranges for the specified fiscal authority.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalEnumerationRangesApi.new
fiscal_authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get invoice enumeration ranges count
  result = api_instance.get_invoice_enumeration_ranges_count(fiscal_authority_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalEnumerationRangesApi->get_invoice_enumeration_ranges_count: #{e}"
end
```

#### Using the get_invoice_enumeration_ranges_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_invoice_enumeration_ranges_count_with_http_info(fiscal_authority_id, opts)

```ruby
begin
  # Get invoice enumeration ranges count
  data, status_code, headers = api_instance.get_invoice_enumeration_ranges_count_with_http_info(fiscal_authority_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalEnumerationRangesApi->get_invoice_enumeration_ranges_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **fiscal_authority_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_invoice_enumeration_range

> <EmptyEnvelope> update_invoice_enumeration_range(tenant_id, enumeration_range_id, opts)

Update an invoice enumeration range

Updates an existing invoice enumeration range identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalEnumerationRangesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
enumeration_range_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  invoice_enumeration_range_update_dto: OpenapiClient::InvoiceEnumerationRangeUpdateDto.new # InvoiceEnumerationRangeUpdateDto | 
}

begin
  # Update an invoice enumeration range
  result = api_instance.update_invoice_enumeration_range(tenant_id, enumeration_range_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalEnumerationRangesApi->update_invoice_enumeration_range: #{e}"
end
```

#### Using the update_invoice_enumeration_range_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_invoice_enumeration_range_with_http_info(tenant_id, enumeration_range_id, opts)

```ruby
begin
  # Update an invoice enumeration range
  data, status_code, headers = api_instance.update_invoice_enumeration_range_with_http_info(tenant_id, enumeration_range_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalEnumerationRangesApi->update_invoice_enumeration_range_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **enumeration_range_id** | **String** |  |  |
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

