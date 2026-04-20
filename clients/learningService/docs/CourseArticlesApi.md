# OpenapiClient::CourseArticlesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_article_async**](CourseArticlesApi.md#create_course_article_async) | **POST** /api/v2/LearningService/CourseArticles | Create a new course article |
| [**delete_course_article_async**](CourseArticlesApi.md#delete_course_article_async) | **DELETE** /api/v2/LearningService/CourseArticles/{articleId} | Delete a course article |
| [**get_course_article_by_id_async**](CourseArticlesApi.md#get_course_article_by_id_async) | **GET** /api/v2/LearningService/CourseArticles/{articleId} | Get course article by ID |
| [**get_course_articles_async**](CourseArticlesApi.md#get_course_articles_async) | **GET** /api/v2/LearningService/CourseArticles | Get all course articles |
| [**get_course_articles_count_async**](CourseArticlesApi.md#get_course_articles_count_async) | **GET** /api/v2/LearningService/CourseArticles/Count | Get course articles count |
| [**update_course_article_async**](CourseArticlesApi.md#update_course_article_async) | **PUT** /api/v2/LearningService/CourseArticles/{articleId} | Update a course article |


## create_course_article_async

> create_course_article_async(tenant_id, opts)

Create a new course article

Creates a new course article for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseArticlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_article_create_dto: OpenapiClient::CourseArticleCreateDto.new({title: 'title_example', course_id: 'course_id_example', course_wiki_id: 'course_wiki_id_example'}) # CourseArticleCreateDto | 
}

begin
  # Create a new course article
  api_instance.create_course_article_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseArticlesApi->create_course_article_async: #{e}"
end
```

#### Using the create_course_article_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_course_article_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new course article
  data, status_code, headers = api_instance.create_course_article_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseArticlesApi->create_course_article_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_article_create_dto** | [**CourseArticleCreateDto**](CourseArticleCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_article_async

> delete_course_article_async(tenant_id, article_id, opts)

Delete a course article

Deletes a course article for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseArticlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
article_id = 'article_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course article
  api_instance.delete_course_article_async(tenant_id, article_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseArticlesApi->delete_course_article_async: #{e}"
end
```

#### Using the delete_course_article_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_article_async_with_http_info(tenant_id, article_id, opts)

```ruby
begin
  # Delete a course article
  data, status_code, headers = api_instance.delete_course_article_async_with_http_info(tenant_id, article_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseArticlesApi->delete_course_article_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **article_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_article_by_id_async

> <CourseArticleDto> get_course_article_by_id_async(article_id, opts)

Get course article by ID

Retrieves a specific course article by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseArticlesApi.new
article_id = 'article_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course article by ID
  result = api_instance.get_course_article_by_id_async(article_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseArticlesApi->get_course_article_by_id_async: #{e}"
end
```

#### Using the get_course_article_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseArticleDto>, Integer, Hash)> get_course_article_by_id_async_with_http_info(article_id, opts)

```ruby
begin
  # Get course article by ID
  data, status_code, headers = api_instance.get_course_article_by_id_async_with_http_info(article_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseArticleDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseArticlesApi->get_course_article_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **article_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseArticleDto**](CourseArticleDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_articles_async

> <Array<CourseArticleDto>> get_course_articles_async(tenant_id, opts)

Get all course articles

Retrieves all course articles for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseArticlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all course articles
  result = api_instance.get_course_articles_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseArticlesApi->get_course_articles_async: #{e}"
end
```

#### Using the get_course_articles_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseArticleDto>>, Integer, Hash)> get_course_articles_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course articles
  data, status_code, headers = api_instance.get_course_articles_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseArticleDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseArticlesApi->get_course_articles_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseArticleDto&gt;**](CourseArticleDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_articles_count_async

> Integer get_course_articles_count_async(tenant_id, opts)

Get course articles count

Returns the count of course articles for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseArticlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course articles count
  result = api_instance.get_course_articles_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseArticlesApi->get_course_articles_count_async: #{e}"
end
```

#### Using the get_course_articles_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_articles_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course articles count
  data, status_code, headers = api_instance.get_course_articles_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseArticlesApi->get_course_articles_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

**Integer**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_course_article_async

> update_course_article_async(tenant_id, article_id, opts)

Update a course article

Updates an existing course article for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseArticlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
article_id = 'article_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_article_update_dto: OpenapiClient::CourseArticleUpdateDto.new # CourseArticleUpdateDto | 
}

begin
  # Update a course article
  api_instance.update_course_article_async(tenant_id, article_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseArticlesApi->update_course_article_async: #{e}"
end
```

#### Using the update_course_article_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_course_article_async_with_http_info(tenant_id, article_id, opts)

```ruby
begin
  # Update a course article
  data, status_code, headers = api_instance.update_course_article_async_with_http_info(tenant_id, article_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseArticlesApi->update_course_article_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **article_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_article_update_dto** | [**CourseArticleUpdateDto**](CourseArticleUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

