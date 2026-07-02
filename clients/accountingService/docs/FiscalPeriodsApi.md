# OpenapiClient::FiscalPeriodsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_fiscal_period**](FiscalPeriodsApi.md#create_fiscal_period) | **POST** /api/v2/AccountingService/Fiscals/Authorities/FiscalPeriods | Create a fiscal period |
| [**delete_fiscal_period**](FiscalPeriodsApi.md#delete_fiscal_period) | **DELETE** /api/v2/AccountingService/Fiscals/Authorities/FiscalPeriods/{fiscalPeriodId} | Delete a fiscal period |
| [**get_fiscal_period**](FiscalPeriodsApi.md#get_fiscal_period) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalYears/{fiscalYearId}/FiscalPeriods/{fiscalPeriodId} | Get fiscal period by ID |
| [**get_fiscal_periods**](FiscalPeriodsApi.md#get_fiscal_periods) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{authorityId}/FiscalYears/{fiscalYearId}/FiscalPeriods | Get fiscal periods for a fiscal year |
| [**get_fiscal_periods_count**](FiscalPeriodsApi.md#get_fiscal_periods_count) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalYears/{fiscalYearId}/FiscalPeriods/Count | Get fiscal periods count |
| [**patch_fiscal_period_async**](FiscalPeriodsApi.md#patch_fiscal_period_async) | **PATCH** /api/v2/AccountingService/Fiscals/Authorities/FiscalPeriods/{fiscalPeriodId} | Patch a fiscal period |
| [**update_fiscal_period**](FiscalPeriodsApi.md#update_fiscal_period) | **PUT** /api/v2/AccountingService/Fiscals/Authorities/FiscalPeriods/{fiscalPeriodId} | Update a fiscal period |


## create_fiscal_period

> <EmptyEnvelope> create_fiscal_period(tenant_id, opts)

Create a fiscal period

Creates a new fiscal period associated with a fiscal year.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  fiscal_period_create_dto: OpenapiClient::FiscalPeriodCreateDto.new # FiscalPeriodCreateDto | 
}

begin
  # Create a fiscal period
  result = api_instance.create_fiscal_period(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalPeriodsApi->create_fiscal_period: #{e}"
end
```

#### Using the create_fiscal_period_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_fiscal_period_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a fiscal period
  data, status_code, headers = api_instance.create_fiscal_period_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalPeriodsApi->create_fiscal_period_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **fiscal_period_create_dto** | [**FiscalPeriodCreateDto**](FiscalPeriodCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_fiscal_period

> <EmptyEnvelope> delete_fiscal_period(tenant_id, fiscal_period_id, opts)

Delete a fiscal period

Deletes a fiscal period identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_period_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a fiscal period
  result = api_instance.delete_fiscal_period(tenant_id, fiscal_period_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalPeriodsApi->delete_fiscal_period: #{e}"
end
```

#### Using the delete_fiscal_period_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_fiscal_period_with_http_info(tenant_id, fiscal_period_id, opts)

```ruby
begin
  # Delete a fiscal period
  data, status_code, headers = api_instance.delete_fiscal_period_with_http_info(tenant_id, fiscal_period_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalPeriodsApi->delete_fiscal_period_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_period_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_period

> <FiscalPeriodDtoEnvelope> get_fiscal_period(tenant_id, fiscal_authority_id, fiscal_year_id, fiscal_period_id, opts)

Get fiscal period by ID

Retrieves a specific fiscal period by its unique identifier within a fiscal year.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_year_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_period_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal period by ID
  result = api_instance.get_fiscal_period(tenant_id, fiscal_authority_id, fiscal_year_id, fiscal_period_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalPeriodsApi->get_fiscal_period: #{e}"
end
```

#### Using the get_fiscal_period_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FiscalPeriodDtoEnvelope>, Integer, Hash)> get_fiscal_period_with_http_info(tenant_id, fiscal_authority_id, fiscal_year_id, fiscal_period_id, opts)

```ruby
begin
  # Get fiscal period by ID
  data, status_code, headers = api_instance.get_fiscal_period_with_http_info(tenant_id, fiscal_authority_id, fiscal_year_id, fiscal_period_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FiscalPeriodDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalPeriodsApi->get_fiscal_period_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_authority_id** | **String** |  |  |
| **fiscal_year_id** | **String** |  |  |
| **fiscal_period_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**FiscalPeriodDtoEnvelope**](FiscalPeriodDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_periods

> <FiscalPeriodDtoListEnvelope> get_fiscal_periods(tenant_id, fiscal_authority_id, fiscal_year_id, authority_id, opts)

Get fiscal periods for a fiscal year

Retrieves all fiscal periods for the specified fiscal year within a fiscal authority.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_year_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
authority_id = 'authority_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal periods for a fiscal year
  result = api_instance.get_fiscal_periods(tenant_id, fiscal_authority_id, fiscal_year_id, authority_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalPeriodsApi->get_fiscal_periods: #{e}"
end
```

#### Using the get_fiscal_periods_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FiscalPeriodDtoListEnvelope>, Integer, Hash)> get_fiscal_periods_with_http_info(tenant_id, fiscal_authority_id, fiscal_year_id, authority_id, opts)

```ruby
begin
  # Get fiscal periods for a fiscal year
  data, status_code, headers = api_instance.get_fiscal_periods_with_http_info(tenant_id, fiscal_authority_id, fiscal_year_id, authority_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FiscalPeriodDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalPeriodsApi->get_fiscal_periods_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_authority_id** | **String** |  |  |
| **fiscal_year_id** | **String** |  |  |
| **authority_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**FiscalPeriodDtoListEnvelope**](FiscalPeriodDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_periods_count

> <Int32Envelope> get_fiscal_periods_count(tenant_id, fiscal_authority_id, fiscal_year_id, opts)

Get fiscal periods count

Returns the total count of fiscal periods for the specified fiscal year.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_year_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal periods count
  result = api_instance.get_fiscal_periods_count(tenant_id, fiscal_authority_id, fiscal_year_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalPeriodsApi->get_fiscal_periods_count: #{e}"
end
```

#### Using the get_fiscal_periods_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_fiscal_periods_count_with_http_info(tenant_id, fiscal_authority_id, fiscal_year_id, opts)

```ruby
begin
  # Get fiscal periods count
  data, status_code, headers = api_instance.get_fiscal_periods_count_with_http_info(tenant_id, fiscal_authority_id, fiscal_year_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalPeriodsApi->get_fiscal_periods_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_authority_id** | **String** |  |  |
| **fiscal_year_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_fiscal_period_async

> <EmptyEnvelope> patch_fiscal_period_async(tenant_id, fiscal_period_id, opts)

Patch a fiscal period

Partially updates a fiscal period.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_period_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a fiscal period
  result = api_instance.patch_fiscal_period_async(tenant_id, fiscal_period_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalPeriodsApi->patch_fiscal_period_async: #{e}"
end
```

#### Using the patch_fiscal_period_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_fiscal_period_async_with_http_info(tenant_id, fiscal_period_id, opts)

```ruby
begin
  # Patch a fiscal period
  data, status_code, headers = api_instance.patch_fiscal_period_async_with_http_info(tenant_id, fiscal_period_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalPeriodsApi->patch_fiscal_period_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_period_id** | **String** |  |  |
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


## update_fiscal_period

> <EmptyEnvelope> update_fiscal_period(tenant_id, fiscal_period_id, opts)

Update a fiscal period

Updates an existing fiscal period identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_period_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  fiscal_period_update_dto: OpenapiClient::FiscalPeriodUpdateDto.new # FiscalPeriodUpdateDto | 
}

begin
  # Update a fiscal period
  result = api_instance.update_fiscal_period(tenant_id, fiscal_period_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalPeriodsApi->update_fiscal_period: #{e}"
end
```

#### Using the update_fiscal_period_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_fiscal_period_with_http_info(tenant_id, fiscal_period_id, opts)

```ruby
begin
  # Update a fiscal period
  data, status_code, headers = api_instance.update_fiscal_period_with_http_info(tenant_id, fiscal_period_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalPeriodsApi->update_fiscal_period_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_period_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **fiscal_period_update_dto** | [**FiscalPeriodUpdateDto**](FiscalPeriodUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

