# OpenapiClient::ShippingLabelsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_shipping_label_async**](ShippingLabelsApi.md#create_shipping_label_async) | **POST** /api/v2/ShipmentsService/ShippingLabels | Create a shipping label |
| [**delete_shipping_label_async**](ShippingLabelsApi.md#delete_shipping_label_async) | **DELETE** /api/v2/ShipmentsService/ShippingLabels/{labelId} | Delete a shipping label |
| [**get_shipping_label_by_id_async**](ShippingLabelsApi.md#get_shipping_label_by_id_async) | **GET** /api/v2/ShipmentsService/ShippingLabels/{labelId} | Get shipping label by ID |
| [**get_shipping_labels_async**](ShippingLabelsApi.md#get_shipping_labels_async) | **GET** /api/v2/ShipmentsService/ShippingLabels | Get all shipping labels |
| [**get_shipping_labels_count_async**](ShippingLabelsApi.md#get_shipping_labels_count_async) | **GET** /api/v2/ShipmentsService/ShippingLabels/Count | Get shipping labels count |
| [**patch_shipping_label_async**](ShippingLabelsApi.md#patch_shipping_label_async) | **PATCH** /api/v2/ShipmentsService/ShippingLabels/{labelId} | Patch a shipping label |
| [**update_shipping_label_async**](ShippingLabelsApi.md#update_shipping_label_async) | **PUT** /api/v2/ShipmentsService/ShippingLabels/{labelId} | Update a shipping label |


## create_shipping_label_async

> create_shipping_label_async(tenant_id, opts)

Create a shipping label

Creates a new shipping label.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingLabelsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipping_label_create_dto: OpenapiClient::ShippingLabelCreateDto.new({tracking_code: 'tracking_code_example'}) # ShippingLabelCreateDto | 
}

begin
  # Create a shipping label
  api_instance.create_shipping_label_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingLabelsApi->create_shipping_label_async: #{e}"
end
```

#### Using the create_shipping_label_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_shipping_label_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a shipping label
  data, status_code, headers = api_instance.create_shipping_label_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingLabelsApi->create_shipping_label_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipping_label_create_dto** | [**ShippingLabelCreateDto**](ShippingLabelCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_shipping_label_async

> delete_shipping_label_async(tenant_id, label_id, opts)

Delete a shipping label

Deletes a shipping label.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingLabelsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
label_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a shipping label
  api_instance.delete_shipping_label_async(tenant_id, label_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingLabelsApi->delete_shipping_label_async: #{e}"
end
```

#### Using the delete_shipping_label_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_shipping_label_async_with_http_info(tenant_id, label_id, opts)

```ruby
begin
  # Delete a shipping label
  data, status_code, headers = api_instance.delete_shipping_label_async_with_http_info(tenant_id, label_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingLabelsApi->delete_shipping_label_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **label_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shipping_label_by_id_async

> <ShippingLabelDtoEnvelope> get_shipping_label_by_id_async(tenant_id, label_id, opts)

Get shipping label by ID

Retrieves a specific shipping label.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingLabelsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
label_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get shipping label by ID
  result = api_instance.get_shipping_label_by_id_async(tenant_id, label_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingLabelsApi->get_shipping_label_by_id_async: #{e}"
end
```

#### Using the get_shipping_label_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShippingLabelDtoEnvelope>, Integer, Hash)> get_shipping_label_by_id_async_with_http_info(tenant_id, label_id, opts)

```ruby
begin
  # Get shipping label by ID
  data, status_code, headers = api_instance.get_shipping_label_by_id_async_with_http_info(tenant_id, label_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShippingLabelDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingLabelsApi->get_shipping_label_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **label_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShippingLabelDtoEnvelope**](ShippingLabelDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shipping_labels_async

> <ShippingLabelDtoListEnvelope> get_shipping_labels_async(tenant_id, opts)

Get all shipping labels

Retrieves all shipping labels for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingLabelsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipping_label_dto_collection_query_parameters: OpenapiClient::ShippingLabelDtoCollectionQueryParameters.new # ShippingLabelDtoCollectionQueryParameters | 
}

begin
  # Get all shipping labels
  result = api_instance.get_shipping_labels_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingLabelsApi->get_shipping_labels_async: #{e}"
end
```

#### Using the get_shipping_labels_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShippingLabelDtoListEnvelope>, Integer, Hash)> get_shipping_labels_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all shipping labels
  data, status_code, headers = api_instance.get_shipping_labels_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShippingLabelDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingLabelsApi->get_shipping_labels_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipping_label_dto_collection_query_parameters** | [**ShippingLabelDtoCollectionQueryParameters**](ShippingLabelDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ShippingLabelDtoListEnvelope**](ShippingLabelDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_shipping_labels_count_async

> <Int32Envelope> get_shipping_labels_count_async(tenant_id, opts)

Get shipping labels count

Returns the count of shipping labels.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingLabelsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipping_label_dto_collection_query_parameters: OpenapiClient::ShippingLabelDtoCollectionQueryParameters.new # ShippingLabelDtoCollectionQueryParameters | 
}

begin
  # Get shipping labels count
  result = api_instance.get_shipping_labels_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingLabelsApi->get_shipping_labels_count_async: #{e}"
end
```

#### Using the get_shipping_labels_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_shipping_labels_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get shipping labels count
  data, status_code, headers = api_instance.get_shipping_labels_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingLabelsApi->get_shipping_labels_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipping_label_dto_collection_query_parameters** | [**ShippingLabelDtoCollectionQueryParameters**](ShippingLabelDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_shipping_label_async

> <EmptyEnvelope> patch_shipping_label_async(tenant_id, label_id, opts)

Patch a shipping label

Partially updates an existing shipping label using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingLabelsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
label_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a shipping label
  result = api_instance.patch_shipping_label_async(tenant_id, label_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingLabelsApi->patch_shipping_label_async: #{e}"
end
```

#### Using the patch_shipping_label_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_shipping_label_async_with_http_info(tenant_id, label_id, opts)

```ruby
begin
  # Patch a shipping label
  data, status_code, headers = api_instance.patch_shipping_label_async_with_http_info(tenant_id, label_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingLabelsApi->patch_shipping_label_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **label_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_shipping_label_async

> update_shipping_label_async(tenant_id, label_id, opts)

Update a shipping label

Updates an existing shipping label.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShippingLabelsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
label_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipping_label_update_dto: OpenapiClient::ShippingLabelUpdateDto.new # ShippingLabelUpdateDto | 
}

begin
  # Update a shipping label
  api_instance.update_shipping_label_async(tenant_id, label_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingLabelsApi->update_shipping_label_async: #{e}"
end
```

#### Using the update_shipping_label_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_shipping_label_async_with_http_info(tenant_id, label_id, opts)

```ruby
begin
  # Update a shipping label
  data, status_code, headers = api_instance.update_shipping_label_async_with_http_info(tenant_id, label_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShippingLabelsApi->update_shipping_label_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **label_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipping_label_update_dto** | [**ShippingLabelUpdateDto**](ShippingLabelUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

