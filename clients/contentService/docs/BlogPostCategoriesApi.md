# OpenapiClient::BlogPostCategoriesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_blog_post_categories_async**](BlogPostCategoriesApi.md#count_blog_post_categories_async) | **GET** /api/v2/ContentService/BlogPostCategories/Count | Count blog post categories |
| [**create_blog_post_category_async**](BlogPostCategoriesApi.md#create_blog_post_category_async) | **POST** /api/v2/ContentService/BlogPostCategories | Create a blog post category |
| [**delete_blog_post_category_async**](BlogPostCategoriesApi.md#delete_blog_post_category_async) | **DELETE** /api/v2/ContentService/BlogPostCategories/{blogPostCategoryId} | Delete a blog post category |
| [**get_blog_post_categories_async**](BlogPostCategoriesApi.md#get_blog_post_categories_async) | **GET** /api/v2/ContentService/BlogPostCategories | Get blog post categories |
| [**get_blog_post_category_by_id_async**](BlogPostCategoriesApi.md#get_blog_post_category_by_id_async) | **GET** /api/v2/ContentService/BlogPostCategories/{blogPostCategoryId} | Get blog post category by ID |
| [**update_blog_post_category_async**](BlogPostCategoriesApi.md#update_blog_post_category_async) | **PUT** /api/v2/ContentService/BlogPostCategories/{blogPostCategoryId} | Update a blog post category |


## count_blog_post_categories_async

> <Int32Envelope> count_blog_post_categories_async(tenant_id, opts)

Count blog post categories

Counts all blog post categories for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count blog post categories
  result = api_instance.count_blog_post_categories_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostCategoriesApi->count_blog_post_categories_async: #{e}"
end
```

#### Using the count_blog_post_categories_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_blog_post_categories_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count blog post categories
  data, status_code, headers = api_instance.count_blog_post_categories_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostCategoriesApi->count_blog_post_categories_async_with_http_info: #{e}"
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


## create_blog_post_category_async

> <EmptyEnvelope> create_blog_post_category_async(tenant_id, opts)

Create a blog post category

Creates a new blog post category for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  blog_post_category_create_dto: OpenapiClient::BlogPostCategoryCreateDto.new # BlogPostCategoryCreateDto | 
}

begin
  # Create a blog post category
  result = api_instance.create_blog_post_category_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostCategoriesApi->create_blog_post_category_async: #{e}"
end
```

#### Using the create_blog_post_category_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_blog_post_category_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a blog post category
  data, status_code, headers = api_instance.create_blog_post_category_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostCategoriesApi->create_blog_post_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **blog_post_category_create_dto** | [**BlogPostCategoryCreateDto**](BlogPostCategoryCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_blog_post_category_async

> <EmptyEnvelope> delete_blog_post_category_async(tenant_id, blog_post_category_id, opts)

Delete a blog post category

Deletes a blog post category for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blog_post_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a blog post category
  result = api_instance.delete_blog_post_category_async(tenant_id, blog_post_category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostCategoriesApi->delete_blog_post_category_async: #{e}"
end
```

#### Using the delete_blog_post_category_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_blog_post_category_async_with_http_info(tenant_id, blog_post_category_id, opts)

```ruby
begin
  # Delete a blog post category
  data, status_code, headers = api_instance.delete_blog_post_category_async_with_http_info(tenant_id, blog_post_category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostCategoriesApi->delete_blog_post_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blog_post_category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_blog_post_categories_async

> <BlogPostCategoryDtoListEnvelope> get_blog_post_categories_async(tenant_id, opts)

Get blog post categories

Retrieves all blog post categories for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get blog post categories
  result = api_instance.get_blog_post_categories_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostCategoriesApi->get_blog_post_categories_async: #{e}"
end
```

#### Using the get_blog_post_categories_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BlogPostCategoryDtoListEnvelope>, Integer, Hash)> get_blog_post_categories_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get blog post categories
  data, status_code, headers = api_instance.get_blog_post_categories_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BlogPostCategoryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostCategoriesApi->get_blog_post_categories_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BlogPostCategoryDtoListEnvelope**](BlogPostCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_blog_post_category_by_id_async

> <BlogPostCategoryDtoEnvelope> get_blog_post_category_by_id_async(tenant_id, blog_post_category_id, opts)

Get blog post category by ID

Retrieves a specific blog post category by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blog_post_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get blog post category by ID
  result = api_instance.get_blog_post_category_by_id_async(tenant_id, blog_post_category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostCategoriesApi->get_blog_post_category_by_id_async: #{e}"
end
```

#### Using the get_blog_post_category_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BlogPostCategoryDtoEnvelope>, Integer, Hash)> get_blog_post_category_by_id_async_with_http_info(tenant_id, blog_post_category_id, opts)

```ruby
begin
  # Get blog post category by ID
  data, status_code, headers = api_instance.get_blog_post_category_by_id_async_with_http_info(tenant_id, blog_post_category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BlogPostCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostCategoriesApi->get_blog_post_category_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blog_post_category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BlogPostCategoryDtoEnvelope**](BlogPostCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_blog_post_category_async

> <EmptyEnvelope> update_blog_post_category_async(tenant_id, blog_post_category_id, opts)

Update a blog post category

Updates an existing blog post category for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blog_post_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  blog_post_category_update_dto: OpenapiClient::BlogPostCategoryUpdateDto.new # BlogPostCategoryUpdateDto | 
}

begin
  # Update a blog post category
  result = api_instance.update_blog_post_category_async(tenant_id, blog_post_category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostCategoriesApi->update_blog_post_category_async: #{e}"
end
```

#### Using the update_blog_post_category_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_blog_post_category_async_with_http_info(tenant_id, blog_post_category_id, opts)

```ruby
begin
  # Update a blog post category
  data, status_code, headers = api_instance.update_blog_post_category_async_with_http_info(tenant_id, blog_post_category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostCategoriesApi->update_blog_post_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blog_post_category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **blog_post_category_update_dto** | [**BlogPostCategoryUpdateDto**](BlogPostCategoryUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

