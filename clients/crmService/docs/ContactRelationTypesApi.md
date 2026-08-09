# OpenapiClient::ContactRelationTypesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_contact_relation_type_async**](ContactRelationTypesApi.md#create_contact_relation_type_async) | **POST** /api/v2/CrmService/ContactRelationTypes | Create a new contact relation type |
| [**delete_contact_relation_type_async**](ContactRelationTypesApi.md#delete_contact_relation_type_async) | **DELETE** /api/v2/CrmService/ContactRelationTypes/{id} | Delete a contact relation type |
| [**get_contact_relation_type_by_id_async**](ContactRelationTypesApi.md#get_contact_relation_type_by_id_async) | **GET** /api/v2/CrmService/ContactRelationTypes/{id} | Get contact relation type by ID |
| [**get_contact_relation_types_async**](ContactRelationTypesApi.md#get_contact_relation_types_async) | **GET** /api/v2/CrmService/ContactRelationTypes | Get all contact relation types |
| [**get_contact_relation_types_count_async**](ContactRelationTypesApi.md#get_contact_relation_types_count_async) | **GET** /api/v2/CrmService/ContactRelationTypes/Count | Get contact relation types count |
| [**patch_contact_relation_type_async**](ContactRelationTypesApi.md#patch_contact_relation_type_async) | **PATCH** /api/v2/CrmService/ContactRelationTypes/{id} | Patch a contact relation type |
| [**update_contact_relation_type_async**](ContactRelationTypesApi.md#update_contact_relation_type_async) | **PUT** /api/v2/CrmService/ContactRelationTypes/{id} | Update a contact relation type |


## create_contact_relation_type_async

> create_contact_relation_type_async(tenant_id, opts)

Create a new contact relation type

Creates a new contact relation type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactRelationTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_relation_type_create_dto: OpenapiClient::ContactRelationTypeCreateDto.new({name: 'name_example'}) # ContactRelationTypeCreateDto | 
}

begin
  # Create a new contact relation type
  api_instance.create_contact_relation_type_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationTypesApi->create_contact_relation_type_async: #{e}"
end
```

#### Using the create_contact_relation_type_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_contact_relation_type_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new contact relation type
  data, status_code, headers = api_instance.create_contact_relation_type_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationTypesApi->create_contact_relation_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_relation_type_create_dto** | [**ContactRelationTypeCreateDto**](ContactRelationTypeCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_contact_relation_type_async

> delete_contact_relation_type_async(tenant_id, id, opts)

Delete a contact relation type

Deletes a contact relation type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactRelationTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a contact relation type
  api_instance.delete_contact_relation_type_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationTypesApi->delete_contact_relation_type_async: #{e}"
end
```

#### Using the delete_contact_relation_type_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_contact_relation_type_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a contact relation type
  data, status_code, headers = api_instance.delete_contact_relation_type_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationTypesApi->delete_contact_relation_type_async_with_http_info: #{e}"
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


## get_contact_relation_type_by_id_async

> <ContactRelationTypeDto> get_contact_relation_type_by_id_async(tenant_id, id, opts)

Get contact relation type by ID

Retrieves a specific contact relation type by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactRelationTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get contact relation type by ID
  result = api_instance.get_contact_relation_type_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationTypesApi->get_contact_relation_type_by_id_async: #{e}"
end
```

#### Using the get_contact_relation_type_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactRelationTypeDto>, Integer, Hash)> get_contact_relation_type_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get contact relation type by ID
  data, status_code, headers = api_instance.get_contact_relation_type_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactRelationTypeDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationTypesApi->get_contact_relation_type_by_id_async_with_http_info: #{e}"
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

[**ContactRelationTypeDto**](ContactRelationTypeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_contact_relation_types_async

> <ContactRelationTypeDtoListEnvelope> get_contact_relation_types_async(tenant_id, opts)

Get all contact relation types

Retrieves all contact relation types for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactRelationTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_relation_type_dto_collection_query_parameters: OpenapiClient::ContactRelationTypeDtoCollectionQueryParameters.new # ContactRelationTypeDtoCollectionQueryParameters | 
}

begin
  # Get all contact relation types
  result = api_instance.get_contact_relation_types_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationTypesApi->get_contact_relation_types_async: #{e}"
end
```

#### Using the get_contact_relation_types_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactRelationTypeDtoListEnvelope>, Integer, Hash)> get_contact_relation_types_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all contact relation types
  data, status_code, headers = api_instance.get_contact_relation_types_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactRelationTypeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationTypesApi->get_contact_relation_types_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_relation_type_dto_collection_query_parameters** | [**ContactRelationTypeDtoCollectionQueryParameters**](ContactRelationTypeDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ContactRelationTypeDtoListEnvelope**](ContactRelationTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_contact_relation_types_count_async

> <Int32Envelope> get_contact_relation_types_count_async(tenant_id, opts)

Get contact relation types count

Returns the count of contact relation types for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactRelationTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_relation_type_dto_collection_query_parameters: OpenapiClient::ContactRelationTypeDtoCollectionQueryParameters.new # ContactRelationTypeDtoCollectionQueryParameters | 
}

begin
  # Get contact relation types count
  result = api_instance.get_contact_relation_types_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationTypesApi->get_contact_relation_types_count_async: #{e}"
end
```

#### Using the get_contact_relation_types_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_contact_relation_types_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get contact relation types count
  data, status_code, headers = api_instance.get_contact_relation_types_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationTypesApi->get_contact_relation_types_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_relation_type_dto_collection_query_parameters** | [**ContactRelationTypeDtoCollectionQueryParameters**](ContactRelationTypeDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_contact_relation_type_async

> <EmptyEnvelope> patch_contact_relation_type_async(tenant_id, id, opts)

Patch a contact relation type

Patch a contact relation type

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactRelationTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a contact relation type
  result = api_instance.patch_contact_relation_type_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationTypesApi->patch_contact_relation_type_async: #{e}"
end
```

#### Using the patch_contact_relation_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_contact_relation_type_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a contact relation type
  data, status_code, headers = api_instance.patch_contact_relation_type_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationTypesApi->patch_contact_relation_type_async_with_http_info: #{e}"
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


## update_contact_relation_type_async

> update_contact_relation_type_async(tenant_id, id, opts)

Update a contact relation type

Updates an existing contact relation type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactRelationTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_relation_type_update_dto: OpenapiClient::ContactRelationTypeUpdateDto.new({name: 'name_example'}) # ContactRelationTypeUpdateDto | 
}

begin
  # Update a contact relation type
  api_instance.update_contact_relation_type_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationTypesApi->update_contact_relation_type_async: #{e}"
end
```

#### Using the update_contact_relation_type_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_contact_relation_type_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a contact relation type
  data, status_code, headers = api_instance.update_contact_relation_type_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactRelationTypesApi->update_contact_relation_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_relation_type_update_dto** | [**ContactRelationTypeUpdateDto**](ContactRelationTypeUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

