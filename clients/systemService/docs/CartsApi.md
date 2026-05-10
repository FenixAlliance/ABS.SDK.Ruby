# OpenapiClient::CartsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**delete_system_cart**](CartsApi.md#delete_system_cart) | **DELETE** /api/v2/SystemService/Carts/{cartId} | Delete a system cart |
| [**get_system_cart_by_id**](CartsApi.md#get_system_cart_by_id) | **GET** /api/v2/SystemService/Carts/{cartId} | Retrieve a single system cart by its ID |
| [**get_system_carts**](CartsApi.md#get_system_carts) | **GET** /api/v2/SystemService/Carts | Retrieve a list of system carts |
| [**get_system_carts_count**](CartsApi.md#get_system_carts_count) | **GET** /api/v2/SystemService/Carts/Count | Get the count of system carts |


## delete_system_cart

> <EmptyEnvelope> delete_system_cart(cart_id, opts)

Delete a system cart

Delete a system cart by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a system cart
  result = api_instance.delete_system_cart(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->delete_system_cart: #{e}"
end
```

#### Using the delete_system_cart_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_system_cart_with_http_info(cart_id, opts)

```ruby
begin
  # Delete a system cart
  data, status_code, headers = api_instance.delete_system_cart_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->delete_system_cart_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_system_cart_by_id

> <CartDtoEnvelope> get_system_cart_by_id(cart_id, opts)

Retrieve a single system cart by its ID

Retrieve a single system cart by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single system cart by its ID
  result = api_instance.get_system_cart_by_id(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_system_cart_by_id: #{e}"
end
```

#### Using the get_system_cart_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CartDtoEnvelope>, Integer, Hash)> get_system_cart_by_id_with_http_info(cart_id, opts)

```ruby
begin
  # Retrieve a single system cart by its ID
  data, status_code, headers = api_instance.get_system_cart_by_id_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CartDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_system_cart_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CartDtoEnvelope**](CartDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_system_carts

> <CartDtoListEnvelope> get_system_carts(opts)

Retrieve a list of system carts

Retrieve a list of all carts in the system

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of system carts
  result = api_instance.get_system_carts(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_system_carts: #{e}"
end
```

#### Using the get_system_carts_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CartDtoListEnvelope>, Integer, Hash)> get_system_carts_with_http_info(opts)

```ruby
begin
  # Retrieve a list of system carts
  data, status_code, headers = api_instance.get_system_carts_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CartDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_system_carts_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CartDtoListEnvelope**](CartDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_system_carts_count

> <Int32Envelope> get_system_carts_count(opts)

Get the count of system carts

Get the count of all carts in the system

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of system carts
  result = api_instance.get_system_carts_count(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_system_carts_count: #{e}"
end
```

#### Using the get_system_carts_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_system_carts_count_with_http_info(opts)

```ruby
begin
  # Get the count of system carts
  data, status_code, headers = api_instance.get_system_carts_count_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_system_carts_count_with_http_info: #{e}"
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

