# OpenapiClient::SocialGroupsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_social_groups_async**](SocialGroupsApi.md#count_social_groups_async) | **GET** /api/v2/SocialService/SocialGroups/Count | Count social groups |
| [**create_social_group_async**](SocialGroupsApi.md#create_social_group_async) | **POST** /api/v2/SocialService/SocialGroups | Create a social group |
| [**delete_social_group_async**](SocialGroupsApi.md#delete_social_group_async) | **DELETE** /api/v2/SocialService/SocialGroups/{socialGroupId} | Delete a social group |
| [**get_social_group_by_id_async**](SocialGroupsApi.md#get_social_group_by_id_async) | **GET** /api/v2/SocialService/SocialGroups/{socialGroupId} | Get social group by ID |
| [**get_social_groups_async**](SocialGroupsApi.md#get_social_groups_async) | **GET** /api/v2/SocialService/SocialGroups | Get social groups |
| [**patch_social_group_async**](SocialGroupsApi.md#patch_social_group_async) | **PATCH** /api/v2/SocialService/SocialGroups/{socialGroupId} | Patch a social group |
| [**update_social_group_async**](SocialGroupsApi.md#update_social_group_async) | **PUT** /api/v2/SocialService/SocialGroups/{socialGroupId} | Update a social group |


## count_social_groups_async

> <Int32Envelope> count_social_groups_async(tenant_id, opts)

Count social groups

Counts all social groups for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count social groups
  result = api_instance.count_social_groups_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialGroupsApi->count_social_groups_async: #{e}"
end
```

#### Using the count_social_groups_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_social_groups_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count social groups
  data, status_code, headers = api_instance.count_social_groups_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialGroupsApi->count_social_groups_async_with_http_info: #{e}"
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


## create_social_group_async

> <EmptyEnvelope> create_social_group_async(tenant_id, social_profile_id, opts)

Create a social group

Creates a new social group for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_group_create_dto: OpenapiClient::SocialGroupCreateDto.new # SocialGroupCreateDto | 
}

begin
  # Create a social group
  result = api_instance.create_social_group_async(tenant_id, social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialGroupsApi->create_social_group_async: #{e}"
end
```

#### Using the create_social_group_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_social_group_async_with_http_info(tenant_id, social_profile_id, opts)

```ruby
begin
  # Create a social group
  data, status_code, headers = api_instance.create_social_group_async_with_http_info(tenant_id, social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialGroupsApi->create_social_group_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_group_create_dto** | [**SocialGroupCreateDto**](SocialGroupCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_social_group_async

> <EmptyEnvelope> delete_social_group_async(tenant_id, social_profile_id, social_group_id, opts)

Delete a social group

Deletes a social group for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a social group
  result = api_instance.delete_social_group_async(tenant_id, social_profile_id, social_group_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialGroupsApi->delete_social_group_async: #{e}"
end
```

#### Using the delete_social_group_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_social_group_async_with_http_info(tenant_id, social_profile_id, social_group_id, opts)

```ruby
begin
  # Delete a social group
  data, status_code, headers = api_instance.delete_social_group_async_with_http_info(tenant_id, social_profile_id, social_group_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialGroupsApi->delete_social_group_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
| **social_group_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_social_group_by_id_async

> <SocialGroupDtoEnvelope> get_social_group_by_id_async(tenant_id, social_group_id, opts)

Get social group by ID

Retrieves a specific social group by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get social group by ID
  result = api_instance.get_social_group_by_id_async(tenant_id, social_group_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialGroupsApi->get_social_group_by_id_async: #{e}"
end
```

#### Using the get_social_group_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialGroupDtoEnvelope>, Integer, Hash)> get_social_group_by_id_async_with_http_info(tenant_id, social_group_id, opts)

```ruby
begin
  # Get social group by ID
  data, status_code, headers = api_instance.get_social_group_by_id_async_with_http_info(tenant_id, social_group_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialGroupDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialGroupsApi->get_social_group_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **social_group_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialGroupDtoEnvelope**](SocialGroupDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_social_groups_async

> <SocialGroupDtoListEnvelope> get_social_groups_async(tenant_id, opts)

Get social groups

Retrieves all social groups for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get social groups
  result = api_instance.get_social_groups_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialGroupsApi->get_social_groups_async: #{e}"
end
```

#### Using the get_social_groups_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialGroupDtoListEnvelope>, Integer, Hash)> get_social_groups_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get social groups
  data, status_code, headers = api_instance.get_social_groups_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialGroupDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialGroupsApi->get_social_groups_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialGroupDtoListEnvelope**](SocialGroupDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_social_group_async

> <EmptyEnvelope> patch_social_group_async(tenant_id, social_profile_id, social_group_id, opts)

Patch a social group

Partially updates an existing social group using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a social group
  result = api_instance.patch_social_group_async(tenant_id, social_profile_id, social_group_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialGroupsApi->patch_social_group_async: #{e}"
end
```

#### Using the patch_social_group_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_social_group_async_with_http_info(tenant_id, social_profile_id, social_group_id, opts)

```ruby
begin
  # Patch a social group
  data, status_code, headers = api_instance.patch_social_group_async_with_http_info(tenant_id, social_profile_id, social_group_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialGroupsApi->patch_social_group_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
| **social_group_id** | **String** |  |  |
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


## update_social_group_async

> <EmptyEnvelope> update_social_group_async(tenant_id, social_profile_id, social_group_id, opts)

Update a social group

Updates an existing social group for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_group_update_dto: OpenapiClient::SocialGroupUpdateDto.new # SocialGroupUpdateDto | 
}

begin
  # Update a social group
  result = api_instance.update_social_group_async(tenant_id, social_profile_id, social_group_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialGroupsApi->update_social_group_async: #{e}"
end
```

#### Using the update_social_group_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_social_group_async_with_http_info(tenant_id, social_profile_id, social_group_id, opts)

```ruby
begin
  # Update a social group
  data, status_code, headers = api_instance.update_social_group_async_with_http_info(tenant_id, social_profile_id, social_group_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialGroupsApi->update_social_group_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
| **social_group_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_group_update_dto** | [**SocialGroupUpdateDto**](SocialGroupUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

