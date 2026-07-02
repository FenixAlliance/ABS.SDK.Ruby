# OpenapiClient::SupportRequestsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_support_request_async**](SupportRequestsApi.md#create_support_request_async) | **POST** /api/v2/SupportService/SupportRequests | Create a new support request |
| [**delete_support_request_async**](SupportRequestsApi.md#delete_support_request_async) | **DELETE** /api/v2/SupportService/SupportRequests/{supportRequestId} | Delete a support request |
| [**get_support_request_async**](SupportRequestsApi.md#get_support_request_async) | **GET** /api/v2/SupportService/SupportRequests/{supportRequestId} | Retrieve a support request by ID |
| [**get_support_request_attachment_by_request**](SupportRequestsApi.md#get_support_request_attachment_by_request) | **GET** /api/v2/SupportService/SupportRequests/{supportRequestId}/Attachments/{attachmentId} | Retrieve a specific attachment for a support request |
| [**get_support_request_attachments_by_request**](SupportRequestsApi.md#get_support_request_attachments_by_request) | **GET** /api/v2/SupportService/SupportRequests/{supportRequestId}/Attachments | Retrieve attachments for a support request |
| [**get_support_request_attachments_count_by_request**](SupportRequestsApi.md#get_support_request_attachments_count_by_request) | **GET** /api/v2/SupportService/SupportRequests/{supportRequestId}/Attachments/Count | Get the count of attachments for a support request |
| [**get_support_request_tickets_async**](SupportRequestsApi.md#get_support_request_tickets_async) | **GET** /api/v2/SupportService/SupportRequests/{supportRequestId}/Tickets | Retrieve tickets for a support request |
| [**get_support_requests_async**](SupportRequestsApi.md#get_support_requests_async) | **GET** /api/v2/SupportService/SupportRequests | Retrieve a list of support requests |
| [**get_support_requests_count_async**](SupportRequestsApi.md#get_support_requests_count_async) | **GET** /api/v2/SupportService/SupportRequests/Count | Get the count of support requests |
| [**patch_support_request_async**](SupportRequestsApi.md#patch_support_request_async) | **PATCH** /api/v2/SupportService/SupportRequests/{supportRequestId} | Patch a support request |
| [**relate_support_request_to_attachment_async**](SupportRequestsApi.md#relate_support_request_to_attachment_async) | **POST** /api/v2/SupportService/SupportRequests/{supportRequestId}/Attachments | Add an attachment to a support request |
| [**update_support_request_async**](SupportRequestsApi.md#update_support_request_async) | **PUT** /api/v2/SupportService/SupportRequests/{supportRequestId} | Update a support request |


## create_support_request_async

> <EmptyEnvelope> create_support_request_async(tenant_id, opts)

Create a new support request

Creates a new support request for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  support_request_create_dto: OpenapiClient::SupportRequestCreateDto.new({title: 'title_example'}) # SupportRequestCreateDto | 
}

begin
  # Create a new support request
  result = api_instance.create_support_request_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->create_support_request_async: #{e}"
end
```

#### Using the create_support_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_support_request_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new support request
  data, status_code, headers = api_instance.create_support_request_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->create_support_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **support_request_create_dto** | [**SupportRequestCreateDto**](SupportRequestCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_support_request_async

> <EmptyEnvelope> delete_support_request_async(tenant_id, support_request_id, opts)

Delete a support request

Deletes a support request by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a support request
  result = api_instance.delete_support_request_async(tenant_id, support_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->delete_support_request_async: #{e}"
end
```

#### Using the delete_support_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_support_request_async_with_http_info(tenant_id, support_request_id, opts)

```ruby
begin
  # Delete a support request
  data, status_code, headers = api_instance.delete_support_request_async_with_http_info(tenant_id, support_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->delete_support_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_request_async

> <SupportRequestDtoEnvelope> get_support_request_async(tenant_id, support_request_id, opts)

Retrieve a support request by ID

Retrieves a single support request by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a support request by ID
  result = api_instance.get_support_request_async(tenant_id, support_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->get_support_request_async: #{e}"
end
```

#### Using the get_support_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SupportRequestDtoEnvelope>, Integer, Hash)> get_support_request_async_with_http_info(tenant_id, support_request_id, opts)

```ruby
begin
  # Retrieve a support request by ID
  data, status_code, headers = api_instance.get_support_request_async_with_http_info(tenant_id, support_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SupportRequestDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->get_support_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SupportRequestDtoEnvelope**](SupportRequestDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_request_attachment_by_request

> <SupportRequestAttachmentDtoEnvelope> get_support_request_attachment_by_request(tenant_id, support_request_id, attachment_id, opts)

Retrieve a specific attachment for a support request

Retrieves a single attachment by its ID for a specific support request.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
attachment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a specific attachment for a support request
  result = api_instance.get_support_request_attachment_by_request(tenant_id, support_request_id, attachment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->get_support_request_attachment_by_request: #{e}"
end
```

#### Using the get_support_request_attachment_by_request_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SupportRequestAttachmentDtoEnvelope>, Integer, Hash)> get_support_request_attachment_by_request_with_http_info(tenant_id, support_request_id, attachment_id, opts)

```ruby
begin
  # Retrieve a specific attachment for a support request
  data, status_code, headers = api_instance.get_support_request_attachment_by_request_with_http_info(tenant_id, support_request_id, attachment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SupportRequestAttachmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->get_support_request_attachment_by_request_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_request_id** | **String** |  |  |
| **attachment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SupportRequestAttachmentDtoEnvelope**](SupportRequestAttachmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_request_attachments_by_request

> <SupportRequestAttachmentDtoListEnvelope> get_support_request_attachments_by_request(tenant_id, support_request_id, opts)

Retrieve attachments for a support request

Retrieves the list of attachments associated with a specific support request.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve attachments for a support request
  result = api_instance.get_support_request_attachments_by_request(tenant_id, support_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->get_support_request_attachments_by_request: #{e}"
end
```

#### Using the get_support_request_attachments_by_request_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SupportRequestAttachmentDtoListEnvelope>, Integer, Hash)> get_support_request_attachments_by_request_with_http_info(tenant_id, support_request_id, opts)

```ruby
begin
  # Retrieve attachments for a support request
  data, status_code, headers = api_instance.get_support_request_attachments_by_request_with_http_info(tenant_id, support_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SupportRequestAttachmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->get_support_request_attachments_by_request_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SupportRequestAttachmentDtoListEnvelope**](SupportRequestAttachmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_request_attachments_count_by_request

> <Int32Envelope> get_support_request_attachments_count_by_request(tenant_id, support_request_id, opts)

Get the count of attachments for a support request

Returns the total count of attachments for a specific support request.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of attachments for a support request
  result = api_instance.get_support_request_attachments_count_by_request(tenant_id, support_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->get_support_request_attachments_count_by_request: #{e}"
end
```

#### Using the get_support_request_attachments_count_by_request_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_support_request_attachments_count_by_request_with_http_info(tenant_id, support_request_id, opts)

```ruby
begin
  # Get the count of attachments for a support request
  data, status_code, headers = api_instance.get_support_request_attachments_count_by_request_with_http_info(tenant_id, support_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->get_support_request_attachments_count_by_request_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_request_tickets_async

> <SupportTicketDtoListEnvelope> get_support_request_tickets_async(tenant_id, support_request_id, opts)

Retrieve tickets for a support request

Retrieves the list of support tickets associated with a specific support request.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve tickets for a support request
  result = api_instance.get_support_request_tickets_async(tenant_id, support_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->get_support_request_tickets_async: #{e}"
end
```

#### Using the get_support_request_tickets_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SupportTicketDtoListEnvelope>, Integer, Hash)> get_support_request_tickets_async_with_http_info(tenant_id, support_request_id, opts)

```ruby
begin
  # Retrieve tickets for a support request
  data, status_code, headers = api_instance.get_support_request_tickets_async_with_http_info(tenant_id, support_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SupportTicketDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->get_support_request_tickets_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SupportTicketDtoListEnvelope**](SupportTicketDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_requests_async

> <SupportRequestDtoListEnvelope> get_support_requests_async(tenant_id, opts)

Retrieve a list of support requests

Retrieves a list of support requests for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of support requests
  result = api_instance.get_support_requests_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->get_support_requests_async: #{e}"
end
```

#### Using the get_support_requests_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SupportRequestDtoListEnvelope>, Integer, Hash)> get_support_requests_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of support requests
  data, status_code, headers = api_instance.get_support_requests_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SupportRequestDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->get_support_requests_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SupportRequestDtoListEnvelope**](SupportRequestDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_requests_count_async

> <Int32Envelope> get_support_requests_count_async(tenant_id, opts)

Get the count of support requests

Returns the total count of support requests for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of support requests
  result = api_instance.get_support_requests_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->get_support_requests_count_async: #{e}"
end
```

#### Using the get_support_requests_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_support_requests_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of support requests
  data, status_code, headers = api_instance.get_support_requests_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->get_support_requests_count_async_with_http_info: #{e}"
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


## patch_support_request_async

> <EmptyEnvelope> patch_support_request_async(tenant_id, support_request_id, opts)

Patch a support request

Partially updates an existing support request by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a support request
  result = api_instance.patch_support_request_async(tenant_id, support_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->patch_support_request_async: #{e}"
end
```

#### Using the patch_support_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_support_request_async_with_http_info(tenant_id, support_request_id, opts)

```ruby
begin
  # Patch a support request
  data, status_code, headers = api_instance.patch_support_request_async_with_http_info(tenant_id, support_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->patch_support_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_request_id** | **String** |  |  |
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


## relate_support_request_to_attachment_async

> <EmptyEnvelope> relate_support_request_to_attachment_async(tenant_id, support_request_id, opts)

Add an attachment to a support request

Creates a new attachment and associates it with the specified support request.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  support_request_attachment_create_dto: OpenapiClient::SupportRequestAttachmentCreateDto.new # SupportRequestAttachmentCreateDto | 
}

begin
  # Add an attachment to a support request
  result = api_instance.relate_support_request_to_attachment_async(tenant_id, support_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->relate_support_request_to_attachment_async: #{e}"
end
```

#### Using the relate_support_request_to_attachment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> relate_support_request_to_attachment_async_with_http_info(tenant_id, support_request_id, opts)

```ruby
begin
  # Add an attachment to a support request
  data, status_code, headers = api_instance.relate_support_request_to_attachment_async_with_http_info(tenant_id, support_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->relate_support_request_to_attachment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **support_request_attachment_create_dto** | [**SupportRequestAttachmentCreateDto**](SupportRequestAttachmentCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_support_request_async

> <EmptyEnvelope> update_support_request_async(tenant_id, support_request_id, opts)

Update a support request

Updates an existing support request by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  support_request_update_dto: OpenapiClient::SupportRequestUpdateDto.new # SupportRequestUpdateDto | 
}

begin
  # Update a support request
  result = api_instance.update_support_request_async(tenant_id, support_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->update_support_request_async: #{e}"
end
```

#### Using the update_support_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_support_request_async_with_http_info(tenant_id, support_request_id, opts)

```ruby
begin
  # Update a support request
  data, status_code, headers = api_instance.update_support_request_async_with_http_info(tenant_id, support_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestsApi->update_support_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **support_request_update_dto** | [**SupportRequestUpdateDto**](SupportRequestUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

