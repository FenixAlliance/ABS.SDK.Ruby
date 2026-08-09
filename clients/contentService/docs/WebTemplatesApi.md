# OpenapiClient::WebTemplatesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_web_templates_async**](WebTemplatesApi.md#count_web_templates_async) | **GET** /api/v2/ContentService/WebTemplates/Count | Count web templates |
| [**create_web_template_async**](WebTemplatesApi.md#create_web_template_async) | **POST** /api/v2/ContentService/WebTemplates | Create a web template |
| [**delete_web_template_async**](WebTemplatesApi.md#delete_web_template_async) | **DELETE** /api/v2/ContentService/WebTemplates/{webTemplateId} | Delete a web template |
| [**get_web_template_by_id_async**](WebTemplatesApi.md#get_web_template_by_id_async) | **GET** /api/v2/ContentService/WebTemplates/{webTemplateId} | Get web template by ID |
| [**get_web_templates_async**](WebTemplatesApi.md#get_web_templates_async) | **GET** /api/v2/ContentService/WebTemplates | Get web templates |
| [**patch_web_template_async**](WebTemplatesApi.md#patch_web_template_async) | **PATCH** /api/v2/ContentService/WebTemplates/{webTemplateId} | Patch a web template |
| [**update_web_template_async**](WebTemplatesApi.md#update_web_template_async) | **PUT** /api/v2/ContentService/WebTemplates/{webTemplateId} | Update a web template |


## count_web_templates_async

> <Int32Envelope> count_web_templates_async(tenant_id, opts)

Count web templates

Counts all web templates for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebTemplatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_template_dto_collection_query_parameters: OpenapiClient::WebTemplateDtoCollectionQueryParameters.new # WebTemplateDtoCollectionQueryParameters | 
}

begin
  # Count web templates
  result = api_instance.count_web_templates_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebTemplatesApi->count_web_templates_async: #{e}"
end
```

#### Using the count_web_templates_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_web_templates_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count web templates
  data, status_code, headers = api_instance.count_web_templates_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebTemplatesApi->count_web_templates_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_template_dto_collection_query_parameters** | [**WebTemplateDtoCollectionQueryParameters**](WebTemplateDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_web_template_async

> create_web_template_async(tenant_id, opts)

Create a web template

Creates a new web template for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebTemplatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_template_create_dto: OpenapiClient::WebTemplateCreateDto.new # WebTemplateCreateDto | 
}

begin
  # Create a web template
  api_instance.create_web_template_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebTemplatesApi->create_web_template_async: #{e}"
end
```

#### Using the create_web_template_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_web_template_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a web template
  data, status_code, headers = api_instance.create_web_template_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebTemplatesApi->create_web_template_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_template_create_dto** | [**WebTemplateCreateDto**](WebTemplateCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_web_template_async

> delete_web_template_async(tenant_id, web_template_id, opts)

Delete a web template

Deletes a web template for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebTemplatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_template_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a web template
  api_instance.delete_web_template_async(tenant_id, web_template_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebTemplatesApi->delete_web_template_async: #{e}"
end
```

#### Using the delete_web_template_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_web_template_async_with_http_info(tenant_id, web_template_id, opts)

```ruby
begin
  # Delete a web template
  data, status_code, headers = api_instance.delete_web_template_async_with_http_info(tenant_id, web_template_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebTemplatesApi->delete_web_template_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_template_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_web_template_by_id_async

> <WebTemplateDtoEnvelope> get_web_template_by_id_async(tenant_id, web_template_id, opts)

Get web template by ID

Retrieves a specific web template by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebTemplatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_template_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get web template by ID
  result = api_instance.get_web_template_by_id_async(tenant_id, web_template_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebTemplatesApi->get_web_template_by_id_async: #{e}"
end
```

#### Using the get_web_template_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebTemplateDtoEnvelope>, Integer, Hash)> get_web_template_by_id_async_with_http_info(tenant_id, web_template_id, opts)

```ruby
begin
  # Get web template by ID
  data, status_code, headers = api_instance.get_web_template_by_id_async_with_http_info(tenant_id, web_template_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebTemplateDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebTemplatesApi->get_web_template_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_template_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebTemplateDtoEnvelope**](WebTemplateDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_web_templates_async

> <WebTemplateDtoListEnvelope> get_web_templates_async(tenant_id, opts)

Get web templates

Retrieves all web templates for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebTemplatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_template_dto_collection_query_parameters: OpenapiClient::WebTemplateDtoCollectionQueryParameters.new # WebTemplateDtoCollectionQueryParameters | 
}

begin
  # Get web templates
  result = api_instance.get_web_templates_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebTemplatesApi->get_web_templates_async: #{e}"
end
```

#### Using the get_web_templates_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebTemplateDtoListEnvelope>, Integer, Hash)> get_web_templates_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get web templates
  data, status_code, headers = api_instance.get_web_templates_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebTemplateDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebTemplatesApi->get_web_templates_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_template_dto_collection_query_parameters** | [**WebTemplateDtoCollectionQueryParameters**](WebTemplateDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**WebTemplateDtoListEnvelope**](WebTemplateDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_web_template_async

> patch_web_template_async(tenant_id, web_template_id, opts)

Patch a web template

Partially updates an existing web template for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebTemplatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_template_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a web template
  api_instance.patch_web_template_async(tenant_id, web_template_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebTemplatesApi->patch_web_template_async: #{e}"
end
```

#### Using the patch_web_template_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> patch_web_template_async_with_http_info(tenant_id, web_template_id, opts)

```ruby
begin
  # Patch a web template
  data, status_code, headers = api_instance.patch_web_template_async_with_http_info(tenant_id, web_template_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebTemplatesApi->patch_web_template_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_template_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_web_template_async

> update_web_template_async(tenant_id, web_template_id, opts)

Update a web template

Updates an existing web template for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebTemplatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_template_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_template_update_dto: OpenapiClient::WebTemplateUpdateDto.new # WebTemplateUpdateDto | 
}

begin
  # Update a web template
  api_instance.update_web_template_async(tenant_id, web_template_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebTemplatesApi->update_web_template_async: #{e}"
end
```

#### Using the update_web_template_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_web_template_async_with_http_info(tenant_id, web_template_id, opts)

```ruby
begin
  # Update a web template
  data, status_code, headers = api_instance.update_web_template_async_with_http_info(tenant_id, web_template_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebTemplatesApi->update_web_template_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_template_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_template_update_dto** | [**WebTemplateUpdateDto**](WebTemplateUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

