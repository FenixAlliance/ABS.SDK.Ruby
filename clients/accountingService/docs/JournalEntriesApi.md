# OpenapiClient::JournalEntriesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_expenses_sum_async**](JournalEntriesApi.md#get_expenses_sum_async) | **GET** /api/v2/AccountingService/JournalEntries/Expenses/Sum | Sum tenant expenses |
| [**get_incomes_sum_async**](JournalEntriesApi.md#get_incomes_sum_async) | **GET** /api/v2/AccountingService/JournalEntries/Incomes/Sum | Sum tenant incomes |


## get_expenses_sum_async

> <DecimalEnvelope> get_expenses_sum_async(tenant_id, opts)

Sum tenant expenses

Returns SUM(JournalEntry.Debit) for Debit-direction journal entries in the tenant, filtered by the supplied OData date range.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalEntriesApi.new
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
  puts "Error when calling JournalEntriesApi->get_expenses_sum_async: #{e}"
end
```

#### Using the get_expenses_sum_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<DecimalEnvelope>, Integer, Hash)> get_expenses_sum_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Sum tenant expenses
  data, status_code, headers = api_instance.get_expenses_sum_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <DecimalEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalEntriesApi->get_expenses_sum_async_with_http_info: #{e}"
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


## get_incomes_sum_async

> <DecimalEnvelope> get_incomes_sum_async(tenant_id, opts)

Sum tenant incomes

Returns SUM(JournalEntry.Credit) for Credit-direction journal entries in the tenant, filtered by the supplied OData date range.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalEntriesApi.new
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
  puts "Error when calling JournalEntriesApi->get_incomes_sum_async: #{e}"
end
```

#### Using the get_incomes_sum_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<DecimalEnvelope>, Integer, Hash)> get_incomes_sum_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Sum tenant incomes
  data, status_code, headers = api_instance.get_incomes_sum_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <DecimalEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalEntriesApi->get_incomes_sum_async_with_http_info: #{e}"
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

