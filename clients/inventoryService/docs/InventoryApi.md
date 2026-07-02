# OpenapiClient::InventoryApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_inventory_details_async**](InventoryApi.md#get_inventory_details_async) | **GET** /api/v2/InventoryService/Inventory/{stockItemId}/Details | Get inventory details for a stock item |


## get_inventory_details_async

> get_inventory_details_async(stock_item_id, opts)

Get inventory details for a stock item

Retrieves the inventory details for a specific stock item by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InventoryApi.new
stock_item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get inventory details for a stock item
  api_instance.get_inventory_details_async(stock_item_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling InventoryApi->get_inventory_details_async: #{e}"
end
```

#### Using the get_inventory_details_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> get_inventory_details_async_with_http_info(stock_item_id, opts)

```ruby
begin
  # Get inventory details for a stock item
  data, status_code, headers = api_instance.get_inventory_details_async_with_http_info(stock_item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling InventoryApi->get_inventory_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **stock_item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

