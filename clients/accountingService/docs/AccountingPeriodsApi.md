# OpenapiClient::AccountingPeriodsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_accounting_period**](AccountingPeriodsApi.md#create_accounting_period) | **POST** /api/v2/AccountingService/AccountingPeriods | Creates a new accounting period |
| [**delete_accounting_period**](AccountingPeriodsApi.md#delete_accounting_period) | **DELETE** /api/v2/AccountingService/AccountingPeriods/{accountingPeriodId} | Deletes an existing accounting period |
| [**get_accounting_period**](AccountingPeriodsApi.md#get_accounting_period) | **GET** /api/v2/AccountingService/AccountingPeriods/{accountingPeriodId} | Gets the current tenant accounting period |
| [**get_accounting_periods**](AccountingPeriodsApi.md#get_accounting_periods) | **GET** /api/v2/AccountingService/AccountingPeriods | Get all accounting periods for a tenant |
| [**get_accounting_periods_count_async**](AccountingPeriodsApi.md#get_accounting_periods_count_async) | **GET** /api/v2/AccountingService/AccountingPeriods/Count | Gets the current tenant accounting periods count |
| [**patch_accounting_period_async**](AccountingPeriodsApi.md#patch_accounting_period_async) | **PATCH** /api/v2/AccountingService/AccountingPeriods/{accountingPeriodId} | Patch an accounting period |
| [**update_accounting_period**](AccountingPeriodsApi.md#update_accounting_period) | **PUT** /api/v2/AccountingService/AccountingPeriods/{accountingPeriodId} | Updates an existing accounting period |


## create_accounting_period

> <EmptyEnvelope> create_accounting_period(tenant_id, opts)

Creates a new accounting period

Creates a new accounting period.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountingPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  accounting_period_create_dto: OpenapiClient::AccountingPeriodCreateDto.new # AccountingPeriodCreateDto | 
}

begin
  # Creates a new accounting period
  result = api_instance.create_accounting_period(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingPeriodsApi->create_accounting_period: #{e}"
end
```

#### Using the create_accounting_period_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_accounting_period_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new accounting period
  data, status_code, headers = api_instance.create_accounting_period_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingPeriodsApi->create_accounting_period_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **accounting_period_create_dto** | [**AccountingPeriodCreateDto**](AccountingPeriodCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_accounting_period

> <EmptyEnvelope> delete_accounting_period(tenant_id, accounting_period_id, opts)

Deletes an existing accounting period

Deletes an existing accounting period.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountingPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
accounting_period_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes an existing accounting period
  result = api_instance.delete_accounting_period(tenant_id, accounting_period_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingPeriodsApi->delete_accounting_period: #{e}"
end
```

#### Using the delete_accounting_period_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_accounting_period_with_http_info(tenant_id, accounting_period_id, opts)

```ruby
begin
  # Deletes an existing accounting period
  data, status_code, headers = api_instance.delete_accounting_period_with_http_info(tenant_id, accounting_period_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingPeriodsApi->delete_accounting_period_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **accounting_period_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_accounting_period

> <AccountingPeriodDtoEnvelope> get_accounting_period(tenant_id, accounting_period_id, opts)

Gets the current tenant accounting period

Get the currently acting tenant accounting period.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountingPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
accounting_period_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant accounting period
  result = api_instance.get_accounting_period(tenant_id, accounting_period_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingPeriodsApi->get_accounting_period: #{e}"
end
```

#### Using the get_accounting_period_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountingPeriodDtoEnvelope>, Integer, Hash)> get_accounting_period_with_http_info(tenant_id, accounting_period_id, opts)

```ruby
begin
  # Gets the current tenant accounting period
  data, status_code, headers = api_instance.get_accounting_period_with_http_info(tenant_id, accounting_period_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountingPeriodDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingPeriodsApi->get_accounting_period_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **accounting_period_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**AccountingPeriodDtoEnvelope**](AccountingPeriodDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_accounting_periods

> <AccountingPeriodDtoListEnvelope> get_accounting_periods(tenant_id, opts)

Get all accounting periods for a tenant

Retrieves all accounting periods for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountingPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all accounting periods for a tenant
  result = api_instance.get_accounting_periods(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingPeriodsApi->get_accounting_periods: #{e}"
end
```

#### Using the get_accounting_periods_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountingPeriodDtoListEnvelope>, Integer, Hash)> get_accounting_periods_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all accounting periods for a tenant
  data, status_code, headers = api_instance.get_accounting_periods_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountingPeriodDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingPeriodsApi->get_accounting_periods_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**AccountingPeriodDtoListEnvelope**](AccountingPeriodDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_accounting_periods_count_async

> <Int32Envelope> get_accounting_periods_count_async(tenant_id, opts)

Gets the current tenant accounting periods count

Get the currently acting tenant accounting periods count.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountingPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant accounting periods count
  result = api_instance.get_accounting_periods_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingPeriodsApi->get_accounting_periods_count_async: #{e}"
end
```

#### Using the get_accounting_periods_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_accounting_periods_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets the current tenant accounting periods count
  data, status_code, headers = api_instance.get_accounting_periods_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingPeriodsApi->get_accounting_periods_count_async_with_http_info: #{e}"
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


## patch_accounting_period_async

> <EmptyEnvelope> patch_accounting_period_async(tenant_id, accounting_period_id, opts)

Patch an accounting period

Partially updates an accounting period.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountingPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
accounting_period_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch an accounting period
  result = api_instance.patch_accounting_period_async(tenant_id, accounting_period_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingPeriodsApi->patch_accounting_period_async: #{e}"
end
```

#### Using the patch_accounting_period_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_accounting_period_async_with_http_info(tenant_id, accounting_period_id, opts)

```ruby
begin
  # Patch an accounting period
  data, status_code, headers = api_instance.patch_accounting_period_async_with_http_info(tenant_id, accounting_period_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingPeriodsApi->patch_accounting_period_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **accounting_period_id** | **String** |  |  |
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


## update_accounting_period

> <EmptyEnvelope> update_accounting_period(tenant_id, accounting_period_id, opts)

Updates an existing accounting period

Updates an existing accounting period.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountingPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
accounting_period_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  accounting_period_update_dto: OpenapiClient::AccountingPeriodUpdateDto.new # AccountingPeriodUpdateDto | 
}

begin
  # Updates an existing accounting period
  result = api_instance.update_accounting_period(tenant_id, accounting_period_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingPeriodsApi->update_accounting_period: #{e}"
end
```

#### Using the update_accounting_period_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_accounting_period_with_http_info(tenant_id, accounting_period_id, opts)

```ruby
begin
  # Updates an existing accounting period
  data, status_code, headers = api_instance.update_accounting_period_with_http_info(tenant_id, accounting_period_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingPeriodsApi->update_accounting_period_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **accounting_period_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **accounting_period_update_dto** | [**AccountingPeriodUpdateDto**](AccountingPeriodUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

