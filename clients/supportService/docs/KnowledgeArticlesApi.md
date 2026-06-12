# OpenapiClient::KnowledgeArticlesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_knowledge_article_async**](KnowledgeArticlesApi.md#create_knowledge_article_async) | **POST** /api/v2/SupportService/KnowledgeArticles | Create a knowledge article |
| [**delete_knowledge_article_async**](KnowledgeArticlesApi.md#delete_knowledge_article_async) | **DELETE** /api/v2/SupportService/KnowledgeArticles/{knowledgeArticleId} | Delete a knowledge article |
| [**get_knowledge_article_async**](KnowledgeArticlesApi.md#get_knowledge_article_async) | **GET** /api/v2/SupportService/KnowledgeArticles/{knowledgeArticleId} | Retrieve a knowledge article by ID |
| [**get_knowledge_articles_async**](KnowledgeArticlesApi.md#get_knowledge_articles_async) | **GET** /api/v2/SupportService/KnowledgeArticles | Retrieve knowledge articles |
| [**get_knowledge_articles_count_async**](KnowledgeArticlesApi.md#get_knowledge_articles_count_async) | **GET** /api/v2/SupportService/KnowledgeArticles/Count | Get knowledge articles count |
| [**patch_knowledge_article_async**](KnowledgeArticlesApi.md#patch_knowledge_article_async) | **PATCH** /api/v2/SupportService/KnowledgeArticles/{knowledgeArticleId} | Patch a knowledge article |
| [**update_knowledge_article_async**](KnowledgeArticlesApi.md#update_knowledge_article_async) | **PUT** /api/v2/SupportService/KnowledgeArticles/{knowledgeArticleId} | Update a knowledge article |


## create_knowledge_article_async

> <EmptyEnvelope> create_knowledge_article_async(tenant_id, opts)

Create a knowledge article

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::KnowledgeArticlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  knowledge_article_create_dto: OpenapiClient::KnowledgeArticleCreateDto.new({title: 'title_example'}) # KnowledgeArticleCreateDto | 
}

begin
  # Create a knowledge article
  result = api_instance.create_knowledge_article_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling KnowledgeArticlesApi->create_knowledge_article_async: #{e}"
end
```

#### Using the create_knowledge_article_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_knowledge_article_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a knowledge article
  data, status_code, headers = api_instance.create_knowledge_article_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling KnowledgeArticlesApi->create_knowledge_article_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **knowledge_article_create_dto** | [**KnowledgeArticleCreateDto**](KnowledgeArticleCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_knowledge_article_async

> <EmptyEnvelope> delete_knowledge_article_async(tenant_id, knowledge_article_id, opts)

Delete a knowledge article

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::KnowledgeArticlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
knowledge_article_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a knowledge article
  result = api_instance.delete_knowledge_article_async(tenant_id, knowledge_article_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling KnowledgeArticlesApi->delete_knowledge_article_async: #{e}"
end
```

#### Using the delete_knowledge_article_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_knowledge_article_async_with_http_info(tenant_id, knowledge_article_id, opts)

```ruby
begin
  # Delete a knowledge article
  data, status_code, headers = api_instance.delete_knowledge_article_async_with_http_info(tenant_id, knowledge_article_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling KnowledgeArticlesApi->delete_knowledge_article_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **knowledge_article_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_knowledge_article_async

> <KnowledgeArticleDtoEnvelope> get_knowledge_article_async(tenant_id, knowledge_article_id, opts)

Retrieve a knowledge article by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::KnowledgeArticlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
knowledge_article_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a knowledge article by ID
  result = api_instance.get_knowledge_article_async(tenant_id, knowledge_article_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling KnowledgeArticlesApi->get_knowledge_article_async: #{e}"
end
```

#### Using the get_knowledge_article_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<KnowledgeArticleDtoEnvelope>, Integer, Hash)> get_knowledge_article_async_with_http_info(tenant_id, knowledge_article_id, opts)

```ruby
begin
  # Retrieve a knowledge article by ID
  data, status_code, headers = api_instance.get_knowledge_article_async_with_http_info(tenant_id, knowledge_article_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <KnowledgeArticleDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling KnowledgeArticlesApi->get_knowledge_article_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **knowledge_article_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**KnowledgeArticleDtoEnvelope**](KnowledgeArticleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_knowledge_articles_async

> <KnowledgeArticleDtoListEnvelope> get_knowledge_articles_async(tenant_id, opts)

Retrieve knowledge articles

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::KnowledgeArticlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve knowledge articles
  result = api_instance.get_knowledge_articles_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling KnowledgeArticlesApi->get_knowledge_articles_async: #{e}"
end
```

#### Using the get_knowledge_articles_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<KnowledgeArticleDtoListEnvelope>, Integer, Hash)> get_knowledge_articles_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve knowledge articles
  data, status_code, headers = api_instance.get_knowledge_articles_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <KnowledgeArticleDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling KnowledgeArticlesApi->get_knowledge_articles_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**KnowledgeArticleDtoListEnvelope**](KnowledgeArticleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_knowledge_articles_count_async

> <Int32Envelope> get_knowledge_articles_count_async(tenant_id, opts)

Get knowledge articles count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::KnowledgeArticlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get knowledge articles count
  result = api_instance.get_knowledge_articles_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling KnowledgeArticlesApi->get_knowledge_articles_count_async: #{e}"
end
```

#### Using the get_knowledge_articles_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_knowledge_articles_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get knowledge articles count
  data, status_code, headers = api_instance.get_knowledge_articles_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling KnowledgeArticlesApi->get_knowledge_articles_count_async_with_http_info: #{e}"
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


## patch_knowledge_article_async

> <EmptyEnvelope> patch_knowledge_article_async(tenant_id, knowledge_article_id, opts)

Patch a knowledge article

Partially updates an existing knowledge article by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::KnowledgeArticlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
knowledge_article_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a knowledge article
  result = api_instance.patch_knowledge_article_async(tenant_id, knowledge_article_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling KnowledgeArticlesApi->patch_knowledge_article_async: #{e}"
end
```

#### Using the patch_knowledge_article_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_knowledge_article_async_with_http_info(tenant_id, knowledge_article_id, opts)

```ruby
begin
  # Patch a knowledge article
  data, status_code, headers = api_instance.patch_knowledge_article_async_with_http_info(tenant_id, knowledge_article_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling KnowledgeArticlesApi->patch_knowledge_article_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **knowledge_article_id** | **String** |  |  |
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


## update_knowledge_article_async

> <EmptyEnvelope> update_knowledge_article_async(tenant_id, knowledge_article_id, opts)

Update a knowledge article

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::KnowledgeArticlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
knowledge_article_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  knowledge_article_update_dto: OpenapiClient::KnowledgeArticleUpdateDto.new # KnowledgeArticleUpdateDto | 
}

begin
  # Update a knowledge article
  result = api_instance.update_knowledge_article_async(tenant_id, knowledge_article_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling KnowledgeArticlesApi->update_knowledge_article_async: #{e}"
end
```

#### Using the update_knowledge_article_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_knowledge_article_async_with_http_info(tenant_id, knowledge_article_id, opts)

```ruby
begin
  # Update a knowledge article
  data, status_code, headers = api_instance.update_knowledge_article_async_with_http_info(tenant_id, knowledge_article_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling KnowledgeArticlesApi->update_knowledge_article_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **knowledge_article_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **knowledge_article_update_dto** | [**KnowledgeArticleUpdateDto**](KnowledgeArticleUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

