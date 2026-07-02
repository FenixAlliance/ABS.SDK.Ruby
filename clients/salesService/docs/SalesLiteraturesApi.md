# OpenapiClient::SalesLiteraturesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_sales_literatures_async**](SalesLiteraturesApi.md#count_sales_literatures_async) | **GET** /api/v2/SalesService/SalesLiteratures/Count | Get sales literatures count |
| [**create_sales_literature_async**](SalesLiteraturesApi.md#create_sales_literature_async) | **POST** /api/v2/SalesService/SalesLiteratures | Create a sales literature |
| [**delete_sales_literature_async**](SalesLiteraturesApi.md#delete_sales_literature_async) | **DELETE** /api/v2/SalesService/SalesLiteratures/{salesLiteratureId} | Delete a sales literature |
| [**get_extended_sales_literatures_async**](SalesLiteraturesApi.md#get_extended_sales_literatures_async) | **GET** /api/v2/SalesService/SalesLiteratures/Extended | Get extended sales literatures |
| [**get_sales_literature_async**](SalesLiteraturesApi.md#get_sales_literature_async) | **GET** /api/v2/SalesService/SalesLiteratures/{salesLiteratureId} | Get sales literature by ID |
| [**get_sales_literatures_async**](SalesLiteraturesApi.md#get_sales_literatures_async) | **GET** /api/v2/SalesService/SalesLiteratures | Get sales literatures |
| [**patch_sales_literature_async**](SalesLiteraturesApi.md#patch_sales_literature_async) | **PATCH** /api/v2/SalesService/SalesLiteratures/{salesLiteratureId} | Patch a sales literature |
| [**update_sales_literature_async**](SalesLiteraturesApi.md#update_sales_literature_async) | **PUT** /api/v2/SalesService/SalesLiteratures/{salesLiteratureId} | Update a sales literature |


## count_sales_literatures_async

> <Int32Envelope> count_sales_literatures_async(tenant_id)

Get sales literatures count

Returns the total count of sales literatures for the specified tenant with OData filter support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SalesLiteraturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get sales literatures count
  result = api_instance.count_sales_literatures_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalesLiteraturesApi->count_sales_literatures_async: #{e}"
end
```

#### Using the count_sales_literatures_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_sales_literatures_async_with_http_info(tenant_id)

```ruby
begin
  # Get sales literatures count
  data, status_code, headers = api_instance.count_sales_literatures_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalesLiteraturesApi->count_sales_literatures_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_sales_literature_async

> <EmptyEnvelope> create_sales_literature_async(tenant_id, opts)

Create a sales literature

Creates a new sales literature for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SalesLiteraturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  sales_literature_create_dto: OpenapiClient::SalesLiteratureCreateDto.new # SalesLiteratureCreateDto | 
}

begin
  # Create a sales literature
  result = api_instance.create_sales_literature_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalesLiteraturesApi->create_sales_literature_async: #{e}"
end
```

#### Using the create_sales_literature_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_sales_literature_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a sales literature
  data, status_code, headers = api_instance.create_sales_literature_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalesLiteraturesApi->create_sales_literature_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **sales_literature_create_dto** | [**SalesLiteratureCreateDto**](SalesLiteratureCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_sales_literature_async

> <EmptyEnvelope> delete_sales_literature_async(tenant_id, sales_literature_id)

Delete a sales literature

Deletes an existing sales literature by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SalesLiteraturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
sales_literature_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete a sales literature
  result = api_instance.delete_sales_literature_async(tenant_id, sales_literature_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalesLiteraturesApi->delete_sales_literature_async: #{e}"
end
```

#### Using the delete_sales_literature_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_sales_literature_async_with_http_info(tenant_id, sales_literature_id)

```ruby
begin
  # Delete a sales literature
  data, status_code, headers = api_instance.delete_sales_literature_async_with_http_info(tenant_id, sales_literature_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalesLiteraturesApi->delete_sales_literature_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **sales_literature_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_extended_sales_literatures_async

> <ExtendedSalesLiteratureDtoListEnvelope> get_extended_sales_literatures_async(tenant_id)

Get extended sales literatures

Retrieves a list of sales literatures with extended details for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SalesLiteraturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get extended sales literatures
  result = api_instance.get_extended_sales_literatures_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalesLiteraturesApi->get_extended_sales_literatures_async: #{e}"
end
```

#### Using the get_extended_sales_literatures_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExtendedSalesLiteratureDtoListEnvelope>, Integer, Hash)> get_extended_sales_literatures_async_with_http_info(tenant_id)

```ruby
begin
  # Get extended sales literatures
  data, status_code, headers = api_instance.get_extended_sales_literatures_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExtendedSalesLiteratureDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalesLiteraturesApi->get_extended_sales_literatures_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**ExtendedSalesLiteratureDtoListEnvelope**](ExtendedSalesLiteratureDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_sales_literature_async

> <SalesLiteratureDtoEnvelope> get_sales_literature_async(tenant_id, sales_literature_id)

Get sales literature by ID

Retrieves a single sales literature by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SalesLiteraturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
sales_literature_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get sales literature by ID
  result = api_instance.get_sales_literature_async(tenant_id, sales_literature_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalesLiteraturesApi->get_sales_literature_async: #{e}"
end
```

#### Using the get_sales_literature_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SalesLiteratureDtoEnvelope>, Integer, Hash)> get_sales_literature_async_with_http_info(tenant_id, sales_literature_id)

```ruby
begin
  # Get sales literature by ID
  data, status_code, headers = api_instance.get_sales_literature_async_with_http_info(tenant_id, sales_literature_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SalesLiteratureDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalesLiteraturesApi->get_sales_literature_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **sales_literature_id** | **String** |  |  |

### Return type

[**SalesLiteratureDtoEnvelope**](SalesLiteratureDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_sales_literatures_async

> <SalesLiteratureDtoListEnvelope> get_sales_literatures_async(tenant_id)

Get sales literatures

Retrieves a list of sales literatures for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SalesLiteraturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get sales literatures
  result = api_instance.get_sales_literatures_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalesLiteraturesApi->get_sales_literatures_async: #{e}"
end
```

#### Using the get_sales_literatures_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SalesLiteratureDtoListEnvelope>, Integer, Hash)> get_sales_literatures_async_with_http_info(tenant_id)

```ruby
begin
  # Get sales literatures
  data, status_code, headers = api_instance.get_sales_literatures_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SalesLiteratureDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalesLiteraturesApi->get_sales_literatures_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**SalesLiteratureDtoListEnvelope**](SalesLiteratureDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_sales_literature_async

> <EmptyEnvelope> patch_sales_literature_async(tenant_id, sales_literature_id, opts)

Patch a sales literature

Partially updates an existing sales literature using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SalesLiteraturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
sales_literature_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a sales literature
  result = api_instance.patch_sales_literature_async(tenant_id, sales_literature_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalesLiteraturesApi->patch_sales_literature_async: #{e}"
end
```

#### Using the patch_sales_literature_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_sales_literature_async_with_http_info(tenant_id, sales_literature_id, opts)

```ruby
begin
  # Patch a sales literature
  data, status_code, headers = api_instance.patch_sales_literature_async_with_http_info(tenant_id, sales_literature_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalesLiteraturesApi->patch_sales_literature_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **sales_literature_id** | **String** |  |  |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_sales_literature_async

> <EmptyEnvelope> update_sales_literature_async(tenant_id, sales_literature_id, opts)

Update a sales literature

Updates an existing sales literature by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SalesLiteraturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
sales_literature_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  sales_literature_update_dto: OpenapiClient::SalesLiteratureUpdateDto.new # SalesLiteratureUpdateDto | 
}

begin
  # Update a sales literature
  result = api_instance.update_sales_literature_async(tenant_id, sales_literature_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalesLiteraturesApi->update_sales_literature_async: #{e}"
end
```

#### Using the update_sales_literature_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_sales_literature_async_with_http_info(tenant_id, sales_literature_id, opts)

```ruby
begin
  # Update a sales literature
  data, status_code, headers = api_instance.update_sales_literature_async_with_http_info(tenant_id, sales_literature_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalesLiteraturesApi->update_sales_literature_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **sales_literature_id** | **String** |  |  |
| **sales_literature_update_dto** | [**SalesLiteratureUpdateDto**](SalesLiteratureUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

