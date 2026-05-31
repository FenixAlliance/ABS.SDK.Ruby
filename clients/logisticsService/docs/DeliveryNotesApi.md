# OpenapiClient::DeliveryNotesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_delivery_note_async**](DeliveryNotesApi.md#create_delivery_note_async) | **POST** /api/v2/LogisticsService/DeliveryNotes | Create a delivery note |
| [**delete_delivery_note_async**](DeliveryNotesApi.md#delete_delivery_note_async) | **DELETE** /api/v2/LogisticsService/DeliveryNotes/{deliveryNoteId} | Delete a delivery note |
| [**get_delivery_note_by_id_async**](DeliveryNotesApi.md#get_delivery_note_by_id_async) | **GET** /api/v2/LogisticsService/DeliveryNotes/{deliveryNoteId} | Get delivery note by ID |
| [**get_delivery_notes_async**](DeliveryNotesApi.md#get_delivery_notes_async) | **GET** /api/v2/LogisticsService/DeliveryNotes | Get all delivery notes |
| [**get_delivery_notes_count_async**](DeliveryNotesApi.md#get_delivery_notes_count_async) | **GET** /api/v2/LogisticsService/DeliveryNotes/Count | Get delivery notes count |
| [**update_delivery_note_async**](DeliveryNotesApi.md#update_delivery_note_async) | **PUT** /api/v2/LogisticsService/DeliveryNotes/{deliveryNoteId} | Update a delivery note |


## create_delivery_note_async

> <EmptyEnvelope> create_delivery_note_async(tenant_id, opts)

Create a delivery note

Creates a new delivery note.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DeliveryNotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  delivery_note_create_dto: OpenapiClient::DeliveryNoteCreateDto.new # DeliveryNoteCreateDto | 
}

begin
  # Create a delivery note
  result = api_instance.create_delivery_note_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DeliveryNotesApi->create_delivery_note_async: #{e}"
end
```

#### Using the create_delivery_note_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_delivery_note_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a delivery note
  data, status_code, headers = api_instance.create_delivery_note_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DeliveryNotesApi->create_delivery_note_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **delivery_note_create_dto** | [**DeliveryNoteCreateDto**](DeliveryNoteCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_delivery_note_async

> <EmptyEnvelope> delete_delivery_note_async(tenant_id, delivery_note_id, opts)

Delete a delivery note

Deletes a delivery note.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DeliveryNotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
delivery_note_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a delivery note
  result = api_instance.delete_delivery_note_async(tenant_id, delivery_note_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DeliveryNotesApi->delete_delivery_note_async: #{e}"
end
```

#### Using the delete_delivery_note_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_delivery_note_async_with_http_info(tenant_id, delivery_note_id, opts)

```ruby
begin
  # Delete a delivery note
  data, status_code, headers = api_instance.delete_delivery_note_async_with_http_info(tenant_id, delivery_note_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DeliveryNotesApi->delete_delivery_note_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **delivery_note_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_delivery_note_by_id_async

> <DeliveryNoteDtoEnvelope> get_delivery_note_by_id_async(tenant_id, delivery_note_id, opts)

Get delivery note by ID

Retrieves a specific delivery note.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DeliveryNotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
delivery_note_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get delivery note by ID
  result = api_instance.get_delivery_note_by_id_async(tenant_id, delivery_note_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DeliveryNotesApi->get_delivery_note_by_id_async: #{e}"
end
```

#### Using the get_delivery_note_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<DeliveryNoteDtoEnvelope>, Integer, Hash)> get_delivery_note_by_id_async_with_http_info(tenant_id, delivery_note_id, opts)

```ruby
begin
  # Get delivery note by ID
  data, status_code, headers = api_instance.get_delivery_note_by_id_async_with_http_info(tenant_id, delivery_note_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <DeliveryNoteDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DeliveryNotesApi->get_delivery_note_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **delivery_note_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**DeliveryNoteDtoEnvelope**](DeliveryNoteDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_delivery_notes_async

> <DeliveryNoteDtoListEnvelope> get_delivery_notes_async(tenant_id, opts)

Get all delivery notes

Retrieves all delivery notes for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DeliveryNotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all delivery notes
  result = api_instance.get_delivery_notes_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DeliveryNotesApi->get_delivery_notes_async: #{e}"
end
```

#### Using the get_delivery_notes_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<DeliveryNoteDtoListEnvelope>, Integer, Hash)> get_delivery_notes_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all delivery notes
  data, status_code, headers = api_instance.get_delivery_notes_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <DeliveryNoteDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DeliveryNotesApi->get_delivery_notes_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**DeliveryNoteDtoListEnvelope**](DeliveryNoteDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_delivery_notes_count_async

> <Int32Envelope> get_delivery_notes_count_async(tenant_id, opts)

Get delivery notes count

Returns the count of delivery notes.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DeliveryNotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get delivery notes count
  result = api_instance.get_delivery_notes_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DeliveryNotesApi->get_delivery_notes_count_async: #{e}"
end
```

#### Using the get_delivery_notes_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_delivery_notes_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get delivery notes count
  data, status_code, headers = api_instance.get_delivery_notes_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DeliveryNotesApi->get_delivery_notes_count_async_with_http_info: #{e}"
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


## update_delivery_note_async

> <EmptyEnvelope> update_delivery_note_async(tenant_id, delivery_note_id, opts)

Update a delivery note

Updates an existing delivery note.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DeliveryNotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
delivery_note_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  delivery_note_update_dto: OpenapiClient::DeliveryNoteUpdateDto.new # DeliveryNoteUpdateDto | 
}

begin
  # Update a delivery note
  result = api_instance.update_delivery_note_async(tenant_id, delivery_note_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DeliveryNotesApi->update_delivery_note_async: #{e}"
end
```

#### Using the update_delivery_note_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_delivery_note_async_with_http_info(tenant_id, delivery_note_id, opts)

```ruby
begin
  # Update a delivery note
  data, status_code, headers = api_instance.update_delivery_note_async_with_http_info(tenant_id, delivery_note_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DeliveryNotesApi->update_delivery_note_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **delivery_note_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **delivery_note_update_dto** | [**DeliveryNoteUpdateDto**](DeliveryNoteUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

