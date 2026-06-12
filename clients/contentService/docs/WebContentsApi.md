# OpenapiClient::WebContentsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_web_contents_async**](WebContentsApi.md#count_web_contents_async) | **GET** /api/v2/ContentService/WebContents/Count | Count web contents |
| [**create_web_content_async**](WebContentsApi.md#create_web_content_async) | **POST** /api/v2/ContentService/WebContents | Create a web content |
| [**delete_web_content_async**](WebContentsApi.md#delete_web_content_async) | **DELETE** /api/v2/ContentService/WebContents/{webContentId} | Delete a web content |
| [**get_web_content_by_id_async**](WebContentsApi.md#get_web_content_by_id_async) | **GET** /api/v2/ContentService/WebContents/{webContentId} | Get web content by ID |
| [**get_web_contents_async**](WebContentsApi.md#get_web_contents_async) | **GET** /api/v2/ContentService/WebContents | Get web contents |
| [**patch_web_content_async**](WebContentsApi.md#patch_web_content_async) | **PATCH** /api/v2/ContentService/WebContents/{webContentId} | Patch a web content |
| [**update_web_content_async**](WebContentsApi.md#update_web_content_async) | **PUT** /api/v2/ContentService/WebContents/{webContentId} | Update a web content |


## count_web_contents_async

> <Int32Envelope> count_web_contents_async(tenant_id, opts)

Count web contents

Counts all web contents for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebContentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count web contents
  result = api_instance.count_web_contents_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebContentsApi->count_web_contents_async: #{e}"
end
```

#### Using the count_web_contents_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_web_contents_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count web contents
  data, status_code, headers = api_instance.count_web_contents_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebContentsApi->count_web_contents_async_with_http_info: #{e}"
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


## create_web_content_async

> <EmptyEnvelope> create_web_content_async(tenant_id, opts)

Create a web content

Creates a new web content for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebContentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_content_create_dto: OpenapiClient::WebContentCreateDto.new({title: 'title_example'}) # WebContentCreateDto | 
}

begin
  # Create a web content
  result = api_instance.create_web_content_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebContentsApi->create_web_content_async: #{e}"
end
```

#### Using the create_web_content_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_web_content_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a web content
  data, status_code, headers = api_instance.create_web_content_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebContentsApi->create_web_content_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_content_create_dto** | [**WebContentCreateDto**](WebContentCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_web_content_async

> <EmptyEnvelope> delete_web_content_async(tenant_id, web_content_id, opts)

Delete a web content

Deletes a web content for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebContentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_content_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a web content
  result = api_instance.delete_web_content_async(tenant_id, web_content_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebContentsApi->delete_web_content_async: #{e}"
end
```

#### Using the delete_web_content_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_web_content_async_with_http_info(tenant_id, web_content_id, opts)

```ruby
begin
  # Delete a web content
  data, status_code, headers = api_instance.delete_web_content_async_with_http_info(tenant_id, web_content_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebContentsApi->delete_web_content_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_content_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_web_content_by_id_async

> <WebContentDtoEnvelope> get_web_content_by_id_async(tenant_id, web_content_id, opts)

Get web content by ID

Retrieves a specific web content by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebContentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_content_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get web content by ID
  result = api_instance.get_web_content_by_id_async(tenant_id, web_content_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebContentsApi->get_web_content_by_id_async: #{e}"
end
```

#### Using the get_web_content_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebContentDtoEnvelope>, Integer, Hash)> get_web_content_by_id_async_with_http_info(tenant_id, web_content_id, opts)

```ruby
begin
  # Get web content by ID
  data, status_code, headers = api_instance.get_web_content_by_id_async_with_http_info(tenant_id, web_content_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebContentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebContentsApi->get_web_content_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_content_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebContentDtoEnvelope**](WebContentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_web_contents_async

> <WebContentDtoListEnvelope> get_web_contents_async(tenant_id, opts)

Get web contents

Retrieves all web contents for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebContentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get web contents
  result = api_instance.get_web_contents_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebContentsApi->get_web_contents_async: #{e}"
end
```

#### Using the get_web_contents_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebContentDtoListEnvelope>, Integer, Hash)> get_web_contents_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get web contents
  data, status_code, headers = api_instance.get_web_contents_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebContentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebContentsApi->get_web_contents_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebContentDtoListEnvelope**](WebContentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_web_content_async

> <EmptyEnvelope> patch_web_content_async(tenant_id, web_content_id, opts)

Patch a web content

Partially updates an existing web content for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebContentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_content_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a web content
  result = api_instance.patch_web_content_async(tenant_id, web_content_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebContentsApi->patch_web_content_async: #{e}"
end
```

#### Using the patch_web_content_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_web_content_async_with_http_info(tenant_id, web_content_id, opts)

```ruby
begin
  # Patch a web content
  data, status_code, headers = api_instance.patch_web_content_async_with_http_info(tenant_id, web_content_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebContentsApi->patch_web_content_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_content_id** | **String** |  |  |
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


## update_web_content_async

> <EmptyEnvelope> update_web_content_async(tenant_id, web_content_id, opts)

Update a web content

Updates an existing web content for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebContentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_content_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_content_update_dto: OpenapiClient::WebContentUpdateDto.new # WebContentUpdateDto | 
}

begin
  # Update a web content
  result = api_instance.update_web_content_async(tenant_id, web_content_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebContentsApi->update_web_content_async: #{e}"
end
```

#### Using the update_web_content_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_web_content_async_with_http_info(tenant_id, web_content_id, opts)

```ruby
begin
  # Update a web content
  data, status_code, headers = api_instance.update_web_content_async_with_http_info(tenant_id, web_content_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebContentsApi->update_web_content_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_content_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_content_update_dto** | [**WebContentUpdateDto**](WebContentUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

