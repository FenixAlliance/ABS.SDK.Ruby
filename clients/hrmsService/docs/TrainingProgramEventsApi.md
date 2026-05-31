# OpenapiClient::TrainingProgramEventsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_training_program_event_async**](TrainingProgramEventsApi.md#create_training_program_event_async) | **POST** /api/v2/HrmsService/TrainingProgramEvents | Create a training program event |
| [**delete_training_program_event_async**](TrainingProgramEventsApi.md#delete_training_program_event_async) | **DELETE** /api/v2/HrmsService/TrainingProgramEvents/{eventId} | Delete a training program event |
| [**get_training_program_event_by_id_async**](TrainingProgramEventsApi.md#get_training_program_event_by_id_async) | **GET** /api/v2/HrmsService/TrainingProgramEvents/{eventId} | Get training program event by ID |
| [**get_training_program_events_async**](TrainingProgramEventsApi.md#get_training_program_events_async) | **GET** /api/v2/HrmsService/TrainingProgramEvents | Get training program events |
| [**get_training_program_events_count_async**](TrainingProgramEventsApi.md#get_training_program_events_count_async) | **GET** /api/v2/HrmsService/TrainingProgramEvents/Count | Count training program events |
| [**update_training_program_event_async**](TrainingProgramEventsApi.md#update_training_program_event_async) | **PUT** /api/v2/HrmsService/TrainingProgramEvents/{eventId} | Update a training program event |


## create_training_program_event_async

> <EmptyEnvelope> create_training_program_event_async(tenant_id, opts)

Create a training program event

Creates a new training program event for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrainingProgramEventsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  training_program_event_create_dto: OpenapiClient::TrainingProgramEventCreateDto.new({title: 'title_example', start: Time.now, _end: Time.now, training_program_id: 'training_program_id_example'}) # TrainingProgramEventCreateDto | 
}

begin
  # Create a training program event
  result = api_instance.create_training_program_event_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramEventsApi->create_training_program_event_async: #{e}"
end
```

#### Using the create_training_program_event_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_training_program_event_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a training program event
  data, status_code, headers = api_instance.create_training_program_event_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramEventsApi->create_training_program_event_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **training_program_event_create_dto** | [**TrainingProgramEventCreateDto**](TrainingProgramEventCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_training_program_event_async

> <EmptyEnvelope> delete_training_program_event_async(tenant_id, event_id, opts)

Delete a training program event

Deletes a training program event for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrainingProgramEventsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
event_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a training program event
  result = api_instance.delete_training_program_event_async(tenant_id, event_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramEventsApi->delete_training_program_event_async: #{e}"
end
```

#### Using the delete_training_program_event_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_training_program_event_async_with_http_info(tenant_id, event_id, opts)

```ruby
begin
  # Delete a training program event
  data, status_code, headers = api_instance.delete_training_program_event_async_with_http_info(tenant_id, event_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramEventsApi->delete_training_program_event_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **event_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_training_program_event_by_id_async

> <TrainingProgramEventDtoEnvelope> get_training_program_event_by_id_async(tenant_id, event_id, opts)

Get training program event by ID

Retrieves a specific training program event by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrainingProgramEventsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
event_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get training program event by ID
  result = api_instance.get_training_program_event_by_id_async(tenant_id, event_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramEventsApi->get_training_program_event_by_id_async: #{e}"
end
```

#### Using the get_training_program_event_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TrainingProgramEventDtoEnvelope>, Integer, Hash)> get_training_program_event_by_id_async_with_http_info(tenant_id, event_id, opts)

```ruby
begin
  # Get training program event by ID
  data, status_code, headers = api_instance.get_training_program_event_by_id_async_with_http_info(tenant_id, event_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TrainingProgramEventDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramEventsApi->get_training_program_event_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **event_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TrainingProgramEventDtoEnvelope**](TrainingProgramEventDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_training_program_events_async

> <TrainingProgramEventDtoListEnvelope> get_training_program_events_async(tenant_id, opts)

Get training program events

Retrieves training program events for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrainingProgramEventsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get training program events
  result = api_instance.get_training_program_events_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramEventsApi->get_training_program_events_async: #{e}"
end
```

#### Using the get_training_program_events_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TrainingProgramEventDtoListEnvelope>, Integer, Hash)> get_training_program_events_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get training program events
  data, status_code, headers = api_instance.get_training_program_events_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TrainingProgramEventDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramEventsApi->get_training_program_events_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TrainingProgramEventDtoListEnvelope**](TrainingProgramEventDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_training_program_events_count_async

> <Int32Envelope> get_training_program_events_count_async(tenant_id, opts)

Count training program events

Counts training program events for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrainingProgramEventsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count training program events
  result = api_instance.get_training_program_events_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramEventsApi->get_training_program_events_count_async: #{e}"
end
```

#### Using the get_training_program_events_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_training_program_events_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count training program events
  data, status_code, headers = api_instance.get_training_program_events_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramEventsApi->get_training_program_events_count_async_with_http_info: #{e}"
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


## update_training_program_event_async

> <EmptyEnvelope> update_training_program_event_async(tenant_id, event_id, opts)

Update a training program event

Updates an existing training program event for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrainingProgramEventsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
event_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  training_program_event_update_dto: OpenapiClient::TrainingProgramEventUpdateDto.new # TrainingProgramEventUpdateDto | 
}

begin
  # Update a training program event
  result = api_instance.update_training_program_event_async(tenant_id, event_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramEventsApi->update_training_program_event_async: #{e}"
end
```

#### Using the update_training_program_event_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_training_program_event_async_with_http_info(tenant_id, event_id, opts)

```ruby
begin
  # Update a training program event
  data, status_code, headers = api_instance.update_training_program_event_async_with_http_info(tenant_id, event_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramEventsApi->update_training_program_event_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **event_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **training_program_event_update_dto** | [**TrainingProgramEventUpdateDto**](TrainingProgramEventUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

