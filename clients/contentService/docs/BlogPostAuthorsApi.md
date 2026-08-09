# OpenapiClient::BlogPostAuthorsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_blog_posts_by_author_async**](BlogPostAuthorsApi.md#count_blog_posts_by_author_async) | **GET** /api/v2/ContentService/BlogPostAuthors/{authorId}/BlogPosts/Count | Count blog posts by author |
| [**get_blog_author_by_id_async**](BlogPostAuthorsApi.md#get_blog_author_by_id_async) | **GET** /api/v2/ContentService/BlogPostAuthors/{authorId} | Get blog author by ID |
| [**get_blog_authors_async**](BlogPostAuthorsApi.md#get_blog_authors_async) | **GET** /api/v2/ContentService/BlogPostAuthors | Get blog authors |
| [**get_blog_posts_by_author_async**](BlogPostAuthorsApi.md#get_blog_posts_by_author_async) | **GET** /api/v2/ContentService/BlogPostAuthors/{authorId}/BlogPosts | Get blog posts by author |


## count_blog_posts_by_author_async

> <Int32Envelope> count_blog_posts_by_author_async(author_id, opts)

Count blog posts by author

Returns the count of blog posts written by a specific author.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostAuthorsApi.new
author_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  blog_post_dto_collection_query_parameters: OpenapiClient::BlogPostDtoCollectionQueryParameters.new # BlogPostDtoCollectionQueryParameters | 
}

begin
  # Count blog posts by author
  result = api_instance.count_blog_posts_by_author_async(author_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostAuthorsApi->count_blog_posts_by_author_async: #{e}"
end
```

#### Using the count_blog_posts_by_author_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_blog_posts_by_author_async_with_http_info(author_id, opts)

```ruby
begin
  # Count blog posts by author
  data, status_code, headers = api_instance.count_blog_posts_by_author_async_with_http_info(author_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostAuthorsApi->count_blog_posts_by_author_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **author_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **blog_post_dto_collection_query_parameters** | [**BlogPostDtoCollectionQueryParameters**](BlogPostDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_blog_author_by_id_async

> <BlogAuthorDtoEnvelope> get_blog_author_by_id_async(author_id, opts)

Get blog author by ID

Retrieves a specific blog author by their identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostAuthorsApi.new
author_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get blog author by ID
  result = api_instance.get_blog_author_by_id_async(author_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostAuthorsApi->get_blog_author_by_id_async: #{e}"
end
```

#### Using the get_blog_author_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BlogAuthorDtoEnvelope>, Integer, Hash)> get_blog_author_by_id_async_with_http_info(author_id, opts)

```ruby
begin
  # Get blog author by ID
  data, status_code, headers = api_instance.get_blog_author_by_id_async_with_http_info(author_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BlogAuthorDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostAuthorsApi->get_blog_author_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **author_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BlogAuthorDtoEnvelope**](BlogAuthorDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_blog_authors_async

> <BlogAuthorDtoListEnvelope> get_blog_authors_async(opts)

Get blog authors

Retrieves all blog authors, optionally filtered by tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostAuthorsApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  blog_author_dto_collection_query_parameters: OpenapiClient::BlogAuthorDtoCollectionQueryParameters.new # BlogAuthorDtoCollectionQueryParameters | 
}

begin
  # Get blog authors
  result = api_instance.get_blog_authors_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostAuthorsApi->get_blog_authors_async: #{e}"
end
```

#### Using the get_blog_authors_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BlogAuthorDtoListEnvelope>, Integer, Hash)> get_blog_authors_async_with_http_info(opts)

```ruby
begin
  # Get blog authors
  data, status_code, headers = api_instance.get_blog_authors_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BlogAuthorDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostAuthorsApi->get_blog_authors_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **blog_author_dto_collection_query_parameters** | [**BlogAuthorDtoCollectionQueryParameters**](BlogAuthorDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**BlogAuthorDtoListEnvelope**](BlogAuthorDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_blog_posts_by_author_async

> <BlogPostDtoListEnvelope> get_blog_posts_by_author_async(author_id, opts)

Get blog posts by author

Retrieves all blog posts written by a specific author.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlogPostAuthorsApi.new
author_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  blog_post_dto_collection_query_parameters: OpenapiClient::BlogPostDtoCollectionQueryParameters.new # BlogPostDtoCollectionQueryParameters | 
}

begin
  # Get blog posts by author
  result = api_instance.get_blog_posts_by_author_async(author_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostAuthorsApi->get_blog_posts_by_author_async: #{e}"
end
```

#### Using the get_blog_posts_by_author_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BlogPostDtoListEnvelope>, Integer, Hash)> get_blog_posts_by_author_async_with_http_info(author_id, opts)

```ruby
begin
  # Get blog posts by author
  data, status_code, headers = api_instance.get_blog_posts_by_author_async_with_http_info(author_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BlogPostDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlogPostAuthorsApi->get_blog_posts_by_author_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **author_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **blog_post_dto_collection_query_parameters** | [**BlogPostDtoCollectionQueryParameters**](BlogPostDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**BlogPostDtoListEnvelope**](BlogPostDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

