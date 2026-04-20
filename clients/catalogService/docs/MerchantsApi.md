# OpenapiClient::MerchantsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_merchant_by_id**](MerchantsApi.md#get_merchant_by_id) | **GET** /api/v2/CatalogService/Merchants/{merchantId} | Get merchant by ID |
| [**get_merchants**](MerchantsApi.md#get_merchants) | **GET** /api/v2/CatalogService/Merchants | Get all merchants |
| [**get_merchants_count**](MerchantsApi.md#get_merchants_count) | **GET** /api/v2/CatalogService/Merchants/Count | Count merchants |


## get_merchant_by_id

> <MerchantDtoEnvelope> get_merchant_by_id(merchant_id, opts)

Get merchant by ID

Retrieves a merchant by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MerchantsApi.new
merchant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get merchant by ID
  result = api_instance.get_merchant_by_id(merchant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MerchantsApi->get_merchant_by_id: #{e}"
end
```

#### Using the get_merchant_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MerchantDtoEnvelope>, Integer, Hash)> get_merchant_by_id_with_http_info(merchant_id, opts)

```ruby
begin
  # Get merchant by ID
  data, status_code, headers = api_instance.get_merchant_by_id_with_http_info(merchant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MerchantDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MerchantsApi->get_merchant_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **merchant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MerchantDtoEnvelope**](MerchantDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_merchants

> <MerchantDtoListEnvelope> get_merchants(opts)

Get all merchants

Retrieves all merchants, optionally filtered by OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MerchantsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all merchants
  result = api_instance.get_merchants(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MerchantsApi->get_merchants: #{e}"
end
```

#### Using the get_merchants_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MerchantDtoListEnvelope>, Integer, Hash)> get_merchants_with_http_info(opts)

```ruby
begin
  # Get all merchants
  data, status_code, headers = api_instance.get_merchants_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MerchantDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MerchantsApi->get_merchants_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MerchantDtoListEnvelope**](MerchantDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_merchants_count

> <Int32Envelope> get_merchants_count(opts)

Count merchants

Counts the number of merchants, optionally filtered by OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MerchantsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count merchants
  result = api_instance.get_merchants_count(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MerchantsApi->get_merchants_count: #{e}"
end
```

#### Using the get_merchants_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_merchants_count_with_http_info(opts)

```ruby
begin
  # Count merchants
  data, status_code, headers = api_instance.get_merchants_count_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MerchantsApi->get_merchants_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

