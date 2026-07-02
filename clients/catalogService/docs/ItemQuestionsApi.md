# OpenapiClient::ItemQuestionsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_item_question_async**](ItemQuestionsApi.md#create_item_question_async) | **POST** /api/v2/CatalogService/ItemQuestions | Create a new item question |
| [**delete_item_question_async**](ItemQuestionsApi.md#delete_item_question_async) | **DELETE** /api/v2/CatalogService/ItemQuestions/{itemQuestionId} | Delete an item question |
| [**get_item_question_by_id_async**](ItemQuestionsApi.md#get_item_question_by_id_async) | **GET** /api/v2/CatalogService/ItemQuestions/{itemQuestionId} | Get item question by ID |
| [**get_item_questions_async**](ItemQuestionsApi.md#get_item_questions_async) | **GET** /api/v2/CatalogService/ItemQuestions | Get all item questions |
| [**patch_item_question_async**](ItemQuestionsApi.md#patch_item_question_async) | **PATCH** /api/v2/CatalogService/ItemQuestions/{itemQuestionId} | Patch an item question |
| [**update_item_question_async**](ItemQuestionsApi.md#update_item_question_async) | **PUT** /api/v2/CatalogService/ItemQuestions/{itemQuestionId} | Update an item question |


## create_item_question_async

> <ItemQuestionDtoEnvelope> create_item_question_async(tenant_id, opts)

Create a new item question

Creates a new item question for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemQuestionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_question_create_dto: OpenapiClient::ItemQuestionCreateDto.new({title: 'title_example', needs_revision: false, question: 'question_example', item_id: 'item_id_example'}) # ItemQuestionCreateDto | 
}

begin
  # Create a new item question
  result = api_instance.create_item_question_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemQuestionsApi->create_item_question_async: #{e}"
end
```

#### Using the create_item_question_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemQuestionDtoEnvelope>, Integer, Hash)> create_item_question_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new item question
  data, status_code, headers = api_instance.create_item_question_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemQuestionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemQuestionsApi->create_item_question_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_question_create_dto** | [**ItemQuestionCreateDto**](ItemQuestionCreateDto.md) |  | [optional] |

### Return type

[**ItemQuestionDtoEnvelope**](ItemQuestionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_item_question_async

> delete_item_question_async(tenant_id, item_question_id, opts)

Delete an item question

Deletes an item question for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemQuestionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_question_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an item question
  api_instance.delete_item_question_async(tenant_id, item_question_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemQuestionsApi->delete_item_question_async: #{e}"
end
```

#### Using the delete_item_question_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_item_question_async_with_http_info(tenant_id, item_question_id, opts)

```ruby
begin
  # Delete an item question
  data, status_code, headers = api_instance.delete_item_question_async_with_http_info(tenant_id, item_question_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemQuestionsApi->delete_item_question_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_question_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_question_by_id_async

> <ItemQuestionDtoEnvelope> get_item_question_by_id_async(item_question_id, opts)

Get item question by ID

Retrieves a specific item question by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemQuestionsApi.new
item_question_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item question by ID
  result = api_instance.get_item_question_by_id_async(item_question_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemQuestionsApi->get_item_question_by_id_async: #{e}"
end
```

#### Using the get_item_question_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemQuestionDtoEnvelope>, Integer, Hash)> get_item_question_by_id_async_with_http_info(item_question_id, opts)

```ruby
begin
  # Get item question by ID
  data, status_code, headers = api_instance.get_item_question_by_id_async_with_http_info(item_question_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemQuestionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemQuestionsApi->get_item_question_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_question_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemQuestionDtoEnvelope**](ItemQuestionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_questions_async

> <ItemQuestionDtoListEnvelope> get_item_questions_async(opts)

Get all item questions

Retrieves all item questions for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemQuestionsApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all item questions
  result = api_instance.get_item_questions_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemQuestionsApi->get_item_questions_async: #{e}"
end
```

#### Using the get_item_questions_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemQuestionDtoListEnvelope>, Integer, Hash)> get_item_questions_async_with_http_info(opts)

```ruby
begin
  # Get all item questions
  data, status_code, headers = api_instance.get_item_questions_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemQuestionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemQuestionsApi->get_item_questions_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemQuestionDtoListEnvelope**](ItemQuestionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_item_question_async

> patch_item_question_async(tenant_id, item_question_id, opts)

Patch an item question

Partially updates an existing item question for the specified tenant using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemQuestionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_question_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch an item question
  api_instance.patch_item_question_async(tenant_id, item_question_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemQuestionsApi->patch_item_question_async: #{e}"
end
```

#### Using the patch_item_question_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> patch_item_question_async_with_http_info(tenant_id, item_question_id, opts)

```ruby
begin
  # Patch an item question
  data, status_code, headers = api_instance.patch_item_question_async_with_http_info(tenant_id, item_question_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemQuestionsApi->patch_item_question_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_question_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_item_question_async

> update_item_question_async(tenant_id, item_question_id, opts)

Update an item question

Updates an existing item question for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemQuestionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_question_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_question_update_dto: OpenapiClient::ItemQuestionUpdateDto.new({needs_revision: false}) # ItemQuestionUpdateDto | 
}

begin
  # Update an item question
  api_instance.update_item_question_async(tenant_id, item_question_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemQuestionsApi->update_item_question_async: #{e}"
end
```

#### Using the update_item_question_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_item_question_async_with_http_info(tenant_id, item_question_id, opts)

```ruby
begin
  # Update an item question
  data, status_code, headers = api_instance.update_item_question_async_with_http_info(tenant_id, item_question_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemQuestionsApi->update_item_question_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_question_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_question_update_dto** | [**ItemQuestionUpdateDto**](ItemQuestionUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

