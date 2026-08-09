# OpenapiClient::WebPageCategoriesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_web_page_categories_async**](WebPageCategoriesApi.md#count_web_page_categories_async) | **GET** /api/v2/ContentService/WebPageCategories/Count | Count web page categories |
| [**create_web_page_category_async**](WebPageCategoriesApi.md#create_web_page_category_async) | **POST** /api/v2/ContentService/WebPageCategories | Create a web page category |
| [**delete_web_page_category_async**](WebPageCategoriesApi.md#delete_web_page_category_async) | **DELETE** /api/v2/ContentService/WebPageCategories/{webPageCategoryId} | Delete a web page category |
| [**get_web_page_categories_async**](WebPageCategoriesApi.md#get_web_page_categories_async) | **GET** /api/v2/ContentService/WebPageCategories | Get web page categories |
| [**get_web_page_category_by_id_async**](WebPageCategoriesApi.md#get_web_page_category_by_id_async) | **GET** /api/v2/ContentService/WebPageCategories/{webPageCategoryId} | Get web page category by ID |
| [**patch_web_page_category_async**](WebPageCategoriesApi.md#patch_web_page_category_async) | **PATCH** /api/v2/ContentService/WebPageCategories/{webPageCategoryId} | Patch a web page category |
| [**update_web_page_category_async**](WebPageCategoriesApi.md#update_web_page_category_async) | **PUT** /api/v2/ContentService/WebPageCategories/{webPageCategoryId} | Update a web page category |


## count_web_page_categories_async

> <Int32Envelope> count_web_page_categories_async(tenant_id, opts)

Count web page categories

Counts all web page categories for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPageCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_page_category_dto_collection_query_parameters: OpenapiClient::WebPageCategoryDtoCollectionQueryParameters.new # WebPageCategoryDtoCollectionQueryParameters | 
}

begin
  # Count web page categories
  result = api_instance.count_web_page_categories_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageCategoriesApi->count_web_page_categories_async: #{e}"
end
```

#### Using the count_web_page_categories_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_web_page_categories_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count web page categories
  data, status_code, headers = api_instance.count_web_page_categories_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageCategoriesApi->count_web_page_categories_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_page_category_dto_collection_query_parameters** | [**WebPageCategoryDtoCollectionQueryParameters**](WebPageCategoryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_web_page_category_async

> <EmptyEnvelope> create_web_page_category_async(tenant_id, opts)

Create a web page category

Creates a new web page category for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPageCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_page_category_create_dto: OpenapiClient::WebPageCategoryCreateDto.new # WebPageCategoryCreateDto | 
}

begin
  # Create a web page category
  result = api_instance.create_web_page_category_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageCategoriesApi->create_web_page_category_async: #{e}"
end
```

#### Using the create_web_page_category_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_web_page_category_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a web page category
  data, status_code, headers = api_instance.create_web_page_category_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageCategoriesApi->create_web_page_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_page_category_create_dto** | [**WebPageCategoryCreateDto**](WebPageCategoryCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_web_page_category_async

> <EmptyEnvelope> delete_web_page_category_async(tenant_id, web_page_category_id, opts)

Delete a web page category

Deletes a web page category for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPageCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_page_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a web page category
  result = api_instance.delete_web_page_category_async(tenant_id, web_page_category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageCategoriesApi->delete_web_page_category_async: #{e}"
end
```

#### Using the delete_web_page_category_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_web_page_category_async_with_http_info(tenant_id, web_page_category_id, opts)

```ruby
begin
  # Delete a web page category
  data, status_code, headers = api_instance.delete_web_page_category_async_with_http_info(tenant_id, web_page_category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageCategoriesApi->delete_web_page_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_page_category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_web_page_categories_async

> <WebPageCategoryDtoListEnvelope> get_web_page_categories_async(tenant_id, opts)

Get web page categories

Retrieves all web page categories for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPageCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_page_category_dto_collection_query_parameters: OpenapiClient::WebPageCategoryDtoCollectionQueryParameters.new # WebPageCategoryDtoCollectionQueryParameters | 
}

begin
  # Get web page categories
  result = api_instance.get_web_page_categories_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageCategoriesApi->get_web_page_categories_async: #{e}"
end
```

#### Using the get_web_page_categories_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebPageCategoryDtoListEnvelope>, Integer, Hash)> get_web_page_categories_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get web page categories
  data, status_code, headers = api_instance.get_web_page_categories_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebPageCategoryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageCategoriesApi->get_web_page_categories_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_page_category_dto_collection_query_parameters** | [**WebPageCategoryDtoCollectionQueryParameters**](WebPageCategoryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**WebPageCategoryDtoListEnvelope**](WebPageCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_web_page_category_by_id_async

> <WebPageCategoryDtoEnvelope> get_web_page_category_by_id_async(tenant_id, web_page_category_id, opts)

Get web page category by ID

Retrieves a specific web page category by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPageCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_page_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get web page category by ID
  result = api_instance.get_web_page_category_by_id_async(tenant_id, web_page_category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageCategoriesApi->get_web_page_category_by_id_async: #{e}"
end
```

#### Using the get_web_page_category_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebPageCategoryDtoEnvelope>, Integer, Hash)> get_web_page_category_by_id_async_with_http_info(tenant_id, web_page_category_id, opts)

```ruby
begin
  # Get web page category by ID
  data, status_code, headers = api_instance.get_web_page_category_by_id_async_with_http_info(tenant_id, web_page_category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebPageCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageCategoriesApi->get_web_page_category_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_page_category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebPageCategoryDtoEnvelope**](WebPageCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_web_page_category_async

> <EmptyEnvelope> patch_web_page_category_async(tenant_id, web_page_category_id, opts)

Patch a web page category

Partially updates an existing web page category for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPageCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_page_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a web page category
  result = api_instance.patch_web_page_category_async(tenant_id, web_page_category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageCategoriesApi->patch_web_page_category_async: #{e}"
end
```

#### Using the patch_web_page_category_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_web_page_category_async_with_http_info(tenant_id, web_page_category_id, opts)

```ruby
begin
  # Patch a web page category
  data, status_code, headers = api_instance.patch_web_page_category_async_with_http_info(tenant_id, web_page_category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageCategoriesApi->patch_web_page_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_page_category_id** | **String** |  |  |
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


## update_web_page_category_async

> <EmptyEnvelope> update_web_page_category_async(tenant_id, web_page_category_id, opts)

Update a web page category

Updates an existing web page category for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPageCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_page_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_page_category_update_dto: OpenapiClient::WebPageCategoryUpdateDto.new # WebPageCategoryUpdateDto | 
}

begin
  # Update a web page category
  result = api_instance.update_web_page_category_async(tenant_id, web_page_category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageCategoriesApi->update_web_page_category_async: #{e}"
end
```

#### Using the update_web_page_category_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_web_page_category_async_with_http_info(tenant_id, web_page_category_id, opts)

```ruby
begin
  # Update a web page category
  data, status_code, headers = api_instance.update_web_page_category_async_with_http_info(tenant_id, web_page_category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageCategoriesApi->update_web_page_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_page_category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_page_category_update_dto** | [**WebPageCategoryUpdateDto**](WebPageCategoryUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

