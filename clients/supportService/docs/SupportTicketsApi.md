# OpenapiClient::SupportTicketsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_support_ticket_async**](SupportTicketsApi.md#create_support_ticket_async) | **POST** /api/v2/SupportService/SupportTickets | Create a new support ticket |
| [**delete_support_ticket_async**](SupportTicketsApi.md#delete_support_ticket_async) | **DELETE** /api/v2/SupportService/SupportTickets/{supportTicketId} | Delete a support ticket |
| [**delete_support_ticket_conversation_async**](SupportTicketsApi.md#delete_support_ticket_conversation_async) | **DELETE** /api/v2/SupportService/SupportTickets/{supportTicketId}/Conversations/{supportTicketConversationId} | Delete a conversation from a support ticket |
| [**get_support_ticket_async**](SupportTicketsApi.md#get_support_ticket_async) | **GET** /api/v2/SupportService/SupportTickets/{supportTicketId} | Retrieve a support ticket by ID |
| [**get_support_ticket_conversation_async**](SupportTicketsApi.md#get_support_ticket_conversation_async) | **GET** /api/v2/SupportService/SupportTickets/{supportTicketId}/Conversations/{supportTicketConversationId} | Retrieve a specific conversation for a support ticket |
| [**get_support_ticket_conversation_messages_async**](SupportTicketsApi.md#get_support_ticket_conversation_messages_async) | **GET** /api/v2/SupportService/SupportTickets/{supportTicketId}/Conversations/{supportTicketConversationId}/Messages | Retrieve messages for a support ticket conversation |
| [**get_support_ticket_conversations_async**](SupportTicketsApi.md#get_support_ticket_conversations_async) | **GET** /api/v2/SupportService/SupportTickets/{supportTicketId}/Conversations | Retrieve conversations for a support ticket |
| [**get_support_tickets_async**](SupportTicketsApi.md#get_support_tickets_async) | **GET** /api/v2/SupportService/SupportTickets | Retrieve a list of support tickets |
| [**get_support_tickets_count_async**](SupportTicketsApi.md#get_support_tickets_count_async) | **GET** /api/v2/SupportService/SupportTickets/Count | Get the count of support tickets |
| [**patch_support_ticket_async**](SupportTicketsApi.md#patch_support_ticket_async) | **PATCH** /api/v2/SupportService/SupportTickets/{supportTicketId} | Patch a support ticket |
| [**relate_support_ticket_to_conversation_async**](SupportTicketsApi.md#relate_support_ticket_to_conversation_async) | **POST** /api/v2/SupportService/SupportTickets/{supportTicketId}/Conversations | Create a conversation for a support ticket |
| [**update_support_ticket_async**](SupportTicketsApi.md#update_support_ticket_async) | **PUT** /api/v2/SupportService/SupportTickets/{supportTicketId} | Update a support ticket |


## create_support_ticket_async

> <EmptyEnvelope> create_support_ticket_async(tenant_id, opts)

Create a new support ticket

Creates a new support ticket for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  support_ticket_create_dto: OpenapiClient::SupportTicketCreateDto.new # SupportTicketCreateDto | 
}

begin
  # Create a new support ticket
  result = api_instance.create_support_ticket_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->create_support_ticket_async: #{e}"
end
```

#### Using the create_support_ticket_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_support_ticket_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new support ticket
  data, status_code, headers = api_instance.create_support_ticket_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->create_support_ticket_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **support_ticket_create_dto** | [**SupportTicketCreateDto**](SupportTicketCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_support_ticket_async

> <EmptyEnvelope> delete_support_ticket_async(tenant_id, support_ticket_id, opts)

Delete a support ticket

Deletes a support ticket by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_ticket_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a support ticket
  result = api_instance.delete_support_ticket_async(tenant_id, support_ticket_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->delete_support_ticket_async: #{e}"
end
```

#### Using the delete_support_ticket_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_support_ticket_async_with_http_info(tenant_id, support_ticket_id, opts)

```ruby
begin
  # Delete a support ticket
  data, status_code, headers = api_instance.delete_support_ticket_async_with_http_info(tenant_id, support_ticket_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->delete_support_ticket_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_ticket_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_support_ticket_conversation_async

> <EmptyEnvelope> delete_support_ticket_conversation_async(tenant_id, support_ticket_id, support_ticket_conversation_id, opts)

Delete a conversation from a support ticket

Deletes a specific conversation from a support ticket.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_ticket_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_ticket_conversation_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a conversation from a support ticket
  result = api_instance.delete_support_ticket_conversation_async(tenant_id, support_ticket_id, support_ticket_conversation_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->delete_support_ticket_conversation_async: #{e}"
end
```

#### Using the delete_support_ticket_conversation_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_support_ticket_conversation_async_with_http_info(tenant_id, support_ticket_id, support_ticket_conversation_id, opts)

```ruby
begin
  # Delete a conversation from a support ticket
  data, status_code, headers = api_instance.delete_support_ticket_conversation_async_with_http_info(tenant_id, support_ticket_id, support_ticket_conversation_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->delete_support_ticket_conversation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_ticket_id** | **String** |  |  |
| **support_ticket_conversation_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_ticket_async

> <SupportTicketDtoEnvelope> get_support_ticket_async(tenant_id, support_ticket_id, opts)

Retrieve a support ticket by ID

Retrieves a single support ticket by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_ticket_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a support ticket by ID
  result = api_instance.get_support_ticket_async(tenant_id, support_ticket_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->get_support_ticket_async: #{e}"
end
```

#### Using the get_support_ticket_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SupportTicketDtoEnvelope>, Integer, Hash)> get_support_ticket_async_with_http_info(tenant_id, support_ticket_id, opts)

```ruby
begin
  # Retrieve a support ticket by ID
  data, status_code, headers = api_instance.get_support_ticket_async_with_http_info(tenant_id, support_ticket_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SupportTicketDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->get_support_ticket_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_ticket_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SupportTicketDtoEnvelope**](SupportTicketDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_ticket_conversation_async

> <SupportTicketConversationDtoEnvelope> get_support_ticket_conversation_async(tenant_id, support_ticket_id, support_ticket_conversation_id, opts)

Retrieve a specific conversation for a support ticket

Retrieves a single conversation by its ID for a specific support ticket.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_ticket_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_ticket_conversation_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a specific conversation for a support ticket
  result = api_instance.get_support_ticket_conversation_async(tenant_id, support_ticket_id, support_ticket_conversation_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->get_support_ticket_conversation_async: #{e}"
end
```

#### Using the get_support_ticket_conversation_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SupportTicketConversationDtoEnvelope>, Integer, Hash)> get_support_ticket_conversation_async_with_http_info(tenant_id, support_ticket_id, support_ticket_conversation_id, opts)

```ruby
begin
  # Retrieve a specific conversation for a support ticket
  data, status_code, headers = api_instance.get_support_ticket_conversation_async_with_http_info(tenant_id, support_ticket_id, support_ticket_conversation_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SupportTicketConversationDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->get_support_ticket_conversation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_ticket_id** | **String** |  |  |
| **support_ticket_conversation_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SupportTicketConversationDtoEnvelope**](SupportTicketConversationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_ticket_conversation_messages_async

> <PrivateMessageDtoListEnvelope> get_support_ticket_conversation_messages_async(tenant_id, support_ticket_id, support_ticket_conversation_id, opts)

Retrieve messages for a support ticket conversation

Retrieves the list of messages within a specific conversation of a support ticket.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_ticket_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_ticket_conversation_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  page_number: 56, # Integer | 
  page_size: 56, # Integer | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve messages for a support ticket conversation
  result = api_instance.get_support_ticket_conversation_messages_async(tenant_id, support_ticket_id, support_ticket_conversation_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->get_support_ticket_conversation_messages_async: #{e}"
end
```

#### Using the get_support_ticket_conversation_messages_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PrivateMessageDtoListEnvelope>, Integer, Hash)> get_support_ticket_conversation_messages_async_with_http_info(tenant_id, support_ticket_id, support_ticket_conversation_id, opts)

```ruby
begin
  # Retrieve messages for a support ticket conversation
  data, status_code, headers = api_instance.get_support_ticket_conversation_messages_async_with_http_info(tenant_id, support_ticket_id, support_ticket_conversation_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PrivateMessageDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->get_support_ticket_conversation_messages_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_ticket_id** | **String** |  |  |
| **support_ticket_conversation_id** | **String** |  |  |
| **page_number** | **Integer** |  | [optional] |
| **page_size** | **Integer** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PrivateMessageDtoListEnvelope**](PrivateMessageDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_ticket_conversations_async

> <SupportTicketConversationDtoListEnvelope> get_support_ticket_conversations_async(tenant_id, support_ticket_id, opts)

Retrieve conversations for a support ticket

Retrieves the list of conversations associated with a specific support ticket.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_ticket_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve conversations for a support ticket
  result = api_instance.get_support_ticket_conversations_async(tenant_id, support_ticket_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->get_support_ticket_conversations_async: #{e}"
end
```

#### Using the get_support_ticket_conversations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SupportTicketConversationDtoListEnvelope>, Integer, Hash)> get_support_ticket_conversations_async_with_http_info(tenant_id, support_ticket_id, opts)

```ruby
begin
  # Retrieve conversations for a support ticket
  data, status_code, headers = api_instance.get_support_ticket_conversations_async_with_http_info(tenant_id, support_ticket_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SupportTicketConversationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->get_support_ticket_conversations_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_ticket_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SupportTicketConversationDtoListEnvelope**](SupportTicketConversationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_tickets_async

> <SupportTicketDtoListEnvelope> get_support_tickets_async(tenant_id, opts)

Retrieve a list of support tickets

Retrieves a list of support tickets for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of support tickets
  result = api_instance.get_support_tickets_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->get_support_tickets_async: #{e}"
end
```

#### Using the get_support_tickets_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SupportTicketDtoListEnvelope>, Integer, Hash)> get_support_tickets_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of support tickets
  data, status_code, headers = api_instance.get_support_tickets_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SupportTicketDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->get_support_tickets_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SupportTicketDtoListEnvelope**](SupportTicketDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_tickets_count_async

> <Int32Envelope> get_support_tickets_count_async(tenant_id, opts)

Get the count of support tickets

Returns the total count of support tickets for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of support tickets
  result = api_instance.get_support_tickets_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->get_support_tickets_count_async: #{e}"
end
```

#### Using the get_support_tickets_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_support_tickets_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of support tickets
  data, status_code, headers = api_instance.get_support_tickets_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->get_support_tickets_count_async_with_http_info: #{e}"
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


## patch_support_ticket_async

> <EmptyEnvelope> patch_support_ticket_async(tenant_id, support_ticket_id, opts)

Patch a support ticket

Partially updates an existing support ticket by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_ticket_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a support ticket
  result = api_instance.patch_support_ticket_async(tenant_id, support_ticket_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->patch_support_ticket_async: #{e}"
end
```

#### Using the patch_support_ticket_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_support_ticket_async_with_http_info(tenant_id, support_ticket_id, opts)

```ruby
begin
  # Patch a support ticket
  data, status_code, headers = api_instance.patch_support_ticket_async_with_http_info(tenant_id, support_ticket_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->patch_support_ticket_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_ticket_id** | **String** |  |  |
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


## relate_support_ticket_to_conversation_async

> <EmptyEnvelope> relate_support_ticket_to_conversation_async(tenant_id, support_ticket_id, opts)

Create a conversation for a support ticket

Creates a new conversation and associates it with the specified support ticket.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_ticket_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  support_ticket_conversation_create_dto: OpenapiClient::SupportTicketConversationCreateDto.new # SupportTicketConversationCreateDto | 
}

begin
  # Create a conversation for a support ticket
  result = api_instance.relate_support_ticket_to_conversation_async(tenant_id, support_ticket_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->relate_support_ticket_to_conversation_async: #{e}"
end
```

#### Using the relate_support_ticket_to_conversation_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> relate_support_ticket_to_conversation_async_with_http_info(tenant_id, support_ticket_id, opts)

```ruby
begin
  # Create a conversation for a support ticket
  data, status_code, headers = api_instance.relate_support_ticket_to_conversation_async_with_http_info(tenant_id, support_ticket_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->relate_support_ticket_to_conversation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_ticket_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **support_ticket_conversation_create_dto** | [**SupportTicketConversationCreateDto**](SupportTicketConversationCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_support_ticket_async

> <EmptyEnvelope> update_support_ticket_async(tenant_id, support_ticket_id, opts)

Update a support ticket

Updates an existing support ticket by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportTicketsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_ticket_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  support_ticket_update_dto: OpenapiClient::SupportTicketUpdateDto.new # SupportTicketUpdateDto | 
}

begin
  # Update a support ticket
  result = api_instance.update_support_ticket_async(tenant_id, support_ticket_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->update_support_ticket_async: #{e}"
end
```

#### Using the update_support_ticket_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_support_ticket_async_with_http_info(tenant_id, support_ticket_id, opts)

```ruby
begin
  # Update a support ticket
  data, status_code, headers = api_instance.update_support_ticket_async_with_http_info(tenant_id, support_ticket_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportTicketsApi->update_support_ticket_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_ticket_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **support_ticket_update_dto** | [**SupportTicketUpdateDto**](SupportTicketUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

