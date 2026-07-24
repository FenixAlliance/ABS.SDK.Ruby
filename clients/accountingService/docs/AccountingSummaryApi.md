# OpenapiClient::AccountingSummaryApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_credits_sum_async**](AccountingSummaryApi.md#get_credits_sum_async) | **GET** /api/v2/AccountingService/Summary/Credits/Sum | Sum tenant accounting-entry credits |
| [**get_debits_sum_async**](AccountingSummaryApi.md#get_debits_sum_async) | **GET** /api/v2/AccountingService/Summary/Debits/Sum | Sum tenant accounting-entry debits |
| [**get_expenses_sum_async**](AccountingSummaryApi.md#get_expenses_sum_async) | **GET** /api/v2/AccountingService/Summary/Expenses/Sum | Sum tenant expenses |
| [**get_incomes_sum_async**](AccountingSummaryApi.md#get_incomes_sum_async) | **GET** /api/v2/AccountingService/Summary/Incomes/Sum | Sum tenant incomes |


## get_credits_sum_async

> <DecimalEnvelope> get_credits_sum_async(tenant_id, opts)

Sum tenant accounting-entry credits

Returns SUM(AccountingEntry.Credit) for the tenant, filtered by the supplied OData date range.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountingSummaryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Sum tenant accounting-entry credits
  result = api_instance.get_credits_sum_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingSummaryApi->get_credits_sum_async: #{e}"
end
```

#### Using the get_credits_sum_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<DecimalEnvelope>, Integer, Hash)> get_credits_sum_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Sum tenant accounting-entry credits
  data, status_code, headers = api_instance.get_credits_sum_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <DecimalEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingSummaryApi->get_credits_sum_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**DecimalEnvelope**](DecimalEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_debits_sum_async

> <DecimalEnvelope> get_debits_sum_async(tenant_id, opts)

Sum tenant accounting-entry debits

Returns SUM(AccountingEntry.Debit) for the tenant, filtered by the supplied OData date range.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountingSummaryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Sum tenant accounting-entry debits
  result = api_instance.get_debits_sum_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingSummaryApi->get_debits_sum_async: #{e}"
end
```

#### Using the get_debits_sum_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<DecimalEnvelope>, Integer, Hash)> get_debits_sum_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Sum tenant accounting-entry debits
  data, status_code, headers = api_instance.get_debits_sum_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <DecimalEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingSummaryApi->get_debits_sum_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**DecimalEnvelope**](DecimalEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_expenses_sum_async

> <MoneyEnvelope> get_expenses_sum_async(tenant_id, opts)

Sum tenant expenses

Returns SUM(JournalEntry.Debit) for Debit-direction journal entries in the tenant, filtered by the supplied OData date range.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountingSummaryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Sum tenant expenses
  result = api_instance.get_expenses_sum_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingSummaryApi->get_expenses_sum_async: #{e}"
end
```

#### Using the get_expenses_sum_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MoneyEnvelope>, Integer, Hash)> get_expenses_sum_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Sum tenant expenses
  data, status_code, headers = api_instance.get_expenses_sum_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MoneyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingSummaryApi->get_expenses_sum_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_incomes_sum_async

> <MoneyEnvelope> get_incomes_sum_async(tenant_id, opts)

Sum tenant incomes

Returns SUM(JournalEntry.Credit) for Credit-direction journal entries in the tenant, filtered by the supplied OData date range.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountingSummaryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Sum tenant incomes
  result = api_instance.get_incomes_sum_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingSummaryApi->get_incomes_sum_async: #{e}"
end
```

#### Using the get_incomes_sum_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MoneyEnvelope>, Integer, Hash)> get_incomes_sum_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Sum tenant incomes
  data, status_code, headers = api_instance.get_incomes_sum_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MoneyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountingSummaryApi->get_incomes_sum_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

