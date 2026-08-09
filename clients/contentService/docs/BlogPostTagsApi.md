# OpenapiClient::BlogPostTagsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_blog_post_tags_async**](BlogPostTagsApi.md#count_blog_post_tags_async) | **GET** /api/v2/ContentService/BlogPostTags/Count | Count blog post tags |
| [**create_blog_post_tag_async**](BlogPostTagsApi.md#create_blog_post_tag_async) | **POST** /api/v2/ContentService/BlogPostTags | Create a blog post tag |
| [**delete_blog_post_tag_async**](BlogPostTagsApi.md#delete_blog_post_tag_async) | **DELETE** /api/v2/ContentService/BlogPostTags/{blogPostTagId} | Delete a blog post tag |
| [**get_blog_post_tag_by_id_async**](BlogPostTagsApi.md#get_blog_post_tag_by_id_async) | **GET** /api/v2/ContentService/BlogPostTags/{blogPostTagId} | Get blog post tag by ID |
| [**get_blog_post_tags_async**](BlogPostTagsApi.md#get_blog_post_tags_async) | **GET** /api/v2/ContentService/BlogPostTags | Get blog post tags |
| [**patch_blog_post_tag_async**](BlogPostTagsApi.md#patch_blog_post_tag_async) | **PATCH** /api/v2/ContentService/BlogPostTags/{blogPostTagId} | Patch a blog post tag |
| [**update_blog_post_tag_async**](BlogPostTagsApi.md#update_blog_post_tag_async) | **PUT** /api/v2/ContentService/BlogPostTags/{blogPostTagId} | Update a blog post tag |


## count_blog_post_tags_async

> <Int32Envelope> count_blog_post_tags_async(tenant_id, opts)

Count blog post tags

Counts all blog post tags for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostTagsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  blog_post_tag_dto_collection_query_parameters: OpenapiClient::BlogPostTagDtoCollectionQueryParameters.new # BlogPostTagDtoCollectionQueryParameters | 
}

begin
  # Count blog post tags
  result = api_instance.count_blog_post_tags_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostTagsApi->count_blog_post_tags_async: #{e}"
end
```

#### Using the count_blog_post_tags_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_blog_post_tags_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count blog post tags
  data, status_code, headers = api_instance.count_blog_post_tags_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostTagsApi->count_blog_post_tags_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **blog_post_tag_dto_collection_query_parameters** | [**BlogPostTagDtoCollectionQueryParameters**](BlogPostTagDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_blog_post_tag_async

> <EmptyEnvelope> create_blog_post_tag_async(tenant_id, opts)

Create a blog post tag

Creates a new blog post tag for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostTagsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  blog_post_tag_create_dto: OpenapiClient::BlogPostTagCreateDto.new # BlogPostTagCreateDto | 
}

begin
  # Create a blog post tag
  result = api_instance.create_blog_post_tag_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostTagsApi->create_blog_post_tag_async: #{e}"
end
```

#### Using the create_blog_post_tag_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_blog_post_tag_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a blog post tag
  data, status_code, headers = api_instance.create_blog_post_tag_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostTagsApi->create_blog_post_tag_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **blog_post_tag_create_dto** | [**BlogPostTagCreateDto**](BlogPostTagCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_blog_post_tag_async

> <EmptyEnvelope> delete_blog_post_tag_async(tenant_id, blog_post_tag_id, opts)

Delete a blog post tag

Deletes a blog post tag for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostTagsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blog_post_tag_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a blog post tag
  result = api_instance.delete_blog_post_tag_async(tenant_id, blog_post_tag_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostTagsApi->delete_blog_post_tag_async: #{e}"
end
```

#### Using the delete_blog_post_tag_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_blog_post_tag_async_with_http_info(tenant_id, blog_post_tag_id, opts)

```ruby
begin
  # Delete a blog post tag
  data, status_code, headers = api_instance.delete_blog_post_tag_async_with_http_info(tenant_id, blog_post_tag_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostTagsApi->delete_blog_post_tag_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blog_post_tag_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_blog_post_tag_by_id_async

> <BlogPostTagDtoEnvelope> get_blog_post_tag_by_id_async(tenant_id, blog_post_tag_id, opts)

Get blog post tag by ID

Retrieves a specific blog post tag by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostTagsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blog_post_tag_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get blog post tag by ID
  result = api_instance.get_blog_post_tag_by_id_async(tenant_id, blog_post_tag_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostTagsApi->get_blog_post_tag_by_id_async: #{e}"
end
```

#### Using the get_blog_post_tag_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BlogPostTagDtoEnvelope>, Integer, Hash)> get_blog_post_tag_by_id_async_with_http_info(tenant_id, blog_post_tag_id, opts)

```ruby
begin
  # Get blog post tag by ID
  data, status_code, headers = api_instance.get_blog_post_tag_by_id_async_with_http_info(tenant_id, blog_post_tag_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BlogPostTagDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostTagsApi->get_blog_post_tag_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blog_post_tag_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BlogPostTagDtoEnvelope**](BlogPostTagDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_blog_post_tags_async

> <BlogPostTagDtoListEnvelope> get_blog_post_tags_async(tenant_id, opts)

Get blog post tags

Retrieves all blog post tags for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostTagsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  blog_post_tag_dto_collection_query_parameters: OpenapiClient::BlogPostTagDtoCollectionQueryParameters.new # BlogPostTagDtoCollectionQueryParameters | 
}

begin
  # Get blog post tags
  result = api_instance.get_blog_post_tags_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostTagsApi->get_blog_post_tags_async: #{e}"
end
```

#### Using the get_blog_post_tags_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BlogPostTagDtoListEnvelope>, Integer, Hash)> get_blog_post_tags_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get blog post tags
  data, status_code, headers = api_instance.get_blog_post_tags_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BlogPostTagDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostTagsApi->get_blog_post_tags_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **blog_post_tag_dto_collection_query_parameters** | [**BlogPostTagDtoCollectionQueryParameters**](BlogPostTagDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**BlogPostTagDtoListEnvelope**](BlogPostTagDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_blog_post_tag_async

> <EmptyEnvelope> patch_blog_post_tag_async(tenant_id, blog_post_tag_id, opts)

Patch a blog post tag

Partially updates an existing blog post tag for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostTagsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blog_post_tag_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a blog post tag
  result = api_instance.patch_blog_post_tag_async(tenant_id, blog_post_tag_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostTagsApi->patch_blog_post_tag_async: #{e}"
end
```

#### Using the patch_blog_post_tag_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_blog_post_tag_async_with_http_info(tenant_id, blog_post_tag_id, opts)

```ruby
begin
  # Patch a blog post tag
  data, status_code, headers = api_instance.patch_blog_post_tag_async_with_http_info(tenant_id, blog_post_tag_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostTagsApi->patch_blog_post_tag_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blog_post_tag_id** | **String** |  |  |
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


## update_blog_post_tag_async

> <EmptyEnvelope> update_blog_post_tag_async(tenant_id, blog_post_tag_id, opts)

Update a blog post tag

Updates an existing blog post tag for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostTagsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blog_post_tag_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  blog_post_tag_update_dto: OpenapiClient::BlogPostTagUpdateDto.new # BlogPostTagUpdateDto | 
}

begin
  # Update a blog post tag
  result = api_instance.update_blog_post_tag_async(tenant_id, blog_post_tag_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostTagsApi->update_blog_post_tag_async: #{e}"
end
```

#### Using the update_blog_post_tag_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_blog_post_tag_async_with_http_info(tenant_id, blog_post_tag_id, opts)

```ruby
begin
  # Update a blog post tag
  data, status_code, headers = api_instance.update_blog_post_tag_async_with_http_info(tenant_id, blog_post_tag_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostTagsApi->update_blog_post_tag_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blog_post_tag_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **blog_post_tag_update_dto** | [**BlogPostTagUpdateDto**](BlogPostTagUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

