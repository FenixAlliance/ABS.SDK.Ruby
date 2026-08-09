# OpenapiClient::OutboxApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**cancel_outbox_message**](OutboxApi.md#cancel_outbox_message) | **POST** /api/v2/SystemService/Outbox/Messages/{id}/Cancel | Cancel an outbox message |
| [**dead_letter_outbox_message**](OutboxApi.md#dead_letter_outbox_message) | **POST** /api/v2/SystemService/Outbox/Messages/{id}/DeadLetter | Manually dead-letter an outbox message |
| [**expedite_outbox_message**](OutboxApi.md#expedite_outbox_message) | **POST** /api/v2/SystemService/Outbox/Messages/{id}/Expedite | Expedite a failed (retry-eligible) outbox message |
| [**get_outbox_correlation_chain**](OutboxApi.md#get_outbox_correlation_chain) | **GET** /api/v2/SystemService/Outbox/Correlations/{correlationId} | Get an outbox correlation chain |
| [**get_outbox_health**](OutboxApi.md#get_outbox_health) | **GET** /api/v2/SystemService/Outbox/Health | Get durable-outbox relay health |
| [**get_outbox_message**](OutboxApi.md#get_outbox_message) | **GET** /api/v2/SystemService/Outbox/Messages/{id} | Get one outbox message |
| [**get_outbox_messages**](OutboxApi.md#get_outbox_messages) | **GET** /api/v2/SystemService/Outbox/Messages | List outbox messages |
| [**get_outbox_messages_count**](OutboxApi.md#get_outbox_messages_count) | **GET** /api/v2/SystemService/Outbox/Messages/Count | Count outbox messages |
| [**release_outbox_message_lease**](OutboxApi.md#release_outbox_message_lease) | **POST** /api/v2/SystemService/Outbox/Messages/{id}/ReleaseLease | Release a stuck outbox lease |
| [**replay_outbox_message**](OutboxApi.md#replay_outbox_message) | **POST** /api/v2/SystemService/Outbox/Messages/{id}/Replay | Replay a dead-lettered or failed outbox message |


## cancel_outbox_message

> <EmptyEnvelope> cancel_outbox_message(id, opts)

Cancel an outbox message

Stops a Pending or Failed message by operator decision, moving it to the terminal Cancelled state (deliberately distinct from DeadLettered so the dead-letter gauge stays honest). The reason is audit-critical. An in-flight (Processing) or already-terminal message is rejected. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OutboxApi.new
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  outbox_admin_reason_dto: OpenapiClient::OutboxAdminReasonDto.new({reason: 'reason_example'}) # OutboxAdminReasonDto | 
}

begin
  # Cancel an outbox message
  result = api_instance.cancel_outbox_message(id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->cancel_outbox_message: #{e}"
end
```

#### Using the cancel_outbox_message_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> cancel_outbox_message_with_http_info(id, opts)

```ruby
begin
  # Cancel an outbox message
  data, status_code, headers = api_instance.cancel_outbox_message_with_http_info(id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->cancel_outbox_message_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **outbox_admin_reason_dto** | [**OutboxAdminReasonDto**](OutboxAdminReasonDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## dead_letter_outbox_message

> <EmptyEnvelope> dead_letter_outbox_message(id, opts)

Manually dead-letter an outbox message

Manually moves a Processing or Failed message to the terminal DeadLettered state. The reason is audit-critical. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OutboxApi.new
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  outbox_admin_reason_dto: OpenapiClient::OutboxAdminReasonDto.new({reason: 'reason_example'}) # OutboxAdminReasonDto | 
}

begin
  # Manually dead-letter an outbox message
  result = api_instance.dead_letter_outbox_message(id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->dead_letter_outbox_message: #{e}"
end
```

#### Using the dead_letter_outbox_message_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> dead_letter_outbox_message_with_http_info(id, opts)

```ruby
begin
  # Manually dead-letter an outbox message
  data, status_code, headers = api_instance.dead_letter_outbox_message_with_http_info(id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->dead_letter_outbox_message_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **outbox_admin_reason_dto** | [**OutboxAdminReasonDto**](OutboxAdminReasonDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## expedite_outbox_message

> <EmptyEnvelope> expedite_outbox_message(id, opts)

Expedite a failed (retry-eligible) outbox message

Pulls a Failed message's scheduled instant forward to now so the relay claims it on the next poll, bypassing the remaining backoff. Same row, retry budget untouched (the lighter-touch counterpart to Replay, which also clears the recorded error). Only a Failed message can be expedited. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OutboxApi.new
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Expedite a failed (retry-eligible) outbox message
  result = api_instance.expedite_outbox_message(id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->expedite_outbox_message: #{e}"
end
```

#### Using the expedite_outbox_message_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> expedite_outbox_message_with_http_info(id, opts)

```ruby
begin
  # Expedite a failed (retry-eligible) outbox message
  data, status_code, headers = api_instance.expedite_outbox_message_with_http_info(id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->expedite_outbox_message_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_outbox_correlation_chain

> <OutboxMessageDtoIReadOnlyListEnvelope> get_outbox_correlation_chain(correlation_id, opts)

Get an outbox correlation chain

Returns every outbox message that shares a correlation id — one logical unit of async work end-to-end (e.g. a command and the events its handler in turn staged) — oldest-created first. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OutboxApi.new
correlation_id = 'correlation_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get an outbox correlation chain
  result = api_instance.get_outbox_correlation_chain(correlation_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->get_outbox_correlation_chain: #{e}"
end
```

#### Using the get_outbox_correlation_chain_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OutboxMessageDtoIReadOnlyListEnvelope>, Integer, Hash)> get_outbox_correlation_chain_with_http_info(correlation_id, opts)

```ruby
begin
  # Get an outbox correlation chain
  data, status_code, headers = api_instance.get_outbox_correlation_chain_with_http_info(correlation_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OutboxMessageDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->get_outbox_correlation_chain_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **correlation_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**OutboxMessageDtoIReadOnlyListEnvelope**](OutboxMessageDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_outbox_health

> <OutboxHealthDtoEnvelope> get_outbox_health(opts)

Get durable-outbox relay health

Returns a single snapshot of the durable-outbox relay: whether it is enabled, the per-status counts (pending/processing/failed/dead-lettered), the age of the oldest pending message, and the last successful dispatch instant. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OutboxApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get durable-outbox relay health
  result = api_instance.get_outbox_health(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->get_outbox_health: #{e}"
end
```

#### Using the get_outbox_health_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OutboxHealthDtoEnvelope>, Integer, Hash)> get_outbox_health_with_http_info(opts)

```ruby
begin
  # Get durable-outbox relay health
  data, status_code, headers = api_instance.get_outbox_health_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OutboxHealthDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->get_outbox_health_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**OutboxHealthDtoEnvelope**](OutboxHealthDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_outbox_message

> <OutboxMessageDtoEnvelope> get_outbox_message(id, opts)

Get one outbox message

Returns one outbox message's payload-safe detail by id — its lifecycle status, the two classification axes (kind + message type), the attempt/ceiling budget, the recorded failure, the idempotency + correlation lineage, and the timestamps. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OutboxApi.new
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get one outbox message
  result = api_instance.get_outbox_message(id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->get_outbox_message: #{e}"
end
```

#### Using the get_outbox_message_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OutboxMessageDtoEnvelope>, Integer, Hash)> get_outbox_message_with_http_info(id, opts)

```ruby
begin
  # Get one outbox message
  data, status_code, headers = api_instance.get_outbox_message_with_http_info(id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OutboxMessageDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->get_outbox_message_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**OutboxMessageDtoEnvelope**](OutboxMessageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_outbox_messages

> <OutboxMessageDtoIReadOnlyListEnvelope> get_outbox_messages(opts)

List outbox messages

Lists durable-outbox messages (payload-safe fields only). Use OData to scope to a state — e.g. $filter=Status eq 'DeadLettered' for the dead-letter set or Status eq 'Failed' for retry-eligible rows — and to page/order. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OutboxApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  outbox_message_dto_collection_query_parameters: OpenapiClient::OutboxMessageDtoCollectionQueryParameters.new # OutboxMessageDtoCollectionQueryParameters | 
}

begin
  # List outbox messages
  result = api_instance.get_outbox_messages(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->get_outbox_messages: #{e}"
end
```

#### Using the get_outbox_messages_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OutboxMessageDtoIReadOnlyListEnvelope>, Integer, Hash)> get_outbox_messages_with_http_info(opts)

```ruby
begin
  # List outbox messages
  data, status_code, headers = api_instance.get_outbox_messages_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OutboxMessageDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->get_outbox_messages_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **outbox_message_dto_collection_query_parameters** | [**OutboxMessageDtoCollectionQueryParameters**](OutboxMessageDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**OutboxMessageDtoIReadOnlyListEnvelope**](OutboxMessageDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_outbox_messages_count

> <Int32Envelope> get_outbox_messages_count(opts)

Count outbox messages

Returns the count of durable-outbox messages under the same OData shaping as the list read (e.g. $filter=Status eq 'DeadLettered'). Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OutboxApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  outbox_message_dto_collection_query_parameters: OpenapiClient::OutboxMessageDtoCollectionQueryParameters.new # OutboxMessageDtoCollectionQueryParameters | 
}

begin
  # Count outbox messages
  result = api_instance.get_outbox_messages_count(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->get_outbox_messages_count: #{e}"
end
```

#### Using the get_outbox_messages_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_outbox_messages_count_with_http_info(opts)

```ruby
begin
  # Count outbox messages
  data, status_code, headers = api_instance.get_outbox_messages_count_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->get_outbox_messages_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **outbox_message_dto_collection_query_parameters** | [**OutboxMessageDtoCollectionQueryParameters**](OutboxMessageDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## release_outbox_message_lease

> <EmptyEnvelope> release_outbox_message_lease(id, opts)

Release a stuck outbox lease

Force-releases the lease on a message wedged in Processing (a crashed/hung relay) and returns it to the claimable Pending state, due now, so the next poll re-drives it. The in-flight attempt is NOT counted — a crash is not a business failure. The relay auto-reclaims a crashed row once its lease expires; this manual lever forces the release immediately. Only a Processing message can have its lease released. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OutboxApi.new
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Release a stuck outbox lease
  result = api_instance.release_outbox_message_lease(id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->release_outbox_message_lease: #{e}"
end
```

#### Using the release_outbox_message_lease_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> release_outbox_message_lease_with_http_info(id, opts)

```ruby
begin
  # Release a stuck outbox lease
  data, status_code, headers = api_instance.release_outbox_message_lease_with_http_info(id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->release_outbox_message_lease_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## replay_outbox_message

> <EmptyEnvelope> replay_outbox_message(id, opts)

Replay a dead-lettered or failed outbox message

Requeues a DeadLettered or Failed message back to Pending so the relay re-drives it immediately (clearing the lease and recorded error, and bypassing the remaining backoff). The attempt budget is preserved — a replay grants one more pass, not a fresh budget. Replaying a message that is already Pending/Processing or is Succeeded/Cancelled is rejected. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OutboxApi.new
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Replay a dead-lettered or failed outbox message
  result = api_instance.replay_outbox_message(id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->replay_outbox_message: #{e}"
end
```

#### Using the replay_outbox_message_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> replay_outbox_message_with_http_info(id, opts)

```ruby
begin
  # Replay a dead-lettered or failed outbox message
  data, status_code, headers = api_instance.replay_outbox_message_with_http_info(id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OutboxApi->replay_outbox_message_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

