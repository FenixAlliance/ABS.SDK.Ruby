# OpenapiClient::AccountingEntriesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_credits_sum_async**](AccountingEntriesApi.md#get_credits_sum_async) | **GET** /api/v2/AccountingService/AccountingEntries/Credits/Sum | Sum tenant accounting-entry credits |
| [**get_debits_sum_async**](AccountingEntriesApi.md#get_debits_sum_async) | **GET** /api/v2/AccountingService/AccountingEntries/Debits/Sum | Sum tenant accounting-entry debits |


## get_credits_sum_async

> <DecimalEnvelope> get_credits_sum_async(tenant_id, opts)

Sum tenant accounting-entry credits

Returns SUM(AccountingEntry.Credit) for the tenant, filtered by the supplied OData date range.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountingEntriesApi.new
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
  puts "Error when calling AccountingEntriesApi->get_credits_sum_async: #{e}"
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
  puts "Error when calling AccountingEntriesApi->get_credits_sum_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::AccountingEntriesApi.new
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
  puts "Error when calling AccountingEntriesApi->get_debits_sum_async: #{e}"
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
  puts "Error when calling AccountingEntriesApi->get_debits_sum_async_with_http_info: #{e}"
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

