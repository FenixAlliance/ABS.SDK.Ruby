# OpenapiClient::BlogPostsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_blog_post_async**](BlogPostsApi.md#create_blog_post_async) | **POST** /api/v2/ContentService/BlogPosts | Create a new blog post |
| [**create_category_for_blog_post_async**](BlogPostsApi.md#create_category_for_blog_post_async) | **POST** /api/v2/ContentService/BlogPosts/{blogPostId}/Categories | Create a category for a blog post |
| [**create_comment_for_blog_post_async**](BlogPostsApi.md#create_comment_for_blog_post_async) | **POST** /api/v2/ContentService/BlogPosts/{blogPostId}/Comments | Create a comment for a blog post |
| [**create_tag_for_blog_post_async**](BlogPostsApi.md#create_tag_for_blog_post_async) | **POST** /api/v2/ContentService/BlogPosts/{blogPostId}/Tags | Create a tag for a blog post |
| [**delete_blog_post_async**](BlogPostsApi.md#delete_blog_post_async) | **DELETE** /api/v2/ContentService/BlogPosts/{blogPostId} | Delete a blog post |
| [**delete_comment_from_blog_post_async**](BlogPostsApi.md#delete_comment_from_blog_post_async) | **DELETE** /api/v2/ContentService/BlogPosts/{blogPostId}/Comments/{commentId} | Delete a blog post comment |
| [**get_blog_post_by_id_async**](BlogPostsApi.md#get_blog_post_by_id_async) | **GET** /api/v2/ContentService/BlogPosts/{blogPostId} | Get a blog post by ID |
| [**get_blog_posts_async**](BlogPostsApi.md#get_blog_posts_async) | **GET** /api/v2/ContentService/BlogPosts | Retrieve a list of blog posts |
| [**get_blog_posts_count_async**](BlogPostsApi.md#get_blog_posts_count_async) | **GET** /api/v2/ContentService/BlogPosts/Count | Get the count of blog posts |
| [**get_categories_for_blog_post_async**](BlogPostsApi.md#get_categories_for_blog_post_async) | **GET** /api/v2/ContentService/BlogPosts/{blogPostId}/Categories | Get categories for a blog post |
| [**get_comments_for_blog_post_async**](BlogPostsApi.md#get_comments_for_blog_post_async) | **GET** /api/v2/ContentService/BlogPosts/{blogPostId}/Comments | Get comments for a blog post |
| [**get_replies_for_comment_async**](BlogPostsApi.md#get_replies_for_comment_async) | **GET** /api/v2/ContentService/BlogPosts/{blogPostId}/Comments/{commentId}/Replies | Get replies for a comment |
| [**get_tags_for_blog_post_async**](BlogPostsApi.md#get_tags_for_blog_post_async) | **GET** /api/v2/ContentService/BlogPosts/{blogPostId}/Tags | Get tags for a blog post |
| [**relate_category_to_blog_post_async**](BlogPostsApi.md#relate_category_to_blog_post_async) | **POST** /api/v2/ContentService/BlogPosts/{blogPostId}/Categories/{categoryId} | Relate an existing category to a blog post |
| [**relate_tag_to_blog_post_async**](BlogPostsApi.md#relate_tag_to_blog_post_async) | **POST** /api/v2/ContentService/BlogPosts/{blogPostId}/Tags/{tagId} | Relate an existing tag to a blog post |
| [**reply_to_comment_async**](BlogPostsApi.md#reply_to_comment_async) | **POST** /api/v2/ContentService/BlogPosts/{blogPostId}/Comments/{commentId}/Reply | Reply to a blog post comment |
| [**unrelate_category_from_blog_post_async**](BlogPostsApi.md#unrelate_category_from_blog_post_async) | **DELETE** /api/v2/ContentService/BlogPosts/{blogPostId}/Categories/{categoryId} | Remove a category from a blog post |
| [**unrelate_tag_from_blog_post_async**](BlogPostsApi.md#unrelate_tag_from_blog_post_async) | **DELETE** /api/v2/ContentService/BlogPosts/{blogPostId}/Tags/{tagId} | Remove a tag from a blog post |
| [**update_blog_post_async**](BlogPostsApi.md#update_blog_post_async) | **PUT** /api/v2/ContentService/BlogPosts/{blogPostId} | Update a blog post |


## create_blog_post_async

> <EmptyEnvelope> create_blog_post_async(tenant_id, opts)

Create a new blog post

Creates a new blog post for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  blog_post_create_dto: OpenapiClient::BlogPostCreateDto.new({title: 'title_example'}) # BlogPostCreateDto | 
}

begin
  # Create a new blog post
  result = api_instance.create_blog_post_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->create_blog_post_async: #{e}"
end
```

#### Using the create_blog_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_blog_post_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new blog post
  data, status_code, headers = api_instance.create_blog_post_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->create_blog_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blog_post_create_dto** | [**BlogPostCreateDto**](BlogPostCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_category_for_blog_post_async

> <EmptyEnvelope> create_category_for_blog_post_async(tenant_id, blog_post_id, opts)

Create a category for a blog post

Creates a new category and relates it to a specific blog post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blog_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  blog_post_category_create_dto: OpenapiClient::BlogPostCategoryCreateDto.new # BlogPostCategoryCreateDto | 
}

begin
  # Create a category for a blog post
  result = api_instance.create_category_for_blog_post_async(tenant_id, blog_post_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->create_category_for_blog_post_async: #{e}"
end
```

#### Using the create_category_for_blog_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_category_for_blog_post_async_with_http_info(tenant_id, blog_post_id, opts)

```ruby
begin
  # Create a category for a blog post
  data, status_code, headers = api_instance.create_category_for_blog_post_async_with_http_info(tenant_id, blog_post_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->create_category_for_blog_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blog_post_id** | **String** |  |  |
| **blog_post_category_create_dto** | [**BlogPostCategoryCreateDto**](BlogPostCategoryCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_comment_for_blog_post_async

> <EmptyEnvelope> create_comment_for_blog_post_async(tenant_id, blog_post_id, opts)

Create a comment for a blog post

Creates a new comment on a specific blog post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blog_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  blog_post_comment_create_dto: OpenapiClient::BlogPostCommentCreateDto.new({message: 'message_example'}) # BlogPostCommentCreateDto | 
}

begin
  # Create a comment for a blog post
  result = api_instance.create_comment_for_blog_post_async(tenant_id, blog_post_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->create_comment_for_blog_post_async: #{e}"
end
```

#### Using the create_comment_for_blog_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_comment_for_blog_post_async_with_http_info(tenant_id, blog_post_id, opts)

```ruby
begin
  # Create a comment for a blog post
  data, status_code, headers = api_instance.create_comment_for_blog_post_async_with_http_info(tenant_id, blog_post_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->create_comment_for_blog_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blog_post_id** | **String** |  |  |
| **blog_post_comment_create_dto** | [**BlogPostCommentCreateDto**](BlogPostCommentCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_tag_for_blog_post_async

> <EmptyEnvelope> create_tag_for_blog_post_async(tenant_id, blog_post_id, opts)

Create a tag for a blog post

Creates a new tag and relates it to a specific blog post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blog_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  blog_post_tag_create_dto: OpenapiClient::BlogPostTagCreateDto.new # BlogPostTagCreateDto | 
}

begin
  # Create a tag for a blog post
  result = api_instance.create_tag_for_blog_post_async(tenant_id, blog_post_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->create_tag_for_blog_post_async: #{e}"
end
```

#### Using the create_tag_for_blog_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tag_for_blog_post_async_with_http_info(tenant_id, blog_post_id, opts)

```ruby
begin
  # Create a tag for a blog post
  data, status_code, headers = api_instance.create_tag_for_blog_post_async_with_http_info(tenant_id, blog_post_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->create_tag_for_blog_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blog_post_id** | **String** |  |  |
| **blog_post_tag_create_dto** | [**BlogPostTagCreateDto**](BlogPostTagCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_blog_post_async

> <EmptyEnvelope> delete_blog_post_async(tenant_id, blog_post_id)

Delete a blog post

Deletes a blog post for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blog_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete a blog post
  result = api_instance.delete_blog_post_async(tenant_id, blog_post_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->delete_blog_post_async: #{e}"
end
```

#### Using the delete_blog_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_blog_post_async_with_http_info(tenant_id, blog_post_id)

```ruby
begin
  # Delete a blog post
  data, status_code, headers = api_instance.delete_blog_post_async_with_http_info(tenant_id, blog_post_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->delete_blog_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blog_post_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_comment_from_blog_post_async

> <EmptyEnvelope> delete_comment_from_blog_post_async(tenant_id, blog_post_id, comment_id)

Delete a blog post comment

Deletes a comment from a specific blog post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blog_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
comment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete a blog post comment
  result = api_instance.delete_comment_from_blog_post_async(tenant_id, blog_post_id, comment_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->delete_comment_from_blog_post_async: #{e}"
end
```

#### Using the delete_comment_from_blog_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_comment_from_blog_post_async_with_http_info(tenant_id, blog_post_id, comment_id)

```ruby
begin
  # Delete a blog post comment
  data, status_code, headers = api_instance.delete_comment_from_blog_post_async_with_http_info(tenant_id, blog_post_id, comment_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->delete_comment_from_blog_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blog_post_id** | **String** |  |  |
| **comment_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_blog_post_by_id_async

> <BlogPostDtoEnvelope> get_blog_post_by_id_async(blog_post_id)

Get a blog post by ID

Retrieves a single blog post by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostsApi.new
blog_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get a blog post by ID
  result = api_instance.get_blog_post_by_id_async(blog_post_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->get_blog_post_by_id_async: #{e}"
end
```

#### Using the get_blog_post_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BlogPostDtoEnvelope>, Integer, Hash)> get_blog_post_by_id_async_with_http_info(blog_post_id)

```ruby
begin
  # Get a blog post by ID
  data, status_code, headers = api_instance.get_blog_post_by_id_async_with_http_info(blog_post_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BlogPostDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->get_blog_post_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **blog_post_id** | **String** |  |  |

### Return type

[**BlogPostDtoEnvelope**](BlogPostDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_blog_posts_async

> <BlogPostDtoListEnvelope> get_blog_posts_async(opts)

Retrieve a list of blog posts

Retrieves all blog posts, optionally filtered by tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostsApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
}

begin
  # Retrieve a list of blog posts
  result = api_instance.get_blog_posts_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->get_blog_posts_async: #{e}"
end
```

#### Using the get_blog_posts_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BlogPostDtoListEnvelope>, Integer, Hash)> get_blog_posts_async_with_http_info(opts)

```ruby
begin
  # Retrieve a list of blog posts
  data, status_code, headers = api_instance.get_blog_posts_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BlogPostDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->get_blog_posts_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |

### Return type

[**BlogPostDtoListEnvelope**](BlogPostDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_blog_posts_count_async

> <Int32Envelope> get_blog_posts_count_async(opts)

Get the count of blog posts

Returns the total count of blog posts, optionally filtered by tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostsApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
}

begin
  # Get the count of blog posts
  result = api_instance.get_blog_posts_count_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->get_blog_posts_count_async: #{e}"
end
```

#### Using the get_blog_posts_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_blog_posts_count_async_with_http_info(opts)

```ruby
begin
  # Get the count of blog posts
  data, status_code, headers = api_instance.get_blog_posts_count_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->get_blog_posts_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_categories_for_blog_post_async

> <BlogPostCategoryDtoListEnvelope> get_categories_for_blog_post_async(blog_post_id)

Get categories for a blog post

Retrieves all categories related to a specific blog post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostsApi.new
blog_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get categories for a blog post
  result = api_instance.get_categories_for_blog_post_async(blog_post_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->get_categories_for_blog_post_async: #{e}"
end
```

#### Using the get_categories_for_blog_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BlogPostCategoryDtoListEnvelope>, Integer, Hash)> get_categories_for_blog_post_async_with_http_info(blog_post_id)

```ruby
begin
  # Get categories for a blog post
  data, status_code, headers = api_instance.get_categories_for_blog_post_async_with_http_info(blog_post_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BlogPostCategoryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->get_categories_for_blog_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **blog_post_id** | **String** |  |  |

### Return type

[**BlogPostCategoryDtoListEnvelope**](BlogPostCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_comments_for_blog_post_async

> <BlogPostCommentDtoListEnvelope> get_comments_for_blog_post_async(blog_post_id)

Get comments for a blog post

Retrieves all comments for a specific blog post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostsApi.new
blog_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get comments for a blog post
  result = api_instance.get_comments_for_blog_post_async(blog_post_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->get_comments_for_blog_post_async: #{e}"
end
```

#### Using the get_comments_for_blog_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BlogPostCommentDtoListEnvelope>, Integer, Hash)> get_comments_for_blog_post_async_with_http_info(blog_post_id)

```ruby
begin
  # Get comments for a blog post
  data, status_code, headers = api_instance.get_comments_for_blog_post_async_with_http_info(blog_post_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BlogPostCommentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->get_comments_for_blog_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **blog_post_id** | **String** |  |  |

### Return type

[**BlogPostCommentDtoListEnvelope**](BlogPostCommentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_replies_for_comment_async

> <BlogPostCommentDtoListEnvelope> get_replies_for_comment_async(comment_id, blog_post_id)

Get replies for a comment

Retrieves all replies for a specific blog post comment.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostsApi.new
comment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blog_post_id = 'blog_post_id_example' # String | 

begin
  # Get replies for a comment
  result = api_instance.get_replies_for_comment_async(comment_id, blog_post_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->get_replies_for_comment_async: #{e}"
end
```

#### Using the get_replies_for_comment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BlogPostCommentDtoListEnvelope>, Integer, Hash)> get_replies_for_comment_async_with_http_info(comment_id, blog_post_id)

```ruby
begin
  # Get replies for a comment
  data, status_code, headers = api_instance.get_replies_for_comment_async_with_http_info(comment_id, blog_post_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BlogPostCommentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->get_replies_for_comment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **comment_id** | **String** |  |  |
| **blog_post_id** | **String** |  |  |

### Return type

[**BlogPostCommentDtoListEnvelope**](BlogPostCommentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tags_for_blog_post_async

> <BlogPostTagDtoListEnvelope> get_tags_for_blog_post_async(blog_post_id)

Get tags for a blog post

Retrieves all tags related to a specific blog post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostsApi.new
blog_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get tags for a blog post
  result = api_instance.get_tags_for_blog_post_async(blog_post_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->get_tags_for_blog_post_async: #{e}"
end
```

#### Using the get_tags_for_blog_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BlogPostTagDtoListEnvelope>, Integer, Hash)> get_tags_for_blog_post_async_with_http_info(blog_post_id)

```ruby
begin
  # Get tags for a blog post
  data, status_code, headers = api_instance.get_tags_for_blog_post_async_with_http_info(blog_post_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BlogPostTagDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->get_tags_for_blog_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **blog_post_id** | **String** |  |  |

### Return type

[**BlogPostTagDtoListEnvelope**](BlogPostTagDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_category_to_blog_post_async

> <EmptyEnvelope> relate_category_to_blog_post_async(tenant_id, blog_post_id, category_id)

Relate an existing category to a blog post

Creates a relationship between an existing category and a blog post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blog_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Relate an existing category to a blog post
  result = api_instance.relate_category_to_blog_post_async(tenant_id, blog_post_id, category_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->relate_category_to_blog_post_async: #{e}"
end
```

#### Using the relate_category_to_blog_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> relate_category_to_blog_post_async_with_http_info(tenant_id, blog_post_id, category_id)

```ruby
begin
  # Relate an existing category to a blog post
  data, status_code, headers = api_instance.relate_category_to_blog_post_async_with_http_info(tenant_id, blog_post_id, category_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->relate_category_to_blog_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blog_post_id** | **String** |  |  |
| **category_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_tag_to_blog_post_async

> <EmptyEnvelope> relate_tag_to_blog_post_async(tenant_id, blog_post_id, tag_id)

Relate an existing tag to a blog post

Creates a relationship between an existing tag and a blog post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blog_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tag_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Relate an existing tag to a blog post
  result = api_instance.relate_tag_to_blog_post_async(tenant_id, blog_post_id, tag_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->relate_tag_to_blog_post_async: #{e}"
end
```

#### Using the relate_tag_to_blog_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> relate_tag_to_blog_post_async_with_http_info(tenant_id, blog_post_id, tag_id)

```ruby
begin
  # Relate an existing tag to a blog post
  data, status_code, headers = api_instance.relate_tag_to_blog_post_async_with_http_info(tenant_id, blog_post_id, tag_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->relate_tag_to_blog_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blog_post_id** | **String** |  |  |
| **tag_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## reply_to_comment_async

> <EmptyEnvelope> reply_to_comment_async(tenant_id, blog_post_id, comment_id, opts)

Reply to a blog post comment

Creates a reply to an existing comment on a blog post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blog_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
comment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  blog_post_comment_create_dto: OpenapiClient::BlogPostCommentCreateDto.new({message: 'message_example'}) # BlogPostCommentCreateDto | 
}

begin
  # Reply to a blog post comment
  result = api_instance.reply_to_comment_async(tenant_id, blog_post_id, comment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->reply_to_comment_async: #{e}"
end
```

#### Using the reply_to_comment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> reply_to_comment_async_with_http_info(tenant_id, blog_post_id, comment_id, opts)

```ruby
begin
  # Reply to a blog post comment
  data, status_code, headers = api_instance.reply_to_comment_async_with_http_info(tenant_id, blog_post_id, comment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->reply_to_comment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blog_post_id** | **String** |  |  |
| **comment_id** | **String** |  |  |
| **blog_post_comment_create_dto** | [**BlogPostCommentCreateDto**](BlogPostCommentCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## unrelate_category_from_blog_post_async

> <EmptyEnvelope> unrelate_category_from_blog_post_async(tenant_id, blog_post_id, category_id)

Remove a category from a blog post

Removes the relationship between a category and a blog post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blog_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Remove a category from a blog post
  result = api_instance.unrelate_category_from_blog_post_async(tenant_id, blog_post_id, category_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->unrelate_category_from_blog_post_async: #{e}"
end
```

#### Using the unrelate_category_from_blog_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> unrelate_category_from_blog_post_async_with_http_info(tenant_id, blog_post_id, category_id)

```ruby
begin
  # Remove a category from a blog post
  data, status_code, headers = api_instance.unrelate_category_from_blog_post_async_with_http_info(tenant_id, blog_post_id, category_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->unrelate_category_from_blog_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blog_post_id** | **String** |  |  |
| **category_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## unrelate_tag_from_blog_post_async

> <EmptyEnvelope> unrelate_tag_from_blog_post_async(tenant_id, blog_post_id, tag_id)

Remove a tag from a blog post

Removes the relationship between a tag and a blog post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blog_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tag_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Remove a tag from a blog post
  result = api_instance.unrelate_tag_from_blog_post_async(tenant_id, blog_post_id, tag_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->unrelate_tag_from_blog_post_async: #{e}"
end
```

#### Using the unrelate_tag_from_blog_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> unrelate_tag_from_blog_post_async_with_http_info(tenant_id, blog_post_id, tag_id)

```ruby
begin
  # Remove a tag from a blog post
  data, status_code, headers = api_instance.unrelate_tag_from_blog_post_async_with_http_info(tenant_id, blog_post_id, tag_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->unrelate_tag_from_blog_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blog_post_id** | **String** |  |  |
| **tag_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_blog_post_async

> <EmptyEnvelope> update_blog_post_async(tenant_id, blog_post_id, opts)

Update a blog post

Updates an existing blog post for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blog_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  blog_post_update_dto: OpenapiClient::BlogPostUpdateDto.new # BlogPostUpdateDto | 
}

begin
  # Update a blog post
  result = api_instance.update_blog_post_async(tenant_id, blog_post_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->update_blog_post_async: #{e}"
end
```

#### Using the update_blog_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_blog_post_async_with_http_info(tenant_id, blog_post_id, opts)

```ruby
begin
  # Update a blog post
  data, status_code, headers = api_instance.update_blog_post_async_with_http_info(tenant_id, blog_post_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostsApi->update_blog_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blog_post_id** | **String** |  |  |
| **blog_post_update_dto** | [**BlogPostUpdateDto**](BlogPostUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

