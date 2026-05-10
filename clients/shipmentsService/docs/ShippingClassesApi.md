# OpenapiClient::ShippingClassesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_shipping_class_async**](ShippingClassesApi.md#create_shipping_class_async) | **POST** /api/v2/ShipmentsService/ShippingClasses | Create a shipping class |
| [**delete_shipping_class_async**](ShippingClassesApi.md#delete_shipping_class_async) | **DELETE** /api/v2/ShipmentsService/ShippingClasses/{classId} | Delete a shipping class |
| [**get_shipping_class_by_id_async**](ShippingClassesApi.md#get_shipping_class_by_id_async) | **GET** /api/v2/ShipmentsService/ShippingClasses/{classId} | Get shipping class by ID |
| [**get_shipping_classes_async**](ShippingClassesApi.md#get_shipping_classes_async) | **GET** /api/v2/ShipmentsService/ShippingClasses | Get all shipping classes |
| [**get_shipping_classes_count_async**](ShippingClassesApi.md#get_shipping_classes_count_async) | **GET** /api/v2/ShipmentsService/ShippingClasses/Count | Get shipping classes count |
| [**update_shipping_class_async**](ShippingClassesApi.md#update_shipping_class_async) | **PUT** /api/v2/ShipmentsService/ShippingClasses/{classId} | Update a shipping class |


## create_shipping_class_async

> create_shipping_class_async(tenant_id, opts)

Create a shipping class

Creates a new shipping class.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingClassesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipping_class_create_dto: OpenapiClient::ShippingClassCreateDto.new({name: 'name_example'}) # ShippingClassCreateDto | 
}

begin
  # Create a shipping class
  api_instance.create_shipping_class_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingClassesApi->create_shipping_class_async: #{e}"
end
```

#### Using the create_shipping_class_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_shipping_class_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a shipping class
  data, status_code, headers = api_instance.create_shipping_class_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingClassesApi->create_shipping_class_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipping_class_create_dto** | [**ShippingClassCreateDto**](ShippingClassCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_shipping_class_async

> delete_shipping_class_async(tenant_id, class_id, opts)

Delete a shipping class

Deletes a shipping class.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingClassesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
class_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a shipping class
  api_instance.delete_shipping_class_async(tenant_id, class_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingClassesApi->delete_shipping_class_async: #{e}"
end
```

#### Using the delete_shipping_class_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_shipping_class_async_with_http_info(tenant_id, class_id, opts)

```ruby
begin
  # Delete a shipping class
  data, status_code, headers = api_instance.delete_shipping_class_async_with_http_info(tenant_id, class_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingClassesApi->delete_shipping_class_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **class_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shipping_class_by_id_async

> <ShippingClassDtoEnvelope> get_shipping_class_by_id_async(tenant_id, class_id, opts)

Get shipping class by ID

Retrieves a specific shipping class.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingClassesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
class_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get shipping class by ID
  result = api_instance.get_shipping_class_by_id_async(tenant_id, class_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingClassesApi->get_shipping_class_by_id_async: #{e}"
end
```

#### Using the get_shipping_class_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShippingClassDtoEnvelope>, Integer, Hash)> get_shipping_class_by_id_async_with_http_info(tenant_id, class_id, opts)

```ruby
begin
  # Get shipping class by ID
  data, status_code, headers = api_instance.get_shipping_class_by_id_async_with_http_info(tenant_id, class_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShippingClassDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingClassesApi->get_shipping_class_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **class_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShippingClassDtoEnvelope**](ShippingClassDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shipping_classes_async

> <ShippingClassDtoListEnvelope> get_shipping_classes_async(tenant_id, opts)

Get all shipping classes

Retrieves all shipping classes for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingClassesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all shipping classes
  result = api_instance.get_shipping_classes_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingClassesApi->get_shipping_classes_async: #{e}"
end
```

#### Using the get_shipping_classes_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShippingClassDtoListEnvelope>, Integer, Hash)> get_shipping_classes_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all shipping classes
  data, status_code, headers = api_instance.get_shipping_classes_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShippingClassDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingClassesApi->get_shipping_classes_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShippingClassDtoListEnvelope**](ShippingClassDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shipping_classes_count_async

> <Int32Envelope> get_shipping_classes_count_async(tenant_id, opts)

Get shipping classes count

Returns the count of shipping classes.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingClassesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get shipping classes count
  result = api_instance.get_shipping_classes_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingClassesApi->get_shipping_classes_count_async: #{e}"
end
```

#### Using the get_shipping_classes_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_shipping_classes_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get shipping classes count
  data, status_code, headers = api_instance.get_shipping_classes_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingClassesApi->get_shipping_classes_count_async_with_http_info: #{e}"
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


## update_shipping_class_async

> update_shipping_class_async(tenant_id, class_id, opts)

Update a shipping class

Updates an existing shipping class.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingClassesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
class_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipping_class_update_dto: OpenapiClient::ShippingClassUpdateDto.new # ShippingClassUpdateDto | 
}

begin
  # Update a shipping class
  api_instance.update_shipping_class_async(tenant_id, class_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingClassesApi->update_shipping_class_async: #{e}"
end
```

#### Using the update_shipping_class_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_shipping_class_async_with_http_info(tenant_id, class_id, opts)

```ruby
begin
  # Update a shipping class
  data, status_code, headers = api_instance.update_shipping_class_async_with_http_info(tenant_id, class_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingClassesApi->update_shipping_class_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **class_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipping_class_update_dto** | [**ShippingClassUpdateDto**](ShippingClassUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

