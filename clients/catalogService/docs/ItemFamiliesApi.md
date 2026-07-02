# OpenapiClient::ItemFamiliesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_item_family_async**](ItemFamiliesApi.md#create_item_family_async) | **POST** /api/v2/CatalogService/ItemFamilies | Create a new item family |
| [**delete_item_family_async**](ItemFamiliesApi.md#delete_item_family_async) | **DELETE** /api/v2/CatalogService/ItemFamilies/{itemFamilyId} | Delete an item family |
| [**get_item_families_async**](ItemFamiliesApi.md#get_item_families_async) | **GET** /api/v2/CatalogService/ItemFamilies | Get all item families |
| [**get_item_families_count_async**](ItemFamiliesApi.md#get_item_families_count_async) | **GET** /api/v2/CatalogService/ItemFamilies/Count | Get item families count |
| [**get_item_family_by_id_async**](ItemFamiliesApi.md#get_item_family_by_id_async) | **GET** /api/v2/CatalogService/ItemFamilies/{itemFamilyId} | Get item family by ID |
| [**patch_item_family_async**](ItemFamiliesApi.md#patch_item_family_async) | **PATCH** /api/v2/CatalogService/ItemFamilies/{itemFamilyId} | Patch an item family |
| [**update_item_family_async**](ItemFamiliesApi.md#update_item_family_async) | **PUT** /api/v2/CatalogService/ItemFamilies/{itemFamilyId} | Update an item family |


## create_item_family_async

> <ItemFamilyDtoEnvelope> create_item_family_async(tenant_id, opts)

Create a new item family

Creates a new item family for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemFamiliesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_family_create_dto: OpenapiClient::ItemFamilyCreateDto.new({name: 'name_example'}) # ItemFamilyCreateDto | 
}

begin
  # Create a new item family
  result = api_instance.create_item_family_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemFamiliesApi->create_item_family_async: #{e}"
end
```

#### Using the create_item_family_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemFamilyDtoEnvelope>, Integer, Hash)> create_item_family_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new item family
  data, status_code, headers = api_instance.create_item_family_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemFamilyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemFamiliesApi->create_item_family_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_family_create_dto** | [**ItemFamilyCreateDto**](ItemFamilyCreateDto.md) |  | [optional] |

### Return type

[**ItemFamilyDtoEnvelope**](ItemFamilyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_item_family_async

> delete_item_family_async(tenant_id, item_family_id, opts)

Delete an item family

Deletes an item family for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemFamiliesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_family_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an item family
  api_instance.delete_item_family_async(tenant_id, item_family_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemFamiliesApi->delete_item_family_async: #{e}"
end
```

#### Using the delete_item_family_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_item_family_async_with_http_info(tenant_id, item_family_id, opts)

```ruby
begin
  # Delete an item family
  data, status_code, headers = api_instance.delete_item_family_async_with_http_info(tenant_id, item_family_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemFamiliesApi->delete_item_family_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_family_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_families_async

> <ItemFamilyDtoListEnvelope> get_item_families_async(opts)

Get all item families

Retrieves all item families for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemFamiliesApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all item families
  result = api_instance.get_item_families_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemFamiliesApi->get_item_families_async: #{e}"
end
```

#### Using the get_item_families_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemFamilyDtoListEnvelope>, Integer, Hash)> get_item_families_async_with_http_info(opts)

```ruby
begin
  # Get all item families
  data, status_code, headers = api_instance.get_item_families_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemFamilyDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemFamiliesApi->get_item_families_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemFamilyDtoListEnvelope**](ItemFamilyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_families_count_async

> <Int32Envelope> get_item_families_count_async(opts)

Get item families count

Returns the count of item families for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemFamiliesApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item families count
  result = api_instance.get_item_families_count_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemFamiliesApi->get_item_families_count_async: #{e}"
end
```

#### Using the get_item_families_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_item_families_count_async_with_http_info(opts)

```ruby
begin
  # Get item families count
  data, status_code, headers = api_instance.get_item_families_count_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemFamiliesApi->get_item_families_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_family_by_id_async

> <ItemFamilyDtoEnvelope> get_item_family_by_id_async(item_family_id, opts)

Get item family by ID

Retrieves a specific item family by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemFamiliesApi.new
item_family_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item family by ID
  result = api_instance.get_item_family_by_id_async(item_family_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemFamiliesApi->get_item_family_by_id_async: #{e}"
end
```

#### Using the get_item_family_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemFamilyDtoEnvelope>, Integer, Hash)> get_item_family_by_id_async_with_http_info(item_family_id, opts)

```ruby
begin
  # Get item family by ID
  data, status_code, headers = api_instance.get_item_family_by_id_async_with_http_info(item_family_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemFamilyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemFamiliesApi->get_item_family_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_family_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemFamilyDtoEnvelope**](ItemFamilyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_item_family_async

> <EmptyEnvelope> patch_item_family_async(tenant_id, item_family_id, opts)

Patch an item family

Partially updates an existing item family for the specified tenant using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemFamiliesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_family_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch an item family
  result = api_instance.patch_item_family_async(tenant_id, item_family_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemFamiliesApi->patch_item_family_async: #{e}"
end
```

#### Using the patch_item_family_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_item_family_async_with_http_info(tenant_id, item_family_id, opts)

```ruby
begin
  # Patch an item family
  data, status_code, headers = api_instance.patch_item_family_async_with_http_info(tenant_id, item_family_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemFamiliesApi->patch_item_family_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_family_id** | **String** |  |  |
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


## update_item_family_async

> <ItemFamilyDtoEnvelope> update_item_family_async(tenant_id, item_family_id, opts)

Update an item family

Updates an existing item family for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemFamiliesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_family_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_family_update_dto: OpenapiClient::ItemFamilyUpdateDto.new({name: 'name_example'}) # ItemFamilyUpdateDto | 
}

begin
  # Update an item family
  result = api_instance.update_item_family_async(tenant_id, item_family_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemFamiliesApi->update_item_family_async: #{e}"
end
```

#### Using the update_item_family_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemFamilyDtoEnvelope>, Integer, Hash)> update_item_family_async_with_http_info(tenant_id, item_family_id, opts)

```ruby
begin
  # Update an item family
  data, status_code, headers = api_instance.update_item_family_async_with_http_info(tenant_id, item_family_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemFamilyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemFamiliesApi->update_item_family_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_family_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_family_update_dto** | [**ItemFamilyUpdateDto**](ItemFamilyUpdateDto.md) |  | [optional] |

### Return type

[**ItemFamilyDtoEnvelope**](ItemFamilyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

