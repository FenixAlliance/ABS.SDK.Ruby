# OpenapiClient::CourseWikisApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_wiki_async**](CourseWikisApi.md#create_course_wiki_async) | **POST** /api/v2/LearningService/CourseWikis | Create a new course wiki |
| [**delete_course_wiki_async**](CourseWikisApi.md#delete_course_wiki_async) | **DELETE** /api/v2/LearningService/CourseWikis/{wikiId} | Delete a course wiki |
| [**get_course_wiki_by_id_async**](CourseWikisApi.md#get_course_wiki_by_id_async) | **GET** /api/v2/LearningService/CourseWikis/{wikiId} | Get course wiki by ID |
| [**get_course_wikis_async**](CourseWikisApi.md#get_course_wikis_async) | **GET** /api/v2/LearningService/CourseWikis | Get all course wikis |
| [**get_course_wikis_count_async**](CourseWikisApi.md#get_course_wikis_count_async) | **GET** /api/v2/LearningService/CourseWikis/Count | Get course wikis count |
| [**patch_course_wiki_async**](CourseWikisApi.md#patch_course_wiki_async) | **PATCH** /api/v2/LearningService/CourseWikis/{wikiId} | Patch a course wiki |
| [**update_course_wiki_async**](CourseWikisApi.md#update_course_wiki_async) | **PUT** /api/v2/LearningService/CourseWikis/{wikiId} | Update a course wiki |


## create_course_wiki_async

> create_course_wiki_async(tenant_id, opts)

Create a new course wiki

Creates a new course wiki for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseWikisApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_wiki_create_dto: OpenapiClient::CourseWikiCreateDto.new({title: 'title_example', course_id: 'course_id_example'}) # CourseWikiCreateDto | 
}

begin
  # Create a new course wiki
  api_instance.create_course_wiki_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseWikisApi->create_course_wiki_async: #{e}"
end
```

#### Using the create_course_wiki_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_course_wiki_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new course wiki
  data, status_code, headers = api_instance.create_course_wiki_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseWikisApi->create_course_wiki_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_wiki_create_dto** | [**CourseWikiCreateDto**](CourseWikiCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_wiki_async

> delete_course_wiki_async(tenant_id, wiki_id, opts)

Delete a course wiki

Deletes a course wiki for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseWikisApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
wiki_id = 'wiki_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course wiki
  api_instance.delete_course_wiki_async(tenant_id, wiki_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseWikisApi->delete_course_wiki_async: #{e}"
end
```

#### Using the delete_course_wiki_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_wiki_async_with_http_info(tenant_id, wiki_id, opts)

```ruby
begin
  # Delete a course wiki
  data, status_code, headers = api_instance.delete_course_wiki_async_with_http_info(tenant_id, wiki_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseWikisApi->delete_course_wiki_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **wiki_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_wiki_by_id_async

> <CourseWikiDto> get_course_wiki_by_id_async(wiki_id, opts)

Get course wiki by ID

Retrieves a specific course wiki by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseWikisApi.new
wiki_id = 'wiki_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course wiki by ID
  result = api_instance.get_course_wiki_by_id_async(wiki_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseWikisApi->get_course_wiki_by_id_async: #{e}"
end
```

#### Using the get_course_wiki_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseWikiDto>, Integer, Hash)> get_course_wiki_by_id_async_with_http_info(wiki_id, opts)

```ruby
begin
  # Get course wiki by ID
  data, status_code, headers = api_instance.get_course_wiki_by_id_async_with_http_info(wiki_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseWikiDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseWikisApi->get_course_wiki_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wiki_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseWikiDto**](CourseWikiDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_wikis_async

> <Array<CourseWikiDto>> get_course_wikis_async(tenant_id, opts)

Get all course wikis

Retrieves all course wikis for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseWikisApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_wiki_dto_collection_query_parameters: OpenapiClient::CourseWikiDtoCollectionQueryParameters.new # CourseWikiDtoCollectionQueryParameters | 
}

begin
  # Get all course wikis
  result = api_instance.get_course_wikis_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseWikisApi->get_course_wikis_async: #{e}"
end
```

#### Using the get_course_wikis_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseWikiDto>>, Integer, Hash)> get_course_wikis_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course wikis
  data, status_code, headers = api_instance.get_course_wikis_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseWikiDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseWikisApi->get_course_wikis_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_wiki_dto_collection_query_parameters** | [**CourseWikiDtoCollectionQueryParameters**](CourseWikiDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Array&lt;CourseWikiDto&gt;**](CourseWikiDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_course_wikis_count_async

> Integer get_course_wikis_count_async(tenant_id, opts)

Get course wikis count

Returns the count of course wikis for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseWikisApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_wiki_dto_collection_query_parameters: OpenapiClient::CourseWikiDtoCollectionQueryParameters.new # CourseWikiDtoCollectionQueryParameters | 
}

begin
  # Get course wikis count
  result = api_instance.get_course_wikis_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseWikisApi->get_course_wikis_count_async: #{e}"
end
```

#### Using the get_course_wikis_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_wikis_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course wikis count
  data, status_code, headers = api_instance.get_course_wikis_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseWikisApi->get_course_wikis_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_wiki_dto_collection_query_parameters** | [**CourseWikiDtoCollectionQueryParameters**](CourseWikiDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

**Integer**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_course_wiki_async

> <EmptyEnvelope> patch_course_wiki_async(tenant_id, wiki_id, opts)

Patch a course wiki

Partially updates a course wiki for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseWikisApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
wiki_id = 'wiki_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a course wiki
  result = api_instance.patch_course_wiki_async(tenant_id, wiki_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseWikisApi->patch_course_wiki_async: #{e}"
end
```

#### Using the patch_course_wiki_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_course_wiki_async_with_http_info(tenant_id, wiki_id, opts)

```ruby
begin
  # Patch a course wiki
  data, status_code, headers = api_instance.patch_course_wiki_async_with_http_info(tenant_id, wiki_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseWikisApi->patch_course_wiki_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **wiki_id** | **String** |  |  |
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


## update_course_wiki_async

> update_course_wiki_async(tenant_id, wiki_id, opts)

Update a course wiki

Updates an existing course wiki for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseWikisApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
wiki_id = 'wiki_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_wiki_update_dto: OpenapiClient::CourseWikiUpdateDto.new # CourseWikiUpdateDto | 
}

begin
  # Update a course wiki
  api_instance.update_course_wiki_async(tenant_id, wiki_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseWikisApi->update_course_wiki_async: #{e}"
end
```

#### Using the update_course_wiki_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_course_wiki_async_with_http_info(tenant_id, wiki_id, opts)

```ruby
begin
  # Update a course wiki
  data, status_code, headers = api_instance.update_course_wiki_async_with_http_info(tenant_id, wiki_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseWikisApi->update_course_wiki_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **wiki_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_wiki_update_dto** | [**CourseWikiUpdateDto**](CourseWikiUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

