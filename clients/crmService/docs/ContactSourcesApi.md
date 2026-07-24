# OpenapiClient::ContactSourcesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_contact_source_async**](ContactSourcesApi.md#create_contact_source_async) | **POST** /api/v2/CrmService/ContactSources | Create a new contact source |
| [**delete_contact_source_async**](ContactSourcesApi.md#delete_contact_source_async) | **DELETE** /api/v2/CrmService/ContactSources/{id} | Delete a contact source |
| [**get_contact_source_by_id_async**](ContactSourcesApi.md#get_contact_source_by_id_async) | **GET** /api/v2/CrmService/ContactSources/{id} | Get contact source by ID |
| [**get_contact_sources_async**](ContactSourcesApi.md#get_contact_sources_async) | **GET** /api/v2/CrmService/ContactSources | Get all contact sources |
| [**get_contact_sources_count_async**](ContactSourcesApi.md#get_contact_sources_count_async) | **GET** /api/v2/CrmService/ContactSources/Count | Get contact sources count |
| [**patch_contact_source_async**](ContactSourcesApi.md#patch_contact_source_async) | **PATCH** /api/v2/CrmService/ContactSources/{id} | Patch a contact source |
| [**update_contact_source_async**](ContactSourcesApi.md#update_contact_source_async) | **PUT** /api/v2/CrmService/ContactSources/{id} | Update a contact source |


## create_contact_source_async

> create_contact_source_async(tenant_id, opts)

Create a new contact source

Creates a new contact source for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactSourcesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_source_create_dto: OpenapiClient::ContactSourceCreateDto.new({name: 'name_example'}) # ContactSourceCreateDto | 
}

begin
  # Create a new contact source
  api_instance.create_contact_source_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactSourcesApi->create_contact_source_async: #{e}"
end
```

#### Using the create_contact_source_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_contact_source_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new contact source
  data, status_code, headers = api_instance.create_contact_source_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactSourcesApi->create_contact_source_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_source_create_dto** | [**ContactSourceCreateDto**](ContactSourceCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_contact_source_async

> delete_contact_source_async(tenant_id, id, opts)

Delete a contact source

Deletes a contact source for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactSourcesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a contact source
  api_instance.delete_contact_source_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactSourcesApi->delete_contact_source_async: #{e}"
end
```

#### Using the delete_contact_source_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_contact_source_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a contact source
  data, status_code, headers = api_instance.delete_contact_source_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactSourcesApi->delete_contact_source_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_contact_source_by_id_async

> <ContactSourceDto> get_contact_source_by_id_async(tenant_id, id, opts)

Get contact source by ID

Retrieves a specific contact source by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactSourcesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get contact source by ID
  result = api_instance.get_contact_source_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactSourcesApi->get_contact_source_by_id_async: #{e}"
end
```

#### Using the get_contact_source_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactSourceDto>, Integer, Hash)> get_contact_source_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get contact source by ID
  data, status_code, headers = api_instance.get_contact_source_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactSourceDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactSourcesApi->get_contact_source_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ContactSourceDto**](ContactSourceDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_contact_sources_async

> <ContactSourceDtoListEnvelope> get_contact_sources_async(tenant_id, opts)

Get all contact sources

Retrieves all contact sources for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactSourcesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all contact sources
  result = api_instance.get_contact_sources_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactSourcesApi->get_contact_sources_async: #{e}"
end
```

#### Using the get_contact_sources_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactSourceDtoListEnvelope>, Integer, Hash)> get_contact_sources_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all contact sources
  data, status_code, headers = api_instance.get_contact_sources_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactSourceDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactSourcesApi->get_contact_sources_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ContactSourceDtoListEnvelope**](ContactSourceDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_contact_sources_count_async

> <Int32Envelope> get_contact_sources_count_async(tenant_id, opts)

Get contact sources count

Returns the count of contact sources for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactSourcesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get contact sources count
  result = api_instance.get_contact_sources_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactSourcesApi->get_contact_sources_count_async: #{e}"
end
```

#### Using the get_contact_sources_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_contact_sources_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get contact sources count
  data, status_code, headers = api_instance.get_contact_sources_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactSourcesApi->get_contact_sources_count_async_with_http_info: #{e}"
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


## patch_contact_source_async

> <EmptyEnvelope> patch_contact_source_async(tenant_id, id, opts)

Patch a contact source

Patch a contact source

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactSourcesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a contact source
  result = api_instance.patch_contact_source_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactSourcesApi->patch_contact_source_async: #{e}"
end
```

#### Using the patch_contact_source_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_contact_source_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a contact source
  data, status_code, headers = api_instance.patch_contact_source_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactSourcesApi->patch_contact_source_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
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


## update_contact_source_async

> update_contact_source_async(tenant_id, id, opts)

Update a contact source

Updates an existing contact source for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactSourcesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_source_update_dto: OpenapiClient::ContactSourceUpdateDto.new({name: 'name_example'}) # ContactSourceUpdateDto | 
}

begin
  # Update a contact source
  api_instance.update_contact_source_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactSourcesApi->update_contact_source_async: #{e}"
end
```

#### Using the update_contact_source_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_contact_source_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a contact source
  data, status_code, headers = api_instance.update_contact_source_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactSourcesApi->update_contact_source_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_source_update_dto** | [**ContactSourceUpdateDto**](ContactSourceUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

