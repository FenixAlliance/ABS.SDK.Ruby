# OpenapiClient::WebComponentsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_web_components_async**](WebComponentsApi.md#count_web_components_async) | **GET** /api/v2/ContentService/WebComponents/Count | Count web components |
| [**create_web_component_async**](WebComponentsApi.md#create_web_component_async) | **POST** /api/v2/ContentService/WebComponents | Create a web component |
| [**delete_web_component_async**](WebComponentsApi.md#delete_web_component_async) | **DELETE** /api/v2/ContentService/WebComponents/{webComponentId} | Delete a web component |
| [**get_web_component_by_id_async**](WebComponentsApi.md#get_web_component_by_id_async) | **GET** /api/v2/ContentService/WebComponents/{webComponentId} | Get web component by ID |
| [**get_web_components_async**](WebComponentsApi.md#get_web_components_async) | **GET** /api/v2/ContentService/WebComponents | Get web components |
| [**update_web_component_async**](WebComponentsApi.md#update_web_component_async) | **PUT** /api/v2/ContentService/WebComponents/{webComponentId} | Update a web component |


## count_web_components_async

> <Int32Envelope> count_web_components_async(tenant_id, opts)

Count web components

Counts all web components for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebComponentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_component_dto_collection_query_parameters: OpenapiClient::WebComponentDtoCollectionQueryParameters.new # WebComponentDtoCollectionQueryParameters | 
}

begin
  # Count web components
  result = api_instance.count_web_components_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebComponentsApi->count_web_components_async: #{e}"
end
```

#### Using the count_web_components_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_web_components_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count web components
  data, status_code, headers = api_instance.count_web_components_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebComponentsApi->count_web_components_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_component_dto_collection_query_parameters** | [**WebComponentDtoCollectionQueryParameters**](WebComponentDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_web_component_async

> <EmptyEnvelope> create_web_component_async(tenant_id, web_component_create_dto, opts)

Create a web component

Creates a new web component for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebComponentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_component_create_dto = OpenapiClient::WebComponentCreateDto.new({name: 'name_example'}) # WebComponentCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a web component
  result = api_instance.create_web_component_async(tenant_id, web_component_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebComponentsApi->create_web_component_async: #{e}"
end
```

#### Using the create_web_component_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_web_component_async_with_http_info(tenant_id, web_component_create_dto, opts)

```ruby
begin
  # Create a web component
  data, status_code, headers = api_instance.create_web_component_async_with_http_info(tenant_id, web_component_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebComponentsApi->create_web_component_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_component_create_dto** | [**WebComponentCreateDto**](WebComponentCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_web_component_async

> <EmptyEnvelope> delete_web_component_async(tenant_id, web_component_id, opts)

Delete a web component

Deletes a web component for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebComponentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_component_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a web component
  result = api_instance.delete_web_component_async(tenant_id, web_component_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebComponentsApi->delete_web_component_async: #{e}"
end
```

#### Using the delete_web_component_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_web_component_async_with_http_info(tenant_id, web_component_id, opts)

```ruby
begin
  # Delete a web component
  data, status_code, headers = api_instance.delete_web_component_async_with_http_info(tenant_id, web_component_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebComponentsApi->delete_web_component_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_component_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_web_component_by_id_async

> <WebComponentDtoEnvelope> get_web_component_by_id_async(tenant_id, web_component_id, opts)

Get web component by ID

Retrieves a specific web component by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebComponentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_component_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get web component by ID
  result = api_instance.get_web_component_by_id_async(tenant_id, web_component_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebComponentsApi->get_web_component_by_id_async: #{e}"
end
```

#### Using the get_web_component_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebComponentDtoEnvelope>, Integer, Hash)> get_web_component_by_id_async_with_http_info(tenant_id, web_component_id, opts)

```ruby
begin
  # Get web component by ID
  data, status_code, headers = api_instance.get_web_component_by_id_async_with_http_info(tenant_id, web_component_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebComponentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebComponentsApi->get_web_component_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_component_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebComponentDtoEnvelope**](WebComponentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_web_components_async

> <WebComponentDtoListEnvelope> get_web_components_async(tenant_id, opts)

Get web components

Retrieves all web components for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebComponentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_component_dto_collection_query_parameters: OpenapiClient::WebComponentDtoCollectionQueryParameters.new # WebComponentDtoCollectionQueryParameters | 
}

begin
  # Get web components
  result = api_instance.get_web_components_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebComponentsApi->get_web_components_async: #{e}"
end
```

#### Using the get_web_components_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebComponentDtoListEnvelope>, Integer, Hash)> get_web_components_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get web components
  data, status_code, headers = api_instance.get_web_components_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebComponentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebComponentsApi->get_web_components_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_component_dto_collection_query_parameters** | [**WebComponentDtoCollectionQueryParameters**](WebComponentDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**WebComponentDtoListEnvelope**](WebComponentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_web_component_async

> <EmptyEnvelope> update_web_component_async(tenant_id, web_component_id, web_component_update_dto, opts)

Update a web component

Updates an existing web component for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebComponentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_component_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
web_component_update_dto = OpenapiClient::WebComponentUpdateDto.new # WebComponentUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update a web component
  result = api_instance.update_web_component_async(tenant_id, web_component_id, web_component_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebComponentsApi->update_web_component_async: #{e}"
end
```

#### Using the update_web_component_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_web_component_async_with_http_info(tenant_id, web_component_id, web_component_update_dto, opts)

```ruby
begin
  # Update a web component
  data, status_code, headers = api_instance.update_web_component_async_with_http_info(tenant_id, web_component_id, web_component_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebComponentsApi->update_web_component_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **web_component_id** | **String** |  |  |
| **web_component_update_dto** | [**WebComponentUpdateDto**](WebComponentUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

