# OpenapiClient::BusinessRelationshipsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_business_relationships_count_async**](BusinessRelationshipsApi.md#get_business_relationships_count_async) | **GET** /api/v2/TenantsService/BusinessRelationships/Count | Get business relationships count |


## get_business_relationships_count_async

> <Int32Envelope> get_business_relationships_count_async(tenant_id, opts)

Get business relationships count

Returns the count of child business relationships owned by the specified parent tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BusinessRelationshipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get business relationships count
  result = api_instance.get_business_relationships_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessRelationshipsApi->get_business_relationships_count_async: #{e}"
end
```

#### Using the get_business_relationships_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_business_relationships_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get business relationships count
  data, status_code, headers = api_instance.get_business_relationships_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessRelationshipsApi->get_business_relationships_count_async_with_http_info: #{e}"
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

