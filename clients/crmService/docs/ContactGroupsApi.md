# OpenapiClient::ContactGroupsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_contact_group_async**](ContactGroupsApi.md#create_contact_group_async) | **POST** /api/v2/CrmService/ContactGroups | Create a new contact group |
| [**delete_contact_group_async**](ContactGroupsApi.md#delete_contact_group_async) | **DELETE** /api/v2/CrmService/ContactGroups/{id} | Delete a contact group |
| [**get_contact_group_by_id_async**](ContactGroupsApi.md#get_contact_group_by_id_async) | **GET** /api/v2/CrmService/ContactGroups/{id} | Get contact group by ID |
| [**get_contact_groups_async**](ContactGroupsApi.md#get_contact_groups_async) | **GET** /api/v2/CrmService/ContactGroups | Get all contact groups |
| [**get_contact_groups_count_async**](ContactGroupsApi.md#get_contact_groups_count_async) | **GET** /api/v2/CrmService/ContactGroups/Count | Get contact groups count |
| [**patch_contact_group_async**](ContactGroupsApi.md#patch_contact_group_async) | **PATCH** /api/v2/CrmService/ContactGroups/{id} | Patch a contact group |
| [**update_contact_group_async**](ContactGroupsApi.md#update_contact_group_async) | **PUT** /api/v2/CrmService/ContactGroups/{id} | Update a contact group |


## create_contact_group_async

> create_contact_group_async(tenant_id, opts)

Create a new contact group

Creates a new contact group for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contacts_group_create_dto: OpenapiClient::ContactsGroupCreateDto.new({name: 'name_example'}) # ContactsGroupCreateDto | 
}

begin
  # Create a new contact group
  api_instance.create_contact_group_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactGroupsApi->create_contact_group_async: #{e}"
end
```

#### Using the create_contact_group_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_contact_group_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new contact group
  data, status_code, headers = api_instance.create_contact_group_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactGroupsApi->create_contact_group_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contacts_group_create_dto** | [**ContactsGroupCreateDto**](ContactsGroupCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_contact_group_async

> delete_contact_group_async(tenant_id, id, opts)

Delete a contact group

Deletes a contact group for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a contact group
  api_instance.delete_contact_group_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactGroupsApi->delete_contact_group_async: #{e}"
end
```

#### Using the delete_contact_group_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_contact_group_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a contact group
  data, status_code, headers = api_instance.delete_contact_group_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactGroupsApi->delete_contact_group_async_with_http_info: #{e}"
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


## get_contact_group_by_id_async

> <ContactsGroupDto> get_contact_group_by_id_async(tenant_id, id, opts)

Get contact group by ID

Retrieves a specific contact group by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get contact group by ID
  result = api_instance.get_contact_group_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactGroupsApi->get_contact_group_by_id_async: #{e}"
end
```

#### Using the get_contact_group_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactsGroupDto>, Integer, Hash)> get_contact_group_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get contact group by ID
  data, status_code, headers = api_instance.get_contact_group_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactsGroupDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactGroupsApi->get_contact_group_by_id_async_with_http_info: #{e}"
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

[**ContactsGroupDto**](ContactsGroupDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_contact_groups_async

> <ContactsGroupDtoListEnvelope> get_contact_groups_async(tenant_id, opts)

Get all contact groups

Retrieves all contact groups for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contacts_group_dto_collection_query_parameters: OpenapiClient::ContactsGroupDtoCollectionQueryParameters.new # ContactsGroupDtoCollectionQueryParameters | 
}

begin
  # Get all contact groups
  result = api_instance.get_contact_groups_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactGroupsApi->get_contact_groups_async: #{e}"
end
```

#### Using the get_contact_groups_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactsGroupDtoListEnvelope>, Integer, Hash)> get_contact_groups_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all contact groups
  data, status_code, headers = api_instance.get_contact_groups_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactsGroupDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactGroupsApi->get_contact_groups_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contacts_group_dto_collection_query_parameters** | [**ContactsGroupDtoCollectionQueryParameters**](ContactsGroupDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ContactsGroupDtoListEnvelope**](ContactsGroupDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_contact_groups_count_async

> <Int32Envelope> get_contact_groups_count_async(tenant_id, opts)

Get contact groups count

Returns the count of contact groups for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contacts_group_dto_collection_query_parameters: OpenapiClient::ContactsGroupDtoCollectionQueryParameters.new # ContactsGroupDtoCollectionQueryParameters | 
}

begin
  # Get contact groups count
  result = api_instance.get_contact_groups_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactGroupsApi->get_contact_groups_count_async: #{e}"
end
```

#### Using the get_contact_groups_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_contact_groups_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get contact groups count
  data, status_code, headers = api_instance.get_contact_groups_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactGroupsApi->get_contact_groups_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contacts_group_dto_collection_query_parameters** | [**ContactsGroupDtoCollectionQueryParameters**](ContactsGroupDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_contact_group_async

> <EmptyEnvelope> patch_contact_group_async(tenant_id, id, opts)

Patch a contact group

Patch a contact group

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a contact group
  result = api_instance.patch_contact_group_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactGroupsApi->patch_contact_group_async: #{e}"
end
```

#### Using the patch_contact_group_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_contact_group_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a contact group
  data, status_code, headers = api_instance.patch_contact_group_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactGroupsApi->patch_contact_group_async_with_http_info: #{e}"
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


## update_contact_group_async

> update_contact_group_async(tenant_id, id, opts)

Update a contact group

Updates an existing contact group for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contacts_group_update_dto: OpenapiClient::ContactsGroupUpdateDto.new({name: 'name_example'}) # ContactsGroupUpdateDto | 
}

begin
  # Update a contact group
  api_instance.update_contact_group_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactGroupsApi->update_contact_group_async: #{e}"
end
```

#### Using the update_contact_group_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_contact_group_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a contact group
  data, status_code, headers = api_instance.update_contact_group_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactGroupsApi->update_contact_group_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contacts_group_update_dto** | [**ContactsGroupUpdateDto**](ContactsGroupUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

