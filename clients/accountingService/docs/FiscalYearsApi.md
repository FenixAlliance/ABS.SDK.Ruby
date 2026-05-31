# OpenapiClient::FiscalYearsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_fiscal_year_async**](FiscalYearsApi.md#create_fiscal_year_async) | **POST** /api/v2/AccountingService/FiscalYears | Create fiscal year |
| [**delete_fiscal_year_async**](FiscalYearsApi.md#delete_fiscal_year_async) | **DELETE** /api/v2/AccountingService/FiscalYears/{fiscalYearId} | Delete fiscal year |
| [**get_fiscal_year_details_async**](FiscalYearsApi.md#get_fiscal_year_details_async) | **GET** /api/v2/AccountingService/FiscalYears/{fiscalYearId} | Get fiscal year by ID |
| [**get_fiscal_years_async**](FiscalYearsApi.md#get_fiscal_years_async) | **GET** /api/v2/AccountingService/FiscalYears | Get all fiscal years |
| [**get_fiscal_years_count_async**](FiscalYearsApi.md#get_fiscal_years_count_async) | **GET** /api/v2/AccountingService/FiscalYears/Count | Count fiscal years |
| [**update_fiscal_year_async**](FiscalYearsApi.md#update_fiscal_year_async) | **PUT** /api/v2/AccountingService/FiscalYears/{fiscalYearId} | Update fiscal year |


## create_fiscal_year_async

> <EmptyEnvelope> create_fiscal_year_async(tenant_id, opts)

Create fiscal year

Creates a new fiscal year entry for a tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalYearsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  fiscal_year_create_dto: OpenapiClient::FiscalYearCreateDto.new # FiscalYearCreateDto | 
}

begin
  # Create fiscal year
  result = api_instance.create_fiscal_year_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalYearsApi->create_fiscal_year_async: #{e}"
end
```

#### Using the create_fiscal_year_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_fiscal_year_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create fiscal year
  data, status_code, headers = api_instance.create_fiscal_year_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalYearsApi->create_fiscal_year_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **fiscal_year_create_dto** | [**FiscalYearCreateDto**](FiscalYearCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_fiscal_year_async

> <EmptyEnvelope> delete_fiscal_year_async(tenant_id, fiscal_year_id, opts)

Delete fiscal year

Deletes a fiscal year identified by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalYearsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_year_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete fiscal year
  result = api_instance.delete_fiscal_year_async(tenant_id, fiscal_year_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalYearsApi->delete_fiscal_year_async: #{e}"
end
```

#### Using the delete_fiscal_year_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_fiscal_year_async_with_http_info(tenant_id, fiscal_year_id, opts)

```ruby
begin
  # Delete fiscal year
  data, status_code, headers = api_instance.delete_fiscal_year_async_with_http_info(tenant_id, fiscal_year_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalYearsApi->delete_fiscal_year_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_year_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_year_details_async

> <FiscalYearDtoEnvelope> get_fiscal_year_details_async(tenant_id, fiscal_year_id, opts)

Get fiscal year by ID

Gets details for a specific fiscal year.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalYearsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_year_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal year by ID
  result = api_instance.get_fiscal_year_details_async(tenant_id, fiscal_year_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalYearsApi->get_fiscal_year_details_async: #{e}"
end
```

#### Using the get_fiscal_year_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FiscalYearDtoEnvelope>, Integer, Hash)> get_fiscal_year_details_async_with_http_info(tenant_id, fiscal_year_id, opts)

```ruby
begin
  # Get fiscal year by ID
  data, status_code, headers = api_instance.get_fiscal_year_details_async_with_http_info(tenant_id, fiscal_year_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FiscalYearDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalYearsApi->get_fiscal_year_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_year_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**FiscalYearDtoEnvelope**](FiscalYearDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_years_async

> <FiscalYearDtoIReadOnlyListEnvelope> get_fiscal_years_async(tenant_id, opts)

Get all fiscal years

Retrieves a list of fiscal years for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalYearsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all fiscal years
  result = api_instance.get_fiscal_years_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalYearsApi->get_fiscal_years_async: #{e}"
end
```

#### Using the get_fiscal_years_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FiscalYearDtoIReadOnlyListEnvelope>, Integer, Hash)> get_fiscal_years_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all fiscal years
  data, status_code, headers = api_instance.get_fiscal_years_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FiscalYearDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalYearsApi->get_fiscal_years_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**FiscalYearDtoIReadOnlyListEnvelope**](FiscalYearDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_years_count_async

> <Int32Envelope> get_fiscal_years_count_async(tenant_id, opts)

Count fiscal years

Returns the number of fiscal years for a tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalYearsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count fiscal years
  result = api_instance.get_fiscal_years_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalYearsApi->get_fiscal_years_count_async: #{e}"
end
```

#### Using the get_fiscal_years_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_fiscal_years_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count fiscal years
  data, status_code, headers = api_instance.get_fiscal_years_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalYearsApi->get_fiscal_years_count_async_with_http_info: #{e}"
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


## update_fiscal_year_async

> <EmptyEnvelope> update_fiscal_year_async(tenant_id, fiscal_year_id, opts)

Update fiscal year

Updates an existing fiscal year identified by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalYearsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_year_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  fiscal_year_update_dto: OpenapiClient::FiscalYearUpdateDto.new # FiscalYearUpdateDto | 
}

begin
  # Update fiscal year
  result = api_instance.update_fiscal_year_async(tenant_id, fiscal_year_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalYearsApi->update_fiscal_year_async: #{e}"
end
```

#### Using the update_fiscal_year_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_fiscal_year_async_with_http_info(tenant_id, fiscal_year_id, opts)

```ruby
begin
  # Update fiscal year
  data, status_code, headers = api_instance.update_fiscal_year_async_with_http_info(tenant_id, fiscal_year_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalYearsApi->update_fiscal_year_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_year_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **fiscal_year_update_dto** | [**FiscalYearUpdateDto**](FiscalYearUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

