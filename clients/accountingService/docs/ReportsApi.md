# OpenapiClient::ReportsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_trial_balance_async**](ReportsApi.md#get_trial_balance_async) | **GET** /api/v2/AccountingService/Reports/TrialBalance | Trial balance for a fiscal period |


## get_trial_balance_async

> <TrialBalanceDtoEnvelope> get_trial_balance_async(tenant_id, fiscal_period_id, opts)

Trial balance for a fiscal period

Returns the per-account posted debit/credit totals for the given fiscal period (optionally scoped to a single financial book), plus grand totals and the Σdebits == Σcredits balanced flag. Amounts are normalized to the target currency (default USD) from the stored USD reporting amounts.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReportsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_period_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  financial_book_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  currency_id: 'currency_id_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Trial balance for a fiscal period
  result = api_instance.get_trial_balance_async(tenant_id, fiscal_period_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReportsApi->get_trial_balance_async: #{e}"
end
```

#### Using the get_trial_balance_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TrialBalanceDtoEnvelope>, Integer, Hash)> get_trial_balance_async_with_http_info(tenant_id, fiscal_period_id, opts)

```ruby
begin
  # Trial balance for a fiscal period
  data, status_code, headers = api_instance.get_trial_balance_async_with_http_info(tenant_id, fiscal_period_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TrialBalanceDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReportsApi->get_trial_balance_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_period_id** | **String** |  |  |
| **financial_book_id** | **String** |  | [optional] |
| **currency_id** | **String** |  | [optional][default to &#39;USD.USA&#39;] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TrialBalanceDtoEnvelope**](TrialBalanceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

