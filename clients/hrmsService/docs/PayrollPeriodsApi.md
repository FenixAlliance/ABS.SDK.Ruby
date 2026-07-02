# OpenapiClient::PayrollPeriodsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_payroll_period_async**](PayrollPeriodsApi.md#create_payroll_period_async) | **POST** /api/v2/HrmsService/PayrollPeriods | Create a payroll period |
| [**delete_payroll_period_async**](PayrollPeriodsApi.md#delete_payroll_period_async) | **DELETE** /api/v2/HrmsService/PayrollPeriods/{periodId} | Delete a payroll period |
| [**get_payroll_period_by_id_async**](PayrollPeriodsApi.md#get_payroll_period_by_id_async) | **GET** /api/v2/HrmsService/PayrollPeriods/{periodId} | Get payroll period by ID |
| [**get_payroll_periods_async**](PayrollPeriodsApi.md#get_payroll_periods_async) | **GET** /api/v2/HrmsService/PayrollPeriods | Get payroll periods |
| [**get_payroll_periods_count_async**](PayrollPeriodsApi.md#get_payroll_periods_count_async) | **GET** /api/v2/HrmsService/PayrollPeriods/Count | Count payroll periods |
| [**update_payroll_period_async**](PayrollPeriodsApi.md#update_payroll_period_async) | **PUT** /api/v2/HrmsService/PayrollPeriods/{periodId} | Update a payroll period |


## create_payroll_period_async

> <EmptyEnvelope> create_payroll_period_async(tenant_id, opts)

Create a payroll period

Creates a new payroll period for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PayrollPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  payroll_period_create_dto: OpenapiClient::PayrollPeriodCreateDto.new({title: 'title_example', start_date: Time.now, end_date: Time.now}) # PayrollPeriodCreateDto | 
}

begin
  # Create a payroll period
  result = api_instance.create_payroll_period_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollPeriodsApi->create_payroll_period_async: #{e}"
end
```

#### Using the create_payroll_period_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_payroll_period_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a payroll period
  data, status_code, headers = api_instance.create_payroll_period_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollPeriodsApi->create_payroll_period_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **payroll_period_create_dto** | [**PayrollPeriodCreateDto**](PayrollPeriodCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_payroll_period_async

> <EmptyEnvelope> delete_payroll_period_async(tenant_id, period_id, opts)

Delete a payroll period

Deletes a payroll period for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PayrollPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
period_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a payroll period
  result = api_instance.delete_payroll_period_async(tenant_id, period_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollPeriodsApi->delete_payroll_period_async: #{e}"
end
```

#### Using the delete_payroll_period_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_payroll_period_async_with_http_info(tenant_id, period_id, opts)

```ruby
begin
  # Delete a payroll period
  data, status_code, headers = api_instance.delete_payroll_period_async_with_http_info(tenant_id, period_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollPeriodsApi->delete_payroll_period_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **period_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payroll_period_by_id_async

> <PayrollPeriodDtoEnvelope> get_payroll_period_by_id_async(tenant_id, period_id, opts)

Get payroll period by ID

Retrieves a specific payroll period by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PayrollPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
period_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get payroll period by ID
  result = api_instance.get_payroll_period_by_id_async(tenant_id, period_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollPeriodsApi->get_payroll_period_by_id_async: #{e}"
end
```

#### Using the get_payroll_period_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PayrollPeriodDtoEnvelope>, Integer, Hash)> get_payroll_period_by_id_async_with_http_info(tenant_id, period_id, opts)

```ruby
begin
  # Get payroll period by ID
  data, status_code, headers = api_instance.get_payroll_period_by_id_async_with_http_info(tenant_id, period_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PayrollPeriodDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollPeriodsApi->get_payroll_period_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **period_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PayrollPeriodDtoEnvelope**](PayrollPeriodDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payroll_periods_async

> <PayrollPeriodDtoListEnvelope> get_payroll_periods_async(tenant_id, opts)

Get payroll periods

Retrieves payroll periods for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PayrollPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get payroll periods
  result = api_instance.get_payroll_periods_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollPeriodsApi->get_payroll_periods_async: #{e}"
end
```

#### Using the get_payroll_periods_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PayrollPeriodDtoListEnvelope>, Integer, Hash)> get_payroll_periods_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get payroll periods
  data, status_code, headers = api_instance.get_payroll_periods_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PayrollPeriodDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollPeriodsApi->get_payroll_periods_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PayrollPeriodDtoListEnvelope**](PayrollPeriodDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payroll_periods_count_async

> <Int32Envelope> get_payroll_periods_count_async(tenant_id, opts)

Count payroll periods

Counts payroll periods for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PayrollPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count payroll periods
  result = api_instance.get_payroll_periods_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollPeriodsApi->get_payroll_periods_count_async: #{e}"
end
```

#### Using the get_payroll_periods_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_payroll_periods_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count payroll periods
  data, status_code, headers = api_instance.get_payroll_periods_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollPeriodsApi->get_payroll_periods_count_async_with_http_info: #{e}"
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


## update_payroll_period_async

> <EmptyEnvelope> update_payroll_period_async(tenant_id, period_id, opts)

Update a payroll period

Updates an existing payroll period for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PayrollPeriodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
period_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  payroll_period_update_dto: OpenapiClient::PayrollPeriodUpdateDto.new # PayrollPeriodUpdateDto | 
}

begin
  # Update a payroll period
  result = api_instance.update_payroll_period_async(tenant_id, period_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollPeriodsApi->update_payroll_period_async: #{e}"
end
```

#### Using the update_payroll_period_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_payroll_period_async_with_http_info(tenant_id, period_id, opts)

```ruby
begin
  # Update a payroll period
  data, status_code, headers = api_instance.update_payroll_period_async_with_http_info(tenant_id, period_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollPeriodsApi->update_payroll_period_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **period_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **payroll_period_update_dto** | [**PayrollPeriodUpdateDto**](PayrollPeriodUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

