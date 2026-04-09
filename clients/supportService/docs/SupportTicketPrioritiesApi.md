# OpenapiClient::SupportTicketPrioritiesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_support_ticket_priority_async**](SupportTicketPrioritiesApi.md#create_support_ticket_priority_async) | **POST** /api/v2/SupportService/SupportTicketPriorities | Create a new support ticket priority |
| [**delete_support_ticket_priority_async**](SupportTicketPrioritiesApi.md#delete_support_ticket_priority_async) | **DELETE** /api/v2/SupportService/SupportTicketPriorities/{supportTicketPriorityId} | Delete a support ticket priority |
| [**get_support_ticket_priorities_async**](SupportTicketPrioritiesApi.md#get_support_ticket_priorities_async) | **GET** /api/v2/SupportService/SupportTicketPriorities | Retrieve a list of support ticket priorities |
| [**get_support_ticket_priorities_count_async**](SupportTicketPrioritiesApi.md#get_support_ticket_priorities_count_async) | **GET** /api/v2/SupportService/SupportTicketPriorities/Count | Get the count of support ticket priorities |
| [**get_support_ticket_priority_async**](SupportTicketPrioritiesApi.md#get_support_ticket_priority_async) | **GET** /api/v2/SupportService/SupportTicketPriorities/{supportTicketPriorityId} | Retrieve a support ticket priority by ID |
| [**update_support_ticket_priority_async**](SupportTicketPrioritiesApi.md#update_support_ticket_priority_async) | **PUT** /api/v2/SupportService/SupportTicketPriorities/{supportTicketPriorityId} | Update a support ticket priority |


## create_support_ticket_priority_async

> <EmptyEnvelope> create_support_ticket_priority_async(tenant_id, opts)

Create a new support ticket priority

Creates a new support ticket priority for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketPrioritiesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  support_ticket_priority_create_dto: OpenapiClient::SupportTicketPriorityCreateDto.new # SupportTicketPriorityCreateDto | 
}

begin
  # Create a new support ticket priority
  result = api_instance.create_support_ticket_priority_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketPrioritiesApi->create_support_ticket_priority_async: #{e}"
end
```

#### Using the create_support_ticket_priority_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_support_ticket_priority_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new support ticket priority
  data, status_code, headers = api_instance.create_support_ticket_priority_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketPrioritiesApi->create_support_ticket_priority_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **support_ticket_priority_create_dto** | [**SupportTicketPriorityCreateDto**](SupportTicketPriorityCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_support_ticket_priority_async

> <EmptyEnvelope> delete_support_ticket_priority_async(tenant_id, support_ticket_priority_id, opts)

Delete a support ticket priority

Deletes a support ticket priority by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketPrioritiesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_ticket_priority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a support ticket priority
  result = api_instance.delete_support_ticket_priority_async(tenant_id, support_ticket_priority_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketPrioritiesApi->delete_support_ticket_priority_async: #{e}"
end
```

#### Using the delete_support_ticket_priority_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_support_ticket_priority_async_with_http_info(tenant_id, support_ticket_priority_id, opts)

```ruby
begin
  # Delete a support ticket priority
  data, status_code, headers = api_instance.delete_support_ticket_priority_async_with_http_info(tenant_id, support_ticket_priority_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketPrioritiesApi->delete_support_ticket_priority_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_ticket_priority_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_ticket_priorities_async

> <SupportTicketPriorityDtoListEnvelope> get_support_ticket_priorities_async(tenant_id, opts)

Retrieve a list of support ticket priorities

Retrieves a list of support ticket priorities for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketPrioritiesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of support ticket priorities
  result = api_instance.get_support_ticket_priorities_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketPrioritiesApi->get_support_ticket_priorities_async: #{e}"
end
```

#### Using the get_support_ticket_priorities_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SupportTicketPriorityDtoListEnvelope>, Integer, Hash)> get_support_ticket_priorities_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of support ticket priorities
  data, status_code, headers = api_instance.get_support_ticket_priorities_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SupportTicketPriorityDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketPrioritiesApi->get_support_ticket_priorities_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SupportTicketPriorityDtoListEnvelope**](SupportTicketPriorityDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_ticket_priorities_count_async

> <Int32Envelope> get_support_ticket_priorities_count_async(tenant_id, opts)

Get the count of support ticket priorities

Returns the total count of support ticket priorities for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketPrioritiesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of support ticket priorities
  result = api_instance.get_support_ticket_priorities_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketPrioritiesApi->get_support_ticket_priorities_count_async: #{e}"
end
```

#### Using the get_support_ticket_priorities_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_support_ticket_priorities_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of support ticket priorities
  data, status_code, headers = api_instance.get_support_ticket_priorities_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketPrioritiesApi->get_support_ticket_priorities_count_async_with_http_info: #{e}"
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


## get_support_ticket_priority_async

> <SupportTicketPriorityDtoEnvelope> get_support_ticket_priority_async(tenant_id, support_ticket_priority_id, opts)

Retrieve a support ticket priority by ID

Retrieves a single support ticket priority by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketPrioritiesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_ticket_priority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a support ticket priority by ID
  result = api_instance.get_support_ticket_priority_async(tenant_id, support_ticket_priority_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketPrioritiesApi->get_support_ticket_priority_async: #{e}"
end
```

#### Using the get_support_ticket_priority_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SupportTicketPriorityDtoEnvelope>, Integer, Hash)> get_support_ticket_priority_async_with_http_info(tenant_id, support_ticket_priority_id, opts)

```ruby
begin
  # Retrieve a support ticket priority by ID
  data, status_code, headers = api_instance.get_support_ticket_priority_async_with_http_info(tenant_id, support_ticket_priority_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SupportTicketPriorityDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketPrioritiesApi->get_support_ticket_priority_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_ticket_priority_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SupportTicketPriorityDtoEnvelope**](SupportTicketPriorityDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_support_ticket_priority_async

> <EmptyEnvelope> update_support_ticket_priority_async(tenant_id, support_ticket_priority_id, opts)

Update a support ticket priority

Updates an existing support ticket priority by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketPrioritiesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_ticket_priority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  support_ticket_priority_update_dto: OpenapiClient::SupportTicketPriorityUpdateDto.new # SupportTicketPriorityUpdateDto | 
}

begin
  # Update a support ticket priority
  result = api_instance.update_support_ticket_priority_async(tenant_id, support_ticket_priority_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketPrioritiesApi->update_support_ticket_priority_async: #{e}"
end
```

#### Using the update_support_ticket_priority_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_support_ticket_priority_async_with_http_info(tenant_id, support_ticket_priority_id, opts)

```ruby
begin
  # Update a support ticket priority
  data, status_code, headers = api_instance.update_support_ticket_priority_async_with_http_info(tenant_id, support_ticket_priority_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketPrioritiesApi->update_support_ticket_priority_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_ticket_priority_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **support_ticket_priority_update_dto** | [**SupportTicketPriorityUpdateDto**](SupportTicketPriorityUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

