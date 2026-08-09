# OpenapiClient::EmailGroupsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_email_group_async**](EmailGroupsApi.md#create_email_group_async) | **POST** /api/v2/MarketingService/EmailGroups | Create an email group |
| [**delete_email_group_async**](EmailGroupsApi.md#delete_email_group_async) | **DELETE** /api/v2/MarketingService/EmailGroups/{emailgroupId} | Delete an email group |
| [**get_email_group_details_async**](EmailGroupsApi.md#get_email_group_details_async) | **GET** /api/v2/MarketingService/EmailGroups/{emailgroupId} | Get email group by ID |
| [**get_email_groups_count_async**](EmailGroupsApi.md#get_email_groups_count_async) | **GET** /api/v2/MarketingService/EmailGroups/Count | Get email groups count |
| [**get_email_groups_o_data_async**](EmailGroupsApi.md#get_email_groups_o_data_async) | **GET** /api/v2/MarketingService/EmailGroups | Get email groups |
| [**patch_email_group_async**](EmailGroupsApi.md#patch_email_group_async) | **PATCH** /api/v2/MarketingService/EmailGroups/{emailgroupId} | Patch an email group |
| [**update_email_group_async**](EmailGroupsApi.md#update_email_group_async) | **PUT** /api/v2/MarketingService/EmailGroups/{emailgroupId} | Update an email group |


## create_email_group_async

> <EmptyEnvelope> create_email_group_async(tenant_id, email_group_create_dto, opts)

Create an email group

Creates a new email group for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
email_group_create_dto = OpenapiClient::EmailGroupCreateDto.new # EmailGroupCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create an email group
  result = api_instance.create_email_group_async(tenant_id, email_group_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailGroupsApi->create_email_group_async: #{e}"
end
```

#### Using the create_email_group_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_email_group_async_with_http_info(tenant_id, email_group_create_dto, opts)

```ruby
begin
  # Create an email group
  data, status_code, headers = api_instance.create_email_group_async_with_http_info(tenant_id, email_group_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailGroupsApi->create_email_group_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **email_group_create_dto** | [**EmailGroupCreateDto**](EmailGroupCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_email_group_async

> <EmptyEnvelope> delete_email_group_async(tenant_id, emailgroup_id, opts)

Delete an email group

Deletes an email group by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
emailgroup_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an email group
  result = api_instance.delete_email_group_async(tenant_id, emailgroup_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailGroupsApi->delete_email_group_async: #{e}"
end
```

#### Using the delete_email_group_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_email_group_async_with_http_info(tenant_id, emailgroup_id, opts)

```ruby
begin
  # Delete an email group
  data, status_code, headers = api_instance.delete_email_group_async_with_http_info(tenant_id, emailgroup_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailGroupsApi->delete_email_group_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **emailgroup_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_email_group_details_async

> <EmailGroupDtoEnvelope> get_email_group_details_async(tenant_id, emailgroup_id, opts)

Get email group by ID

Retrieves the details of a specific email group by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
emailgroup_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get email group by ID
  result = api_instance.get_email_group_details_async(tenant_id, emailgroup_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailGroupsApi->get_email_group_details_async: #{e}"
end
```

#### Using the get_email_group_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmailGroupDtoEnvelope>, Integer, Hash)> get_email_group_details_async_with_http_info(tenant_id, emailgroup_id, opts)

```ruby
begin
  # Get email group by ID
  data, status_code, headers = api_instance.get_email_group_details_async_with_http_info(tenant_id, emailgroup_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmailGroupDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailGroupsApi->get_email_group_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **emailgroup_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmailGroupDtoEnvelope**](EmailGroupDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_email_groups_count_async

> <Int32Envelope> get_email_groups_count_async(tenant_id, opts)

Get email groups count

Returns the count of email groups for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  email_group_dto_collection_query_parameters: OpenapiClient::EmailGroupDtoCollectionQueryParameters.new # EmailGroupDtoCollectionQueryParameters | 
}

begin
  # Get email groups count
  result = api_instance.get_email_groups_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailGroupsApi->get_email_groups_count_async: #{e}"
end
```

#### Using the get_email_groups_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_email_groups_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get email groups count
  data, status_code, headers = api_instance.get_email_groups_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailGroupsApi->get_email_groups_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **email_group_dto_collection_query_parameters** | [**EmailGroupDtoCollectionQueryParameters**](EmailGroupDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_email_groups_o_data_async

> <EmailGroupDtoListEnvelope> get_email_groups_o_data_async(tenant_id, opts)

Get email groups

Retrieves a collection of email groups for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  email_group_dto_collection_query_parameters: OpenapiClient::EmailGroupDtoCollectionQueryParameters.new # EmailGroupDtoCollectionQueryParameters | 
}

begin
  # Get email groups
  result = api_instance.get_email_groups_o_data_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailGroupsApi->get_email_groups_o_data_async: #{e}"
end
```

#### Using the get_email_groups_o_data_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmailGroupDtoListEnvelope>, Integer, Hash)> get_email_groups_o_data_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get email groups
  data, status_code, headers = api_instance.get_email_groups_o_data_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmailGroupDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailGroupsApi->get_email_groups_o_data_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **email_group_dto_collection_query_parameters** | [**EmailGroupDtoCollectionQueryParameters**](EmailGroupDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**EmailGroupDtoListEnvelope**](EmailGroupDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_email_group_async

> <EmptyEnvelope> patch_email_group_async(tenant_id, emailgroup_id, opts)

Patch an email group

Partially updates an email group by its ID using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
emailgroup_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch an email group
  result = api_instance.patch_email_group_async(tenant_id, emailgroup_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailGroupsApi->patch_email_group_async: #{e}"
end
```

#### Using the patch_email_group_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_email_group_async_with_http_info(tenant_id, emailgroup_id, opts)

```ruby
begin
  # Patch an email group
  data, status_code, headers = api_instance.patch_email_group_async_with_http_info(tenant_id, emailgroup_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailGroupsApi->patch_email_group_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **emailgroup_id** | **String** |  |  |
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


## update_email_group_async

> <EmptyEnvelope> update_email_group_async(tenant_id, emailgroup_id, email_group_update_dto, opts)

Update an email group

Updates an existing email group by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
emailgroup_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
email_group_update_dto = OpenapiClient::EmailGroupUpdateDto.new # EmailGroupUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update an email group
  result = api_instance.update_email_group_async(tenant_id, emailgroup_id, email_group_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailGroupsApi->update_email_group_async: #{e}"
end
```

#### Using the update_email_group_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_email_group_async_with_http_info(tenant_id, emailgroup_id, email_group_update_dto, opts)

```ruby
begin
  # Update an email group
  data, status_code, headers = api_instance.update_email_group_async_with_http_info(tenant_id, emailgroup_id, email_group_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailGroupsApi->update_email_group_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **emailgroup_id** | **String** |  |  |
| **email_group_update_dto** | [**EmailGroupUpdateDto**](EmailGroupUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

