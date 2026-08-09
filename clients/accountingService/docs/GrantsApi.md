# OpenapiClient::GrantsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_grant_async**](GrantsApi.md#create_grant_async) | **POST** /api/v2/AccountingService/Grants | Create grant |
| [**delete_grant_async**](GrantsApi.md#delete_grant_async) | **DELETE** /api/v2/AccountingService/Grants/{grantId} | Delete grant |
| [**get_grant_details_async**](GrantsApi.md#get_grant_details_async) | **GET** /api/v2/AccountingService/Grants/{grantId} | Get grant by ID |
| [**get_grants_async**](GrantsApi.md#get_grants_async) | **GET** /api/v2/AccountingService/Grants | Get all grants |
| [**get_grants_count_async**](GrantsApi.md#get_grants_count_async) | **GET** /api/v2/AccountingService/Grants/Count | Count grants |
| [**patch_grant_async**](GrantsApi.md#patch_grant_async) | **PATCH** /api/v2/AccountingService/Grants/{grantId} | Patch a grant |
| [**update_grant_async**](GrantsApi.md#update_grant_async) | **PUT** /api/v2/AccountingService/Grants/{grantId} | Update grant |


## create_grant_async

> <EmptyEnvelope> create_grant_async(tenant_id, opts)

Create grant

Creates a new grant entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GrantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  grant_create_dto: OpenapiClient::GrantCreateDto.new # GrantCreateDto | 
}

begin
  # Create grant
  result = api_instance.create_grant_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GrantsApi->create_grant_async: #{e}"
end
```

#### Using the create_grant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_grant_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create grant
  data, status_code, headers = api_instance.create_grant_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GrantsApi->create_grant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **grant_create_dto** | [**GrantCreateDto**](GrantCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_grant_async

> <EmptyEnvelope> delete_grant_async(tenant_id, grant_id, opts)

Delete grant

Deletes a grant identified by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GrantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
grant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete grant
  result = api_instance.delete_grant_async(tenant_id, grant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GrantsApi->delete_grant_async: #{e}"
end
```

#### Using the delete_grant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_grant_async_with_http_info(tenant_id, grant_id, opts)

```ruby
begin
  # Delete grant
  data, status_code, headers = api_instance.delete_grant_async_with_http_info(tenant_id, grant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GrantsApi->delete_grant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **grant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_grant_details_async

> <GrantDtoEnvelope> get_grant_details_async(tenant_id, grant_id, opts)

Get grant by ID

Gets detailed information for a specific grant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GrantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
grant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get grant by ID
  result = api_instance.get_grant_details_async(tenant_id, grant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GrantsApi->get_grant_details_async: #{e}"
end
```

#### Using the get_grant_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<GrantDtoEnvelope>, Integer, Hash)> get_grant_details_async_with_http_info(tenant_id, grant_id, opts)

```ruby
begin
  # Get grant by ID
  data, status_code, headers = api_instance.get_grant_details_async_with_http_info(tenant_id, grant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <GrantDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GrantsApi->get_grant_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **grant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**GrantDtoEnvelope**](GrantDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_grants_async

> <GrantDtoIReadOnlyListEnvelope> get_grants_async(tenant_id, opts)

Get all grants

Retrieves a list of grants associated with the tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GrantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  grant_dto_collection_query_parameters: OpenapiClient::GrantDtoCollectionQueryParameters.new # GrantDtoCollectionQueryParameters | 
}

begin
  # Get all grants
  result = api_instance.get_grants_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GrantsApi->get_grants_async: #{e}"
end
```

#### Using the get_grants_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<GrantDtoIReadOnlyListEnvelope>, Integer, Hash)> get_grants_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all grants
  data, status_code, headers = api_instance.get_grants_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <GrantDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GrantsApi->get_grants_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **grant_dto_collection_query_parameters** | [**GrantDtoCollectionQueryParameters**](GrantDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**GrantDtoIReadOnlyListEnvelope**](GrantDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_grants_count_async

> <Int32Envelope> get_grants_count_async(tenant_id, opts)

Count grants

Returns the number of grants for the tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GrantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  grant_dto_collection_query_parameters: OpenapiClient::GrantDtoCollectionQueryParameters.new # GrantDtoCollectionQueryParameters | 
}

begin
  # Count grants
  result = api_instance.get_grants_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GrantsApi->get_grants_count_async: #{e}"
end
```

#### Using the get_grants_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_grants_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count grants
  data, status_code, headers = api_instance.get_grants_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GrantsApi->get_grants_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **grant_dto_collection_query_parameters** | [**GrantDtoCollectionQueryParameters**](GrantDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_grant_async

> <EmptyEnvelope> patch_grant_async(tenant_id, grant_id, opts)

Patch a grant

Partially updates a grant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GrantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
grant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a grant
  result = api_instance.patch_grant_async(tenant_id, grant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GrantsApi->patch_grant_async: #{e}"
end
```

#### Using the patch_grant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_grant_async_with_http_info(tenant_id, grant_id, opts)

```ruby
begin
  # Patch a grant
  data, status_code, headers = api_instance.patch_grant_async_with_http_info(tenant_id, grant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GrantsApi->patch_grant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **grant_id** | **String** |  |  |
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


## update_grant_async

> <EmptyEnvelope> update_grant_async(tenant_id, grant_id, opts)

Update grant

Updates an existing grant identified by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GrantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
grant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  body: { ... } # Object | 
}

begin
  # Update grant
  result = api_instance.update_grant_async(tenant_id, grant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GrantsApi->update_grant_async: #{e}"
end
```

#### Using the update_grant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_grant_async_with_http_info(tenant_id, grant_id, opts)

```ruby
begin
  # Update grant
  data, status_code, headers = api_instance.update_grant_async_with_http_info(tenant_id, grant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GrantsApi->update_grant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **grant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **body** | **Object** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

