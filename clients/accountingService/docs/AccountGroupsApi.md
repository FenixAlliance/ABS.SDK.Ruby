# OpenapiClient::AccountGroupsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_account_group**](AccountGroupsApi.md#create_account_group) | **POST** /api/v2/AccountingService/AccountGroups | Creates a new account group |
| [**delete_account_group**](AccountGroupsApi.md#delete_account_group) | **DELETE** /api/v2/AccountingService/AccountGroups/{accountGroupId} | Deletes an existing account group |
| [**get_account_group**](AccountGroupsApi.md#get_account_group) | **GET** /api/v2/AccountingService/AccountGroups/{accountGroupId} | Gets the current tenant account group |
| [**get_account_groups**](AccountGroupsApi.md#get_account_groups) | **GET** /api/v2/AccountingService/AccountGroups | Gets the current tenant account groups |
| [**get_account_groups_count_async**](AccountGroupsApi.md#get_account_groups_count_async) | **GET** /api/v2/AccountingService/AccountGroups/Count | Gets the current tenant accounts count |
| [**update_account_group**](AccountGroupsApi.md#update_account_group) | **PUT** /api/v2/AccountingService/AccountGroups/{accountGroupId} | Updates an existing account group |


## create_account_group

> <AccountGroupDtoEnvelope> create_account_group(tenant_id, opts)

Creates a new account group

Creates a new account group.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  account_group_create_dto: OpenapiClient::AccountGroupCreateDto.new # AccountGroupCreateDto | 
}

begin
  # Creates a new account group
  result = api_instance.create_account_group(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountGroupsApi->create_account_group: #{e}"
end
```

#### Using the create_account_group_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountGroupDtoEnvelope>, Integer, Hash)> create_account_group_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new account group
  data, status_code, headers = api_instance.create_account_group_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountGroupDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountGroupsApi->create_account_group_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **account_group_create_dto** | [**AccountGroupCreateDto**](AccountGroupCreateDto.md) |  | [optional] |

### Return type

[**AccountGroupDtoEnvelope**](AccountGroupDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_account_group

> delete_account_group(tenant_id, account_group_id, opts)

Deletes an existing account group

Deletes an existing account group.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes an existing account group
  api_instance.delete_account_group(tenant_id, account_group_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountGroupsApi->delete_account_group: #{e}"
end
```

#### Using the delete_account_group_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_account_group_with_http_info(tenant_id, account_group_id, opts)

```ruby
begin
  # Deletes an existing account group
  data, status_code, headers = api_instance.delete_account_group_with_http_info(tenant_id, account_group_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountGroupsApi->delete_account_group_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_group_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_account_group

> <AccountGroupDtoEnvelope> get_account_group(tenant_id, account_group_id, opts)

Gets the current tenant account group

Get the currently acting tenant account group.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant account group
  result = api_instance.get_account_group(tenant_id, account_group_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountGroupsApi->get_account_group: #{e}"
end
```

#### Using the get_account_group_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountGroupDtoEnvelope>, Integer, Hash)> get_account_group_with_http_info(tenant_id, account_group_id, opts)

```ruby
begin
  # Gets the current tenant account group
  data, status_code, headers = api_instance.get_account_group_with_http_info(tenant_id, account_group_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountGroupDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountGroupsApi->get_account_group_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_group_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**AccountGroupDtoEnvelope**](AccountGroupDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_account_groups

> <AccountGroupDtoListEnvelope> get_account_groups(tenant_id, opts)

Gets the current tenant account groups

Get the currently acting tenant account groups.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant account groups
  result = api_instance.get_account_groups(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountGroupsApi->get_account_groups: #{e}"
end
```

#### Using the get_account_groups_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountGroupDtoListEnvelope>, Integer, Hash)> get_account_groups_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets the current tenant account groups
  data, status_code, headers = api_instance.get_account_groups_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountGroupDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountGroupsApi->get_account_groups_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**AccountGroupDtoListEnvelope**](AccountGroupDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_account_groups_count_async

> <Int32Envelope> get_account_groups_count_async(tenant_id, opts)

Gets the current tenant accounts count

Get the currently acting tenant accounts count.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant accounts count
  result = api_instance.get_account_groups_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountGroupsApi->get_account_groups_count_async: #{e}"
end
```

#### Using the get_account_groups_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_account_groups_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets the current tenant accounts count
  data, status_code, headers = api_instance.get_account_groups_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountGroupsApi->get_account_groups_count_async_with_http_info: #{e}"
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


## update_account_group

> <AccountGroupDtoEnvelope> update_account_group(tenant_id, account_group_id, opts)

Updates an existing account group

Updates an existing account group.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  account_group_update_dto: OpenapiClient::AccountGroupUpdateDto.new # AccountGroupUpdateDto | 
}

begin
  # Updates an existing account group
  result = api_instance.update_account_group(tenant_id, account_group_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountGroupsApi->update_account_group: #{e}"
end
```

#### Using the update_account_group_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountGroupDtoEnvelope>, Integer, Hash)> update_account_group_with_http_info(tenant_id, account_group_id, opts)

```ruby
begin
  # Updates an existing account group
  data, status_code, headers = api_instance.update_account_group_with_http_info(tenant_id, account_group_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountGroupDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountGroupsApi->update_account_group_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_group_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **account_group_update_dto** | [**AccountGroupUpdateDto**](AccountGroupUpdateDto.md) |  | [optional] |

### Return type

[**AccountGroupDtoEnvelope**](AccountGroupDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

