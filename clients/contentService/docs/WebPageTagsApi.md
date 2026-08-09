# OpenapiClient::WebPageTagsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_web_page_tags_async**](WebPageTagsApi.md#count_web_page_tags_async) | **GET** /api/v2/ContentService/WebPageTags/Count | Count web page tags |
| [**create_web_page_tag_async**](WebPageTagsApi.md#create_web_page_tag_async) | **POST** /api/v2/ContentService/WebPageTags | Create a web page tag |
| [**delete_web_page_tag_async**](WebPageTagsApi.md#delete_web_page_tag_async) | **DELETE** /api/v2/ContentService/WebPageTags/{webPageTagId} | Delete a web page tag |
| [**get_web_page_tag_by_id_async**](WebPageTagsApi.md#get_web_page_tag_by_id_async) | **GET** /api/v2/ContentService/WebPageTags/{webPageTagId} | Get web page tag by ID |
| [**get_web_page_tags_async**](WebPageTagsApi.md#get_web_page_tags_async) | **GET** /api/v2/ContentService/WebPageTags | Get web page tags |
| [**patch_web_page_tag_async**](WebPageTagsApi.md#patch_web_page_tag_async) | **PATCH** /api/v2/ContentService/WebPageTags/{webPageTagId} | Patch a web page tag |
| [**update_web_page_tag_async**](WebPageTagsApi.md#update_web_page_tag_async) | **PUT** /api/v2/ContentService/WebPageTags/{webPageTagId} | Update a web page tag |


## count_web_page_tags_async

> <Int32Envelope> count_web_page_tags_async(tenant_id, opts)

Count web page tags

Counts all web page tags for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPageTagsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_page_tag_dto_collection_query_parameters: OpenapiClient::WebPageTagDtoCollectionQueryParameters.new # WebPageTagDtoCollectionQueryParameters | 
}

begin
  # Count web page tags
  result = api_instance.count_web_page_tags_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageTagsApi->count_web_page_tags_async: #{e}"
end
```

#### Using the count_web_page_tags_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_web_page_tags_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count web page tags
  data, status_code, headers = api_instance.count_web_page_tags_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageTagsApi->count_web_page_tags_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_page_tag_dto_collection_query_parameters** | [**WebPageTagDtoCollectionQueryParameters**](WebPageTagDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_web_page_tag_async

> <EmptyEnvelope> create_web_page_tag_async(tenant_id, opts)

Create a web page tag

Creates a new web page tag for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPageTagsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_page_tag_create_dto: OpenapiClient::WebPageTagCreateDto.new # WebPageTagCreateDto | 
}

begin
  # Create a web page tag
  result = api_instance.create_web_page_tag_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageTagsApi->create_web_page_tag_async: #{e}"
end
```

#### Using the create_web_page_tag_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_web_page_tag_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a web page tag
  data, status_code, headers = api_instance.create_web_page_tag_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageTagsApi->create_web_page_tag_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_page_tag_create_dto** | [**WebPageTagCreateDto**](WebPageTagCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_web_page_tag_async

> <EmptyEnvelope> delete_web_page_tag_async(tenant_id, web_page_tag_id, opts)

Delete a web page tag

Deletes a web page tag for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPageTagsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_page_tag_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a web page tag
  result = api_instance.delete_web_page_tag_async(tenant_id, web_page_tag_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageTagsApi->delete_web_page_tag_async: #{e}"
end
```

#### Using the delete_web_page_tag_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_web_page_tag_async_with_http_info(tenant_id, web_page_tag_id, opts)

```ruby
begin
  # Delete a web page tag
  data, status_code, headers = api_instance.delete_web_page_tag_async_with_http_info(tenant_id, web_page_tag_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageTagsApi->delete_web_page_tag_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_page_tag_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_web_page_tag_by_id_async

> <WebPageTagDtoEnvelope> get_web_page_tag_by_id_async(tenant_id, web_page_tag_id, opts)

Get web page tag by ID

Retrieves a specific web page tag by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPageTagsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_page_tag_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get web page tag by ID
  result = api_instance.get_web_page_tag_by_id_async(tenant_id, web_page_tag_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageTagsApi->get_web_page_tag_by_id_async: #{e}"
end
```

#### Using the get_web_page_tag_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebPageTagDtoEnvelope>, Integer, Hash)> get_web_page_tag_by_id_async_with_http_info(tenant_id, web_page_tag_id, opts)

```ruby
begin
  # Get web page tag by ID
  data, status_code, headers = api_instance.get_web_page_tag_by_id_async_with_http_info(tenant_id, web_page_tag_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebPageTagDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageTagsApi->get_web_page_tag_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_page_tag_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebPageTagDtoEnvelope**](WebPageTagDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_web_page_tags_async

> <WebPageTagDtoListEnvelope> get_web_page_tags_async(tenant_id, opts)

Get web page tags

Retrieves all web page tags for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPageTagsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_page_tag_dto_collection_query_parameters: OpenapiClient::WebPageTagDtoCollectionQueryParameters.new # WebPageTagDtoCollectionQueryParameters | 
}

begin
  # Get web page tags
  result = api_instance.get_web_page_tags_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageTagsApi->get_web_page_tags_async: #{e}"
end
```

#### Using the get_web_page_tags_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebPageTagDtoListEnvelope>, Integer, Hash)> get_web_page_tags_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get web page tags
  data, status_code, headers = api_instance.get_web_page_tags_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebPageTagDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageTagsApi->get_web_page_tags_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_page_tag_dto_collection_query_parameters** | [**WebPageTagDtoCollectionQueryParameters**](WebPageTagDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**WebPageTagDtoListEnvelope**](WebPageTagDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_web_page_tag_async

> <EmptyEnvelope> patch_web_page_tag_async(tenant_id, web_page_tag_id, opts)

Patch a web page tag

Partially updates an existing web page tag for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPageTagsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_page_tag_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a web page tag
  result = api_instance.patch_web_page_tag_async(tenant_id, web_page_tag_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageTagsApi->patch_web_page_tag_async: #{e}"
end
```

#### Using the patch_web_page_tag_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_web_page_tag_async_with_http_info(tenant_id, web_page_tag_id, opts)

```ruby
begin
  # Patch a web page tag
  data, status_code, headers = api_instance.patch_web_page_tag_async_with_http_info(tenant_id, web_page_tag_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageTagsApi->patch_web_page_tag_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_page_tag_id** | **String** |  |  |
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


## update_web_page_tag_async

> <EmptyEnvelope> update_web_page_tag_async(tenant_id, web_page_tag_id, opts)

Update a web page tag

Updates an existing web page tag for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebPageTagsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_page_tag_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_page_tag_update_dto: OpenapiClient::WebPageTagUpdateDto.new # WebPageTagUpdateDto | 
}

begin
  # Update a web page tag
  result = api_instance.update_web_page_tag_async(tenant_id, web_page_tag_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageTagsApi->update_web_page_tag_async: #{e}"
end
```

#### Using the update_web_page_tag_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_web_page_tag_async_with_http_info(tenant_id, web_page_tag_id, opts)

```ruby
begin
  # Update a web page tag
  data, status_code, headers = api_instance.update_web_page_tag_async_with_http_info(tenant_id, web_page_tag_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebPageTagsApi->update_web_page_tag_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_page_tag_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_page_tag_update_dto** | [**WebPageTagUpdateDto**](WebPageTagUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

