# OpenapiClient::ShippingMethodsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_shipping_method_async**](ShippingMethodsApi.md#create_shipping_method_async) | **POST** /api/v2/ShipmentsService/ShippingMethods | Create a shipping method |
| [**delete_shipping_method_async**](ShippingMethodsApi.md#delete_shipping_method_async) | **DELETE** /api/v2/ShipmentsService/ShippingMethods/{methodId} | Delete a shipping method |
| [**get_shipping_method_by_id_async**](ShippingMethodsApi.md#get_shipping_method_by_id_async) | **GET** /api/v2/ShipmentsService/ShippingMethods/{methodId} | Get shipping method by ID |
| [**get_shipping_methods_async**](ShippingMethodsApi.md#get_shipping_methods_async) | **GET** /api/v2/ShipmentsService/ShippingMethods | Get all shipping methods |
| [**get_shipping_methods_count_async**](ShippingMethodsApi.md#get_shipping_methods_count_async) | **GET** /api/v2/ShipmentsService/ShippingMethods/Count | Get shipping methods count |
| [**patch_shipping_method_async**](ShippingMethodsApi.md#patch_shipping_method_async) | **PATCH** /api/v2/ShipmentsService/ShippingMethods/{methodId} | Patch a shipping method |
| [**update_shipping_method_async**](ShippingMethodsApi.md#update_shipping_method_async) | **PUT** /api/v2/ShipmentsService/ShippingMethods/{methodId} | Update a shipping method |


## create_shipping_method_async

> create_shipping_method_async(tenant_id, opts)

Create a shipping method

Creates a new shipping method.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingMethodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipping_method_create_dto: OpenapiClient::ShippingMethodCreateDto.new({name: 'name_example'}) # ShippingMethodCreateDto | 
}

begin
  # Create a shipping method
  api_instance.create_shipping_method_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingMethodsApi->create_shipping_method_async: #{e}"
end
```

#### Using the create_shipping_method_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_shipping_method_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a shipping method
  data, status_code, headers = api_instance.create_shipping_method_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingMethodsApi->create_shipping_method_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipping_method_create_dto** | [**ShippingMethodCreateDto**](ShippingMethodCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_shipping_method_async

> delete_shipping_method_async(tenant_id, method_id, opts)

Delete a shipping method

Deletes a shipping method.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingMethodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
method_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a shipping method
  api_instance.delete_shipping_method_async(tenant_id, method_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingMethodsApi->delete_shipping_method_async: #{e}"
end
```

#### Using the delete_shipping_method_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_shipping_method_async_with_http_info(tenant_id, method_id, opts)

```ruby
begin
  # Delete a shipping method
  data, status_code, headers = api_instance.delete_shipping_method_async_with_http_info(tenant_id, method_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingMethodsApi->delete_shipping_method_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **method_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shipping_method_by_id_async

> <ShippingMethodDtoEnvelope> get_shipping_method_by_id_async(tenant_id, method_id, opts)

Get shipping method by ID

Retrieves a specific shipping method.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingMethodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
method_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get shipping method by ID
  result = api_instance.get_shipping_method_by_id_async(tenant_id, method_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingMethodsApi->get_shipping_method_by_id_async: #{e}"
end
```

#### Using the get_shipping_method_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShippingMethodDtoEnvelope>, Integer, Hash)> get_shipping_method_by_id_async_with_http_info(tenant_id, method_id, opts)

```ruby
begin
  # Get shipping method by ID
  data, status_code, headers = api_instance.get_shipping_method_by_id_async_with_http_info(tenant_id, method_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShippingMethodDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingMethodsApi->get_shipping_method_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **method_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShippingMethodDtoEnvelope**](ShippingMethodDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shipping_methods_async

> <ShippingMethodDtoListEnvelope> get_shipping_methods_async(tenant_id, opts)

Get all shipping methods

Retrieves all shipping methods for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingMethodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all shipping methods
  result = api_instance.get_shipping_methods_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingMethodsApi->get_shipping_methods_async: #{e}"
end
```

#### Using the get_shipping_methods_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShippingMethodDtoListEnvelope>, Integer, Hash)> get_shipping_methods_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all shipping methods
  data, status_code, headers = api_instance.get_shipping_methods_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShippingMethodDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingMethodsApi->get_shipping_methods_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShippingMethodDtoListEnvelope**](ShippingMethodDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shipping_methods_count_async

> <Int32Envelope> get_shipping_methods_count_async(tenant_id, opts)

Get shipping methods count

Returns the count of shipping methods.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingMethodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get shipping methods count
  result = api_instance.get_shipping_methods_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingMethodsApi->get_shipping_methods_count_async: #{e}"
end
```

#### Using the get_shipping_methods_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_shipping_methods_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get shipping methods count
  data, status_code, headers = api_instance.get_shipping_methods_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingMethodsApi->get_shipping_methods_count_async_with_http_info: #{e}"
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


## patch_shipping_method_async

> <EmptyEnvelope> patch_shipping_method_async(tenant_id, method_id, opts)

Patch a shipping method

Partially updates an existing shipping method using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingMethodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
method_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a shipping method
  result = api_instance.patch_shipping_method_async(tenant_id, method_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingMethodsApi->patch_shipping_method_async: #{e}"
end
```

#### Using the patch_shipping_method_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_shipping_method_async_with_http_info(tenant_id, method_id, opts)

```ruby
begin
  # Patch a shipping method
  data, status_code, headers = api_instance.patch_shipping_method_async_with_http_info(tenant_id, method_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingMethodsApi->patch_shipping_method_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **method_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_shipping_method_async

> update_shipping_method_async(tenant_id, method_id, opts)

Update a shipping method

Updates an existing shipping method.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingMethodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
method_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipping_method_update_dto: OpenapiClient::ShippingMethodUpdateDto.new # ShippingMethodUpdateDto | 
}

begin
  # Update a shipping method
  api_instance.update_shipping_method_async(tenant_id, method_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingMethodsApi->update_shipping_method_async: #{e}"
end
```

#### Using the update_shipping_method_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_shipping_method_async_with_http_info(tenant_id, method_id, opts)

```ruby
begin
  # Update a shipping method
  data, status_code, headers = api_instance.update_shipping_method_async_with_http_info(tenant_id, method_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingMethodsApi->update_shipping_method_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **method_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipping_method_update_dto** | [**ShippingMethodUpdateDto**](ShippingMethodUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

