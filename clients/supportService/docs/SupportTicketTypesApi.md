# OpenapiClient::SupportTicketTypesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_support_ticket_type_async**](SupportTicketTypesApi.md#create_support_ticket_type_async) | **POST** /api/v2/SupportService/SupportTicketTypes | Create a new support ticket type |
| [**delete_support_ticket_type_async**](SupportTicketTypesApi.md#delete_support_ticket_type_async) | **DELETE** /api/v2/SupportService/SupportTicketTypes/{supportTicketTypeId} | Delete a support ticket type |
| [**get_support_ticket_type_async**](SupportTicketTypesApi.md#get_support_ticket_type_async) | **GET** /api/v2/SupportService/SupportTicketTypes/{supportTicketTypeId} | Retrieve a support ticket type by ID |
| [**get_support_ticket_types_async**](SupportTicketTypesApi.md#get_support_ticket_types_async) | **GET** /api/v2/SupportService/SupportTicketTypes | Retrieve a list of support ticket types |
| [**get_support_ticket_types_count_async**](SupportTicketTypesApi.md#get_support_ticket_types_count_async) | **GET** /api/v2/SupportService/SupportTicketTypes/Count | Get the count of support ticket types |
| [**update_support_ticket_type_async**](SupportTicketTypesApi.md#update_support_ticket_type_async) | **PUT** /api/v2/SupportService/SupportTicketTypes/{supportTicketTypeId} | Update a support ticket type |


## create_support_ticket_type_async

> <EmptyEnvelope> create_support_ticket_type_async(tenant_id, opts)

Create a new support ticket type

Creates a new support ticket type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  support_ticket_type_create_dto: OpenapiClient::SupportTicketTypeCreateDto.new # SupportTicketTypeCreateDto | 
}

begin
  # Create a new support ticket type
  result = api_instance.create_support_ticket_type_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketTypesApi->create_support_ticket_type_async: #{e}"
end
```

#### Using the create_support_ticket_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_support_ticket_type_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new support ticket type
  data, status_code, headers = api_instance.create_support_ticket_type_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketTypesApi->create_support_ticket_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **support_ticket_type_create_dto** | [**SupportTicketTypeCreateDto**](SupportTicketTypeCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_support_ticket_type_async

> <EmptyEnvelope> delete_support_ticket_type_async(tenant_id, support_ticket_type_id, opts)

Delete a support ticket type

Deletes a support ticket type by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_ticket_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a support ticket type
  result = api_instance.delete_support_ticket_type_async(tenant_id, support_ticket_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketTypesApi->delete_support_ticket_type_async: #{e}"
end
```

#### Using the delete_support_ticket_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_support_ticket_type_async_with_http_info(tenant_id, support_ticket_type_id, opts)

```ruby
begin
  # Delete a support ticket type
  data, status_code, headers = api_instance.delete_support_ticket_type_async_with_http_info(tenant_id, support_ticket_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketTypesApi->delete_support_ticket_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_ticket_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_ticket_type_async

> <SupportTicketTypeDtoEnvelope> get_support_ticket_type_async(tenant_id, support_ticket_type_id, opts)

Retrieve a support ticket type by ID

Retrieves a single support ticket type by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_ticket_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a support ticket type by ID
  result = api_instance.get_support_ticket_type_async(tenant_id, support_ticket_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketTypesApi->get_support_ticket_type_async: #{e}"
end
```

#### Using the get_support_ticket_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SupportTicketTypeDtoEnvelope>, Integer, Hash)> get_support_ticket_type_async_with_http_info(tenant_id, support_ticket_type_id, opts)

```ruby
begin
  # Retrieve a support ticket type by ID
  data, status_code, headers = api_instance.get_support_ticket_type_async_with_http_info(tenant_id, support_ticket_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SupportTicketTypeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketTypesApi->get_support_ticket_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_ticket_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SupportTicketTypeDtoEnvelope**](SupportTicketTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_ticket_types_async

> <SupportTicketTypeDtoListEnvelope> get_support_ticket_types_async(tenant_id, opts)

Retrieve a list of support ticket types

Retrieves a list of support ticket types for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of support ticket types
  result = api_instance.get_support_ticket_types_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketTypesApi->get_support_ticket_types_async: #{e}"
end
```

#### Using the get_support_ticket_types_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SupportTicketTypeDtoListEnvelope>, Integer, Hash)> get_support_ticket_types_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of support ticket types
  data, status_code, headers = api_instance.get_support_ticket_types_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SupportTicketTypeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketTypesApi->get_support_ticket_types_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SupportTicketTypeDtoListEnvelope**](SupportTicketTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_ticket_types_count_async

> <Int32Envelope> get_support_ticket_types_count_async(tenant_id, opts)

Get the count of support ticket types

Returns the total count of support ticket types for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of support ticket types
  result = api_instance.get_support_ticket_types_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketTypesApi->get_support_ticket_types_count_async: #{e}"
end
```

#### Using the get_support_ticket_types_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_support_ticket_types_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of support ticket types
  data, status_code, headers = api_instance.get_support_ticket_types_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketTypesApi->get_support_ticket_types_count_async_with_http_info: #{e}"
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


## update_support_ticket_type_async

> <EmptyEnvelope> update_support_ticket_type_async(tenant_id, support_ticket_type_id, opts)

Update a support ticket type

Updates an existing support ticket type by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_ticket_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  support_ticket_type_update_dto: OpenapiClient::SupportTicketTypeUpdateDto.new # SupportTicketTypeUpdateDto | 
}

begin
  # Update a support ticket type
  result = api_instance.update_support_ticket_type_async(tenant_id, support_ticket_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketTypesApi->update_support_ticket_type_async: #{e}"
end
```

#### Using the update_support_ticket_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_support_ticket_type_async_with_http_info(tenant_id, support_ticket_type_id, opts)

```ruby
begin
  # Update a support ticket type
  data, status_code, headers = api_instance.update_support_ticket_type_async_with_http_info(tenant_id, support_ticket_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketTypesApi->update_support_ticket_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_ticket_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **support_ticket_type_update_dto** | [**SupportTicketTypeUpdateDto**](SupportTicketTypeUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

