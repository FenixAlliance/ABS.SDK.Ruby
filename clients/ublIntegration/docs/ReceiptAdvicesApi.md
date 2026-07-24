# OpenapiClient::ReceiptAdvicesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**api_v2_ubl_service_receipt_advices_item_restock_id_get**](ReceiptAdvicesApi.md#api_v2_ubl_service_receipt_advices_item_restock_id_get) | **GET** /api/v2/UblService/ReceiptAdvices/{itemRestockId} |  |
| [**api_v2_ubl_service_receipt_advices_item_restock_id_partitions_get**](ReceiptAdvicesApi.md#api_v2_ubl_service_receipt_advices_item_restock_id_partitions_get) | **GET** /api/v2/UblService/ReceiptAdvices/{itemRestockId}/partitions |  |


## api_v2_ubl_service_receipt_advices_item_restock_id_get

> api_v2_ubl_service_receipt_advices_item_restock_id_get(tenant_id, item_restock_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReceiptAdvicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_restock_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  profile: 'Generic', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  api_instance.api_v2_ubl_service_receipt_advices_item_restock_id_get(tenant_id, item_restock_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReceiptAdvicesApi->api_v2_ubl_service_receipt_advices_item_restock_id_get: #{e}"
end
```

#### Using the api_v2_ubl_service_receipt_advices_item_restock_id_get_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> api_v2_ubl_service_receipt_advices_item_restock_id_get_with_http_info(tenant_id, item_restock_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_v2_ubl_service_receipt_advices_item_restock_id_get_with_http_info(tenant_id, item_restock_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReceiptAdvicesApi->api_v2_ubl_service_receipt_advices_item_restock_id_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_restock_id** | **String** |  |  |
| **profile** | **String** |  | [optional][default to &#39;Generic&#39;] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## api_v2_ubl_service_receipt_advices_item_restock_id_partitions_get

> api_v2_ubl_service_receipt_advices_item_restock_id_partitions_get(tenant_id, item_restock_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReceiptAdvicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_restock_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  profile: 'Generic', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  api_instance.api_v2_ubl_service_receipt_advices_item_restock_id_partitions_get(tenant_id, item_restock_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReceiptAdvicesApi->api_v2_ubl_service_receipt_advices_item_restock_id_partitions_get: #{e}"
end
```

#### Using the api_v2_ubl_service_receipt_advices_item_restock_id_partitions_get_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> api_v2_ubl_service_receipt_advices_item_restock_id_partitions_get_with_http_info(tenant_id, item_restock_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_v2_ubl_service_receipt_advices_item_restock_id_partitions_get_with_http_info(tenant_id, item_restock_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReceiptAdvicesApi->api_v2_ubl_service_receipt_advices_item_restock_id_partitions_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_restock_id** | **String** |  |  |
| **profile** | **String** |  | [optional][default to &#39;Generic&#39;] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

