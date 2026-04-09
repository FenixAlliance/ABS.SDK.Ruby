# OpenapiClient::ShipmentsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_shipments_async**](ShipmentsApi.md#get_shipments_async) | **GET** /api/v2/ShipmentsService/Shipments | Retrieve a list of shipments |


## get_shipments_async

> <ShipmentDtoListEnvelope> get_shipments_async(tenant_id, opts)

Retrieve a list of shipments

Retrieves a list of shipments for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShipmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of shipments
  result = api_instance.get_shipments_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShipmentsApi->get_shipments_async: #{e}"
end
```

#### Using the get_shipments_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShipmentDtoListEnvelope>, Integer, Hash)> get_shipments_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of shipments
  data, status_code, headers = api_instance.get_shipments_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShipmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShipmentsApi->get_shipments_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShipmentDtoListEnvelope**](ShipmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

