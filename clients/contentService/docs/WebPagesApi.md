# OpenapiClient::WebPagesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_web_pages_async**](WebPagesApi.md#count_web_pages_async) | **GET** /api/v2/ContentService/WebPages/Count | Count web pages |
| [**create_web_page_async**](WebPagesApi.md#create_web_page_async) | **POST** /api/v2/ContentService/WebPages | Create a web page |
| [**create_web_page_category_relation_async**](WebPagesApi.md#create_web_page_category_relation_async) | **POST** /api/v2/ContentService/WebPages/{webPageId}/Categories | Create a web page category relation |
| [**create_web_page_tag_relation_async**](WebPagesApi.md#create_web_page_tag_relation_async) | **POST** /api/v2/ContentService/WebPages/{webPageId}/Tags | Create a web page tag relation |
| [**delete_web_page_async**](WebPagesApi.md#delete_web_page_async) | **DELETE** /api/v2/ContentService/WebPages/{webPageId} | Delete a web page |
| [**get_categories_by_web_page_async**](WebPagesApi.md#get_categories_by_web_page_async) | **GET** /api/v2/ContentService/WebPages/{webPageId}/Categories | Get categories by web page |
| [**get_tags_by_web_page_async**](WebPagesApi.md#get_tags_by_web_page_async) | **GET** /api/v2/ContentService/WebPages/{webPageId}/Tags | Get tags by web page |
| [**get_web_page_by_id_async**](WebPagesApi.md#get_web_page_by_id_async) | **GET** /api/v2/ContentService/WebPages/{webPageId} | Get web page by ID |
| [**get_web_pages_async**](WebPagesApi.md#get_web_pages_async) | **GET** /api/v2/ContentService/WebPages | Get web pages |
| [**relate_web_page_to_category_async**](WebPagesApi.md#relate_web_page_to_category_async) | **POST** /api/v2/ContentService/WebPages/{webPageId}/Categories/{categoryId} | Relate web page to category |
| [**relate_web_page_to_tag_async**](WebPagesApi.md#relate_web_page_to_tag_async) | **POST** /api/v2/ContentService/WebPages/{webPageId}/Tags/{tagId} | Relate web page to tag |
| [**unrelate_web_page_category_async**](WebPagesApi.md#unrelate_web_page_category_async) | **DELETE** /api/v2/ContentService/WebPages/{webPageId}/Categories/{categoryId} | Unrelate web page from category |
| [**unrelate_web_page_tag_async**](WebPagesApi.md#unrelate_web_page_tag_async) | **DELETE** /api/v2/ContentService/WebPages/{webPageId}/Tags/{tagId} | Unrelate web page from tag |
| [**update_web_page_async**](WebPagesApi.md#update_web_page_async) | **PUT** /api/v2/ContentService/WebPages/{webPageId} | Update a web page |


## count_web_pages_async

> <Int32Envelope> count_web_pages_async(tenant_id, opts)

Count web pages

Counts all web pages for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count web pages
  result = api_instance.count_web_pages_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->count_web_pages_async: #{e}"
end
```

#### Using the count_web_pages_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_web_pages_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count web pages
  data, status_code, headers = api_instance.count_web_pages_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->count_web_pages_async_with_http_info: #{e}"
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


## create_web_page_async

> create_web_page_async(tenant_id, opts)

Create a web page

Creates a new web page for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_page_create_dto: OpenapiClient::WebPageCreateDto.new # WebPageCreateDto | 
}

begin
  # Create a web page
  api_instance.create_web_page_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->create_web_page_async: #{e}"
end
```

#### Using the create_web_page_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_web_page_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a web page
  data, status_code, headers = api_instance.create_web_page_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->create_web_page_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_page_create_dto** | [**WebPageCreateDto**](WebPageCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_web_page_category_relation_async

> create_web_page_category_relation_async(tenant_id, web_page_id, opts)

Create a web page category relation

Creates a new category and relates it to a web page.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_page_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_page_category_create_dto: OpenapiClient::WebPageCategoryCreateDto.new # WebPageCategoryCreateDto | 
}

begin
  # Create a web page category relation
  api_instance.create_web_page_category_relation_async(tenant_id, web_page_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->create_web_page_category_relation_async: #{e}"
end
```

#### Using the create_web_page_category_relation_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_web_page_category_relation_async_with_http_info(tenant_id, web_page_id, opts)

```ruby
begin
  # Create a web page category relation
  data, status_code, headers = api_instance.create_web_page_category_relation_async_with_http_info(tenant_id, web_page_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->create_web_page_category_relation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_page_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_page_category_create_dto** | [**WebPageCategoryCreateDto**](WebPageCategoryCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_web_page_tag_relation_async

> create_web_page_tag_relation_async(tenant_id, web_page_id, opts)

Create a web page tag relation

Creates a new tag and relates it to a web page.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_page_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_page_tag_create_dto: OpenapiClient::WebPageTagCreateDto.new # WebPageTagCreateDto | 
}

begin
  # Create a web page tag relation
  api_instance.create_web_page_tag_relation_async(tenant_id, web_page_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->create_web_page_tag_relation_async: #{e}"
end
```

#### Using the create_web_page_tag_relation_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_web_page_tag_relation_async_with_http_info(tenant_id, web_page_id, opts)

```ruby
begin
  # Create a web page tag relation
  data, status_code, headers = api_instance.create_web_page_tag_relation_async_with_http_info(tenant_id, web_page_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->create_web_page_tag_relation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_page_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_page_tag_create_dto** | [**WebPageTagCreateDto**](WebPageTagCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_web_page_async

> delete_web_page_async(tenant_id, web_page_id, opts)

Delete a web page

Deletes a web page for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_page_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a web page
  api_instance.delete_web_page_async(tenant_id, web_page_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->delete_web_page_async: #{e}"
end
```

#### Using the delete_web_page_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_web_page_async_with_http_info(tenant_id, web_page_id, opts)

```ruby
begin
  # Delete a web page
  data, status_code, headers = api_instance.delete_web_page_async_with_http_info(tenant_id, web_page_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->delete_web_page_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_page_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_categories_by_web_page_async

> <WebPageCategoryDtoListEnvelope> get_categories_by_web_page_async(web_page_id, opts)

Get categories by web page

Retrieves all categories related to a specific web page.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPagesApi.new
web_page_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get categories by web page
  result = api_instance.get_categories_by_web_page_async(web_page_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->get_categories_by_web_page_async: #{e}"
end
```

#### Using the get_categories_by_web_page_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebPageCategoryDtoListEnvelope>, Integer, Hash)> get_categories_by_web_page_async_with_http_info(web_page_id, opts)

```ruby
begin
  # Get categories by web page
  data, status_code, headers = api_instance.get_categories_by_web_page_async_with_http_info(web_page_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebPageCategoryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->get_categories_by_web_page_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **web_page_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebPageCategoryDtoListEnvelope**](WebPageCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tags_by_web_page_async

> <WebPageTagDtoListEnvelope> get_tags_by_web_page_async(web_page_id, opts)

Get tags by web page

Retrieves all tags related to a specific web page.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPagesApi.new
web_page_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get tags by web page
  result = api_instance.get_tags_by_web_page_async(web_page_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->get_tags_by_web_page_async: #{e}"
end
```

#### Using the get_tags_by_web_page_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebPageTagDtoListEnvelope>, Integer, Hash)> get_tags_by_web_page_async_with_http_info(web_page_id, opts)

```ruby
begin
  # Get tags by web page
  data, status_code, headers = api_instance.get_tags_by_web_page_async_with_http_info(web_page_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebPageTagDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->get_tags_by_web_page_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **web_page_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebPageTagDtoListEnvelope**](WebPageTagDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_web_page_by_id_async

> <WebPageDtoEnvelope> get_web_page_by_id_async(tenant_id, web_page_id, opts)

Get web page by ID

Retrieves a specific web page by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_page_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get web page by ID
  result = api_instance.get_web_page_by_id_async(tenant_id, web_page_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->get_web_page_by_id_async: #{e}"
end
```

#### Using the get_web_page_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebPageDtoEnvelope>, Integer, Hash)> get_web_page_by_id_async_with_http_info(tenant_id, web_page_id, opts)

```ruby
begin
  # Get web page by ID
  data, status_code, headers = api_instance.get_web_page_by_id_async_with_http_info(tenant_id, web_page_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebPageDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->get_web_page_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_page_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebPageDtoEnvelope**](WebPageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_web_pages_async

> <WebPageDtoListEnvelope> get_web_pages_async(tenant_id, opts)

Get web pages

Retrieves all web pages for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get web pages
  result = api_instance.get_web_pages_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->get_web_pages_async: #{e}"
end
```

#### Using the get_web_pages_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebPageDtoListEnvelope>, Integer, Hash)> get_web_pages_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get web pages
  data, status_code, headers = api_instance.get_web_pages_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebPageDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->get_web_pages_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebPageDtoListEnvelope**](WebPageDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_web_page_to_category_async

> relate_web_page_to_category_async(tenant_id, web_page_id, category_id, opts)

Relate web page to category

Relates an existing category to a web page.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_page_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate web page to category
  api_instance.relate_web_page_to_category_async(tenant_id, web_page_id, category_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->relate_web_page_to_category_async: #{e}"
end
```

#### Using the relate_web_page_to_category_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> relate_web_page_to_category_async_with_http_info(tenant_id, web_page_id, category_id, opts)

```ruby
begin
  # Relate web page to category
  data, status_code, headers = api_instance.relate_web_page_to_category_async_with_http_info(tenant_id, web_page_id, category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->relate_web_page_to_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_page_id** | **String** |  |  |
| **category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_web_page_to_tag_async

> relate_web_page_to_tag_async(tenant_id, web_page_id, tag_id, opts)

Relate web page to tag

Relates an existing tag to a web page.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_page_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tag_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate web page to tag
  api_instance.relate_web_page_to_tag_async(tenant_id, web_page_id, tag_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->relate_web_page_to_tag_async: #{e}"
end
```

#### Using the relate_web_page_to_tag_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> relate_web_page_to_tag_async_with_http_info(tenant_id, web_page_id, tag_id, opts)

```ruby
begin
  # Relate web page to tag
  data, status_code, headers = api_instance.relate_web_page_to_tag_async_with_http_info(tenant_id, web_page_id, tag_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->relate_web_page_to_tag_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_page_id** | **String** |  |  |
| **tag_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## unrelate_web_page_category_async

> unrelate_web_page_category_async(tenant_id, web_page_id, category_id, opts)

Unrelate web page from category

Removes the relationship between a web page and a category.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_page_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Unrelate web page from category
  api_instance.unrelate_web_page_category_async(tenant_id, web_page_id, category_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->unrelate_web_page_category_async: #{e}"
end
```

#### Using the unrelate_web_page_category_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> unrelate_web_page_category_async_with_http_info(tenant_id, web_page_id, category_id, opts)

```ruby
begin
  # Unrelate web page from category
  data, status_code, headers = api_instance.unrelate_web_page_category_async_with_http_info(tenant_id, web_page_id, category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->unrelate_web_page_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_page_id** | **String** |  |  |
| **category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## unrelate_web_page_tag_async

> unrelate_web_page_tag_async(tenant_id, web_page_id, tag_id, opts)

Unrelate web page from tag

Removes the relationship between a web page and a tag.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_page_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tag_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Unrelate web page from tag
  api_instance.unrelate_web_page_tag_async(tenant_id, web_page_id, tag_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->unrelate_web_page_tag_async: #{e}"
end
```

#### Using the unrelate_web_page_tag_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> unrelate_web_page_tag_async_with_http_info(tenant_id, web_page_id, tag_id, opts)

```ruby
begin
  # Unrelate web page from tag
  data, status_code, headers = api_instance.unrelate_web_page_tag_async_with_http_info(tenant_id, web_page_id, tag_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->unrelate_web_page_tag_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_page_id** | **String** |  |  |
| **tag_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_web_page_async

> update_web_page_async(tenant_id, web_page_id, opts)

Update a web page

Updates an existing web page for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_page_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_page_update_dto: OpenapiClient::WebPageUpdateDto.new # WebPageUpdateDto | 
}

begin
  # Update a web page
  api_instance.update_web_page_async(tenant_id, web_page_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->update_web_page_async: #{e}"
end
```

#### Using the update_web_page_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_web_page_async_with_http_info(tenant_id, web_page_id, opts)

```ruby
begin
  # Update a web page
  data, status_code, headers = api_instance.update_web_page_async_with_http_info(tenant_id, web_page_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPagesApi->update_web_page_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_page_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_page_update_dto** | [**WebPageUpdateDto**](WebPageUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

