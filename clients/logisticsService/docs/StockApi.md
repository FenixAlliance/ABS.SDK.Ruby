# OpenapiClient::StockApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_contacts_async**](StockApi.md#get_contacts_async) | **GET** /api/v2/LogisticsService/Stock | Get all stock-related contacts |


## get_contacts_async

> <ContactDtoListEnvelope> get_contacts_async(tenant_id, opts)

Get all stock-related contacts

Retrieves all business-owned contacts related to stock and logistics for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::StockApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all stock-related contacts
  result = api_instance.get_contacts_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling StockApi->get_contacts_async: #{e}"
end
```

#### Using the get_contacts_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactDtoListEnvelope>, Integer, Hash)> get_contacts_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all stock-related contacts
  data, status_code, headers = api_instance.get_contacts_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling StockApi->get_contacts_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

