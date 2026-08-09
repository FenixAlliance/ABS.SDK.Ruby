# OpenapiClient::ContactRelationsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_contact_relation_async**](ContactRelationsApi.md#create_contact_relation_async) | **POST** /api/v2/CrmService/ContactRelations | Create a new contact relation |
| [**delete_contact_relation_async**](ContactRelationsApi.md#delete_contact_relation_async) | **DELETE** /api/v2/CrmService/ContactRelations/{id} | Delete a contact relation |
| [**get_contact_relation_by_id_async**](ContactRelationsApi.md#get_contact_relation_by_id_async) | **GET** /api/v2/CrmService/ContactRelations/{id} | Get contact relation by ID |
| [**get_contact_relations_async**](ContactRelationsApi.md#get_contact_relations_async) | **GET** /api/v2/CrmService/ContactRelations | Get all contact relations |
| [**get_contact_relations_count_async**](ContactRelationsApi.md#get_contact_relations_count_async) | **GET** /api/v2/CrmService/ContactRelations/Count | Get contact relations count |
| [**patch_contact_relation_async**](ContactRelationsApi.md#patch_contact_relation_async) | **PATCH** /api/v2/CrmService/ContactRelations/{id} | Patch a contact relation |
| [**update_contact_relation_async**](ContactRelationsApi.md#update_contact_relation_async) | **PUT** /api/v2/CrmService/ContactRelations/{id} | Update a contact relation |


## create_contact_relation_async

> create_contact_relation_async(tenant_id, opts)

Create a new contact relation

Creates a new contact relation for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactRelationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_relation_create_dto: OpenapiClient::ContactRelationCreateDto.new # ContactRelationCreateDto | 
}

begin
  # Create a new contact relation
  api_instance.create_contact_relation_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationsApi->create_contact_relation_async: #{e}"
end
```

#### Using the create_contact_relation_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_contact_relation_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new contact relation
  data, status_code, headers = api_instance.create_contact_relation_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationsApi->create_contact_relation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_relation_create_dto** | [**ContactRelationCreateDto**](ContactRelationCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_contact_relation_async

> delete_contact_relation_async(tenant_id, id, opts)

Delete a contact relation

Deletes a contact relation for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactRelationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a contact relation
  api_instance.delete_contact_relation_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationsApi->delete_contact_relation_async: #{e}"
end
```

#### Using the delete_contact_relation_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_contact_relation_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a contact relation
  data, status_code, headers = api_instance.delete_contact_relation_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationsApi->delete_contact_relation_async_with_http_info: #{e}"
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


## get_contact_relation_by_id_async

> <ContactRelationDto> get_contact_relation_by_id_async(tenant_id, id, opts)

Get contact relation by ID

Retrieves a specific contact relation by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactRelationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get contact relation by ID
  result = api_instance.get_contact_relation_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationsApi->get_contact_relation_by_id_async: #{e}"
end
```

#### Using the get_contact_relation_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactRelationDto>, Integer, Hash)> get_contact_relation_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get contact relation by ID
  data, status_code, headers = api_instance.get_contact_relation_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactRelationDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationsApi->get_contact_relation_by_id_async_with_http_info: #{e}"
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

[**ContactRelationDto**](ContactRelationDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_contact_relations_async

> <ContactRelationDtoListEnvelope> get_contact_relations_async(tenant_id, opts)

Get all contact relations

Retrieves all contact relations for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactRelationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_relation_dto_collection_query_parameters: OpenapiClient::ContactRelationDtoCollectionQueryParameters.new # ContactRelationDtoCollectionQueryParameters | 
}

begin
  # Get all contact relations
  result = api_instance.get_contact_relations_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationsApi->get_contact_relations_async: #{e}"
end
```

#### Using the get_contact_relations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactRelationDtoListEnvelope>, Integer, Hash)> get_contact_relations_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all contact relations
  data, status_code, headers = api_instance.get_contact_relations_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactRelationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationsApi->get_contact_relations_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_relation_dto_collection_query_parameters** | [**ContactRelationDtoCollectionQueryParameters**](ContactRelationDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ContactRelationDtoListEnvelope**](ContactRelationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_contact_relations_count_async

> <Int32Envelope> get_contact_relations_count_async(tenant_id, opts)

Get contact relations count

Returns the count of contact relations for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactRelationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_relation_dto_collection_query_parameters: OpenapiClient::ContactRelationDtoCollectionQueryParameters.new # ContactRelationDtoCollectionQueryParameters | 
}

begin
  # Get contact relations count
  result = api_instance.get_contact_relations_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationsApi->get_contact_relations_count_async: #{e}"
end
```

#### Using the get_contact_relations_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_contact_relations_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get contact relations count
  data, status_code, headers = api_instance.get_contact_relations_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationsApi->get_contact_relations_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_relation_dto_collection_query_parameters** | [**ContactRelationDtoCollectionQueryParameters**](ContactRelationDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_contact_relation_async

> <EmptyEnvelope> patch_contact_relation_async(tenant_id, id, opts)

Patch a contact relation

Patch a contact relation

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactRelationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a contact relation
  result = api_instance.patch_contact_relation_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationsApi->patch_contact_relation_async: #{e}"
end
```

#### Using the patch_contact_relation_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_contact_relation_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a contact relation
  data, status_code, headers = api_instance.patch_contact_relation_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationsApi->patch_contact_relation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
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


## update_contact_relation_async

> update_contact_relation_async(tenant_id, id, opts)

Update a contact relation

Updates an existing contact relation for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactRelationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_relation_update_dto: OpenapiClient::ContactRelationUpdateDto.new # ContactRelationUpdateDto | 
}

begin
  # Update a contact relation
  api_instance.update_contact_relation_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationsApi->update_contact_relation_async: #{e}"
end
```

#### Using the update_contact_relation_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_contact_relation_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a contact relation
  data, status_code, headers = api_instance.update_contact_relation_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationsApi->update_contact_relation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_relation_update_dto** | [**ContactRelationUpdateDto**](ContactRelationUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

