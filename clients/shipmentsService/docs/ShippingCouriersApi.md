# OpenapiClient::ShippingCouriersApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_shipping_courier_async**](ShippingCouriersApi.md#create_shipping_courier_async) | **POST** /api/v2/ShipmentsService/ShippingCouriers | Create a shipping courier |
| [**delete_shipping_courier_async**](ShippingCouriersApi.md#delete_shipping_courier_async) | **DELETE** /api/v2/ShipmentsService/ShippingCouriers/{courierId} | Delete a shipping courier |
| [**get_shipping_courier_by_id_async**](ShippingCouriersApi.md#get_shipping_courier_by_id_async) | **GET** /api/v2/ShipmentsService/ShippingCouriers/{courierId} | Get shipping courier by ID |
| [**get_shipping_couriers_async**](ShippingCouriersApi.md#get_shipping_couriers_async) | **GET** /api/v2/ShipmentsService/ShippingCouriers | Get all shipping couriers |
| [**get_shipping_couriers_count_async**](ShippingCouriersApi.md#get_shipping_couriers_count_async) | **GET** /api/v2/ShipmentsService/ShippingCouriers/Count | Get shipping couriers count |
| [**update_shipping_courier_async**](ShippingCouriersApi.md#update_shipping_courier_async) | **PUT** /api/v2/ShipmentsService/ShippingCouriers/{courierId} | Update a shipping courier |


## create_shipping_courier_async

> create_shipping_courier_async(tenant_id, opts)

Create a shipping courier

Creates a new shipping courier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingCouriersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipping_courier_create_dto: OpenapiClient::ShippingCourierCreateDto.new({name: 'name_example'}) # ShippingCourierCreateDto | 
}

begin
  # Create a shipping courier
  api_instance.create_shipping_courier_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingCouriersApi->create_shipping_courier_async: #{e}"
end
```

#### Using the create_shipping_courier_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_shipping_courier_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a shipping courier
  data, status_code, headers = api_instance.create_shipping_courier_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingCouriersApi->create_shipping_courier_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipping_courier_create_dto** | [**ShippingCourierCreateDto**](ShippingCourierCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_shipping_courier_async

> delete_shipping_courier_async(tenant_id, courier_id, opts)

Delete a shipping courier

Deletes a shipping courier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingCouriersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
courier_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a shipping courier
  api_instance.delete_shipping_courier_async(tenant_id, courier_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingCouriersApi->delete_shipping_courier_async: #{e}"
end
```

#### Using the delete_shipping_courier_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_shipping_courier_async_with_http_info(tenant_id, courier_id, opts)

```ruby
begin
  # Delete a shipping courier
  data, status_code, headers = api_instance.delete_shipping_courier_async_with_http_info(tenant_id, courier_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingCouriersApi->delete_shipping_courier_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **courier_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shipping_courier_by_id_async

> <ShippingCourierDtoEnvelope> get_shipping_courier_by_id_async(tenant_id, courier_id, opts)

Get shipping courier by ID

Retrieves a specific shipping courier by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingCouriersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
courier_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get shipping courier by ID
  result = api_instance.get_shipping_courier_by_id_async(tenant_id, courier_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingCouriersApi->get_shipping_courier_by_id_async: #{e}"
end
```

#### Using the get_shipping_courier_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShippingCourierDtoEnvelope>, Integer, Hash)> get_shipping_courier_by_id_async_with_http_info(tenant_id, courier_id, opts)

```ruby
begin
  # Get shipping courier by ID
  data, status_code, headers = api_instance.get_shipping_courier_by_id_async_with_http_info(tenant_id, courier_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShippingCourierDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingCouriersApi->get_shipping_courier_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **courier_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShippingCourierDtoEnvelope**](ShippingCourierDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shipping_couriers_async

> <ShippingCourierDtoListEnvelope> get_shipping_couriers_async(tenant_id, opts)

Get all shipping couriers

Retrieves all shipping couriers for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingCouriersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all shipping couriers
  result = api_instance.get_shipping_couriers_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingCouriersApi->get_shipping_couriers_async: #{e}"
end
```

#### Using the get_shipping_couriers_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShippingCourierDtoListEnvelope>, Integer, Hash)> get_shipping_couriers_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all shipping couriers
  data, status_code, headers = api_instance.get_shipping_couriers_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShippingCourierDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingCouriersApi->get_shipping_couriers_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShippingCourierDtoListEnvelope**](ShippingCourierDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shipping_couriers_count_async

> <Int32Envelope> get_shipping_couriers_count_async(tenant_id, opts)

Get shipping couriers count

Returns the count of shipping couriers for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingCouriersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get shipping couriers count
  result = api_instance.get_shipping_couriers_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingCouriersApi->get_shipping_couriers_count_async: #{e}"
end
```

#### Using the get_shipping_couriers_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_shipping_couriers_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get shipping couriers count
  data, status_code, headers = api_instance.get_shipping_couriers_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingCouriersApi->get_shipping_couriers_count_async_with_http_info: #{e}"
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


## update_shipping_courier_async

> update_shipping_courier_async(tenant_id, courier_id, opts)

Update a shipping courier

Updates an existing shipping courier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingCouriersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
courier_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipping_courier_update_dto: OpenapiClient::ShippingCourierUpdateDto.new # ShippingCourierUpdateDto | 
}

begin
  # Update a shipping courier
  api_instance.update_shipping_courier_async(tenant_id, courier_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingCouriersApi->update_shipping_courier_async: #{e}"
end
```

#### Using the update_shipping_courier_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_shipping_courier_async_with_http_info(tenant_id, courier_id, opts)

```ruby
begin
  # Update a shipping courier
  data, status_code, headers = api_instance.update_shipping_courier_async_with_http_info(tenant_id, courier_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingCouriersApi->update_shipping_courier_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **courier_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipping_courier_update_dto** | [**ShippingCourierUpdateDto**](ShippingCourierUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

