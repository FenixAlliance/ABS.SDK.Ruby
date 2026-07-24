# OpenapiClient::BusinessRelationshipsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_business_relationship_async**](BusinessRelationshipsApi.md#create_business_relationship_async) | **POST** /api/v2/TenantsService/BusinessRelationships | Create a business relationship |
| [**delete_business_relationship_async**](BusinessRelationshipsApi.md#delete_business_relationship_async) | **DELETE** /api/v2/TenantsService/BusinessRelationships/{businessRelationshipId} | Delete a business relationship |
| [**get_business_relationship_by_id_async**](BusinessRelationshipsApi.md#get_business_relationship_by_id_async) | **GET** /api/v2/TenantsService/BusinessRelationships/{businessRelationshipId} | Get business relationship by ID |
| [**get_business_relationships_async**](BusinessRelationshipsApi.md#get_business_relationships_async) | **GET** /api/v2/TenantsService/BusinessRelationships | Get business relationships |
| [**get_business_relationships_count_async**](BusinessRelationshipsApi.md#get_business_relationships_count_async) | **GET** /api/v2/TenantsService/BusinessRelationships/Count | Get business relationships count |
| [**update_business_relationship_async**](BusinessRelationshipsApi.md#update_business_relationship_async) | **PUT** /api/v2/TenantsService/BusinessRelationships/{businessRelationshipId} | Update a business relationship |


## create_business_relationship_async

> <EmptyEnvelope> create_business_relationship_async(tenant_id, business_relationship_create_dto, opts)

Create a business relationship

Creates a new business relationship owned by the specified parent tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BusinessRelationshipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
business_relationship_create_dto = OpenapiClient::BusinessRelationshipCreateDto.new # BusinessRelationshipCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a business relationship
  result = api_instance.create_business_relationship_async(tenant_id, business_relationship_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessRelationshipsApi->create_business_relationship_async: #{e}"
end
```

#### Using the create_business_relationship_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_business_relationship_async_with_http_info(tenant_id, business_relationship_create_dto, opts)

```ruby
begin
  # Create a business relationship
  data, status_code, headers = api_instance.create_business_relationship_async_with_http_info(tenant_id, business_relationship_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessRelationshipsApi->create_business_relationship_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **business_relationship_create_dto** | [**BusinessRelationshipCreateDto**](BusinessRelationshipCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_business_relationship_async

> <EmptyEnvelope> delete_business_relationship_async(tenant_id, business_relationship_id, opts)

Delete a business relationship

Deletes a business relationship by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BusinessRelationshipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
business_relationship_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a business relationship
  result = api_instance.delete_business_relationship_async(tenant_id, business_relationship_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessRelationshipsApi->delete_business_relationship_async: #{e}"
end
```

#### Using the delete_business_relationship_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_business_relationship_async_with_http_info(tenant_id, business_relationship_id, opts)

```ruby
begin
  # Delete a business relationship
  data, status_code, headers = api_instance.delete_business_relationship_async_with_http_info(tenant_id, business_relationship_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessRelationshipsApi->delete_business_relationship_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **business_relationship_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_business_relationship_by_id_async

> <BusinessRelationshipDtoEnvelope> get_business_relationship_by_id_async(tenant_id, business_relationship_id, opts)

Get business relationship by ID

Retrieves the details of a specific business relationship by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BusinessRelationshipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
business_relationship_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get business relationship by ID
  result = api_instance.get_business_relationship_by_id_async(tenant_id, business_relationship_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessRelationshipsApi->get_business_relationship_by_id_async: #{e}"
end
```

#### Using the get_business_relationship_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BusinessRelationshipDtoEnvelope>, Integer, Hash)> get_business_relationship_by_id_async_with_http_info(tenant_id, business_relationship_id, opts)

```ruby
begin
  # Get business relationship by ID
  data, status_code, headers = api_instance.get_business_relationship_by_id_async_with_http_info(tenant_id, business_relationship_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BusinessRelationshipDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessRelationshipsApi->get_business_relationship_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **business_relationship_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BusinessRelationshipDtoEnvelope**](BusinessRelationshipDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_business_relationships_async

> <BusinessRelationshipDtoListEnvelope> get_business_relationships_async(tenant_id, opts)

Get business relationships

Retrieves the child business relationships owned by the specified parent tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BusinessRelationshipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get business relationships
  result = api_instance.get_business_relationships_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessRelationshipsApi->get_business_relationships_async: #{e}"
end
```

#### Using the get_business_relationships_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BusinessRelationshipDtoListEnvelope>, Integer, Hash)> get_business_relationships_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get business relationships
  data, status_code, headers = api_instance.get_business_relationships_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BusinessRelationshipDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessRelationshipsApi->get_business_relationships_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BusinessRelationshipDtoListEnvelope**](BusinessRelationshipDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_business_relationships_count_async

> <Int32Envelope> get_business_relationships_count_async(tenant_id, opts)

Get business relationships count

Returns the count of child business relationships owned by the specified parent tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BusinessRelationshipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get business relationships count
  result = api_instance.get_business_relationships_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessRelationshipsApi->get_business_relationships_count_async: #{e}"
end
```

#### Using the get_business_relationships_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_business_relationships_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get business relationships count
  data, status_code, headers = api_instance.get_business_relationships_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessRelationshipsApi->get_business_relationships_count_async_with_http_info: #{e}"
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


## update_business_relationship_async

> <EmptyEnvelope> update_business_relationship_async(tenant_id, business_relationship_id, business_relationship_update_dto, opts)

Update a business relationship

Updates an existing business relationship by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BusinessRelationshipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
business_relationship_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
business_relationship_update_dto = OpenapiClient::BusinessRelationshipUpdateDto.new # BusinessRelationshipUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update a business relationship
  result = api_instance.update_business_relationship_async(tenant_id, business_relationship_id, business_relationship_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessRelationshipsApi->update_business_relationship_async: #{e}"
end
```

#### Using the update_business_relationship_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_business_relationship_async_with_http_info(tenant_id, business_relationship_id, business_relationship_update_dto, opts)

```ruby
begin
  # Update a business relationship
  data, status_code, headers = api_instance.update_business_relationship_async_with_http_info(tenant_id, business_relationship_id, business_relationship_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessRelationshipsApi->update_business_relationship_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **business_relationship_id** | **String** |  |  |
| **business_relationship_update_dto** | [**BusinessRelationshipUpdateDto**](BusinessRelationshipUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

