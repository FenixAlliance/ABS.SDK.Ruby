# OpenapiClient::InboxApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**cancel_inbox_message_retry**](InboxApi.md#cancel_inbox_message_retry) | **POST** /api/v2/SystemService/Inbox/Messages/{id}/CancelRetry | Cancel a scheduled inbox retry |
| [**dead_letter_inbox_message**](InboxApi.md#dead_letter_inbox_message) | **POST** /api/v2/SystemService/Inbox/Messages/{id}/DeadLetter | Manually dead-letter an inbox message |
| [**expedite_inbox_message**](InboxApi.md#expedite_inbox_message) | **POST** /api/v2/SystemService/Inbox/Messages/{id}/Expedite | Expedite a retry-scheduled inbox message |
| [**get_duplicate_inbox_messages**](InboxApi.md#get_duplicate_inbox_messages) | **GET** /api/v2/SystemService/Inbox/Duplicates | List duplicate-bearing inbox messages |
| [**get_duplicate_inbox_messages_count**](InboxApi.md#get_duplicate_inbox_messages_count) | **GET** /api/v2/SystemService/Inbox/Duplicates/Count | Count duplicate-bearing inbox messages |
| [**get_inbox_correlation_chain**](InboxApi.md#get_inbox_correlation_chain) | **GET** /api/v2/SystemService/Inbox/Correlations/{correlationId} | Get an inbox correlation chain |
| [**get_inbox_health**](InboxApi.md#get_inbox_health) | **GET** /api/v2/SystemService/Inbox/Health | Get durable-inbox processor health |
| [**get_inbox_message**](InboxApi.md#get_inbox_message) | **GET** /api/v2/SystemService/Inbox/Messages/{id} | Get one inbox message |
| [**get_inbox_messages**](InboxApi.md#get_inbox_messages) | **GET** /api/v2/SystemService/Inbox/Messages | List inbox messages |
| [**get_inbox_messages_count**](InboxApi.md#get_inbox_messages_count) | **GET** /api/v2/SystemService/Inbox/Messages/Count | Count inbox messages |
| [**quarantine_inbox_message**](InboxApi.md#quarantine_inbox_message) | **POST** /api/v2/SystemService/Inbox/Messages/{id}/Quarantine | Manually quarantine an inbox message |
| [**release_inbox_message_lease**](InboxApi.md#release_inbox_message_lease) | **POST** /api/v2/SystemService/Inbox/Messages/{id}/ReleaseLease | Release a stuck inbox lease |
| [**replay_inbox_message**](InboxApi.md#replay_inbox_message) | **POST** /api/v2/SystemService/Inbox/Messages/{id}/Replay | Replay a terminal inbox message as a new generation |


## cancel_inbox_message_retry

> <EmptyEnvelope> cancel_inbox_message_retry(id, opts)

Cancel a scheduled inbox retry

Stops a RetryScheduled message from retrying by operator decision, moving it to the terminal Cancelled state (deliberately distinct from DeadLettered so the dead-letter gauge stays honest). The reason is audit-critical. Only a RetryScheduled message can be cancelled. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InboxApi.new
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  inbox_admin_reason_dto: OpenapiClient::InboxAdminReasonDto.new({reason: 'reason_example'}) # InboxAdminReasonDto | 
}

begin
  # Cancel a scheduled inbox retry
  result = api_instance.cancel_inbox_message_retry(id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->cancel_inbox_message_retry: #{e}"
end
```

#### Using the cancel_inbox_message_retry_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> cancel_inbox_message_retry_with_http_info(id, opts)

```ruby
begin
  # Cancel a scheduled inbox retry
  data, status_code, headers = api_instance.cancel_inbox_message_retry_with_http_info(id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->cancel_inbox_message_retry_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **inbox_admin_reason_dto** | [**InboxAdminReasonDto**](InboxAdminReasonDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## dead_letter_inbox_message

> <EmptyEnvelope> dead_letter_inbox_message(id, opts)

Manually dead-letter an inbox message

Manually moves a non-terminal message to the terminal DeadLettered state. The reason is audit-critical. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InboxApi.new
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  inbox_admin_reason_dto: OpenapiClient::InboxAdminReasonDto.new({reason: 'reason_example'}) # InboxAdminReasonDto | 
}

begin
  # Manually dead-letter an inbox message
  result = api_instance.dead_letter_inbox_message(id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->dead_letter_inbox_message: #{e}"
end
```

#### Using the dead_letter_inbox_message_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> dead_letter_inbox_message_with_http_info(id, opts)

```ruby
begin
  # Manually dead-letter an inbox message
  data, status_code, headers = api_instance.dead_letter_inbox_message_with_http_info(id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->dead_letter_inbox_message_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **inbox_admin_reason_dto** | [**InboxAdminReasonDto**](InboxAdminReasonDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## expedite_inbox_message

> <EmptyEnvelope> expedite_inbox_message(id, opts)

Expedite a retry-scheduled inbox message

Pulls a RetryScheduled message's scheduled instant forward to now so the processor claims it on the next poll, bypassing the remaining backoff. Same row, retry budget untouched. Only a RetryScheduled message can be expedited. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InboxApi.new
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Expedite a retry-scheduled inbox message
  result = api_instance.expedite_inbox_message(id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->expedite_inbox_message: #{e}"
end
```

#### Using the expedite_inbox_message_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> expedite_inbox_message_with_http_info(id, opts)

```ruby
begin
  # Expedite a retry-scheduled inbox message
  data, status_code, headers = api_instance.expedite_inbox_message_with_http_info(id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->expedite_inbox_message_with_http_info: #{e}"
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


## get_duplicate_inbox_messages

> <InboxMessageDtoIReadOnlyListEnvelope> get_duplicate_inbox_messages(opts)

List duplicate-bearing inbox messages

Lists inbox messages that have observed a re-delivery (DeliveryCount > 1) — durable evidence that a source is re-sending, surfaced with DeliveryCount / LastDuplicateReceivedAtUtc. Further OData filtering/paging applies. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InboxApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  inbox_message_dto_collection_query_parameters: OpenapiClient::InboxMessageDtoCollectionQueryParameters.new # InboxMessageDtoCollectionQueryParameters | 
}

begin
  # List duplicate-bearing inbox messages
  result = api_instance.get_duplicate_inbox_messages(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->get_duplicate_inbox_messages: #{e}"
end
```

#### Using the get_duplicate_inbox_messages_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InboxMessageDtoIReadOnlyListEnvelope>, Integer, Hash)> get_duplicate_inbox_messages_with_http_info(opts)

```ruby
begin
  # List duplicate-bearing inbox messages
  data, status_code, headers = api_instance.get_duplicate_inbox_messages_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InboxMessageDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->get_duplicate_inbox_messages_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **inbox_message_dto_collection_query_parameters** | [**InboxMessageDtoCollectionQueryParameters**](InboxMessageDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**InboxMessageDtoIReadOnlyListEnvelope**](InboxMessageDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_duplicate_inbox_messages_count

> <Int32Envelope> get_duplicate_inbox_messages_count(opts)

Count duplicate-bearing inbox messages

Returns the count of duplicate-bearing inbox messages under the same OData shaping as the duplicates list. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InboxApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  inbox_message_dto_collection_query_parameters: OpenapiClient::InboxMessageDtoCollectionQueryParameters.new # InboxMessageDtoCollectionQueryParameters | 
}

begin
  # Count duplicate-bearing inbox messages
  result = api_instance.get_duplicate_inbox_messages_count(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->get_duplicate_inbox_messages_count: #{e}"
end
```

#### Using the get_duplicate_inbox_messages_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_duplicate_inbox_messages_count_with_http_info(opts)

```ruby
begin
  # Count duplicate-bearing inbox messages
  data, status_code, headers = api_instance.get_duplicate_inbox_messages_count_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->get_duplicate_inbox_messages_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **inbox_message_dto_collection_query_parameters** | [**InboxMessageDtoCollectionQueryParameters**](InboxMessageDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_inbox_correlation_chain

> <InboxMessageDtoIReadOnlyListEnvelope> get_inbox_correlation_chain(correlation_id, opts)

Get an inbox correlation chain

Returns every inbox message that shares a correlation id — one logical inbound interaction end-to-end, including its replay generations — oldest-received first. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InboxApi.new
correlation_id = 'correlation_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get an inbox correlation chain
  result = api_instance.get_inbox_correlation_chain(correlation_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->get_inbox_correlation_chain: #{e}"
end
```

#### Using the get_inbox_correlation_chain_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InboxMessageDtoIReadOnlyListEnvelope>, Integer, Hash)> get_inbox_correlation_chain_with_http_info(correlation_id, opts)

```ruby
begin
  # Get an inbox correlation chain
  data, status_code, headers = api_instance.get_inbox_correlation_chain_with_http_info(correlation_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InboxMessageDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->get_inbox_correlation_chain_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **correlation_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**InboxMessageDtoIReadOnlyListEnvelope**](InboxMessageDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_inbox_health

> <InboxHealthDtoEnvelope> get_inbox_health(opts)

Get durable-inbox processor health

Returns a single snapshot of the durable-inbox processor: whether it is enabled, the per-status counts (received/accepted/processing/retry-scheduled/rejected/quarantined/dead-lettered/cancelled), the age of the oldest accepted message, and the last successful processing instant. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InboxApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get durable-inbox processor health
  result = api_instance.get_inbox_health(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->get_inbox_health: #{e}"
end
```

#### Using the get_inbox_health_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InboxHealthDtoEnvelope>, Integer, Hash)> get_inbox_health_with_http_info(opts)

```ruby
begin
  # Get durable-inbox processor health
  data, status_code, headers = api_instance.get_inbox_health_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InboxHealthDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->get_inbox_health_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**InboxHealthDtoEnvelope**](InboxHealthDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_inbox_message

> <InboxMessageDtoEnvelope> get_inbox_message(id, opts)

Get one inbox message

Returns one inbox message's payload-safe detail by id — both lifecycle axes (processing status + independent verification status), the dedup lineage, attempt/generation counters, the recorded failure, and the timestamps. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InboxApi.new
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get one inbox message
  result = api_instance.get_inbox_message(id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->get_inbox_message: #{e}"
end
```

#### Using the get_inbox_message_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InboxMessageDtoEnvelope>, Integer, Hash)> get_inbox_message_with_http_info(id, opts)

```ruby
begin
  # Get one inbox message
  data, status_code, headers = api_instance.get_inbox_message_with_http_info(id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InboxMessageDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->get_inbox_message_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**InboxMessageDtoEnvelope**](InboxMessageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_inbox_messages

> <InboxMessageDtoIReadOnlyListEnvelope> get_inbox_messages(opts)

List inbox messages

Lists durable-inbox messages (payload-safe fields only). Use OData to scope by any projected field — e.g. $filter=Status eq 'Quarantined' for the quarantine review, Status eq 'DeadLettered' for terminal failures, VerificationStatus eq 'Failed' for forged/untrusted callbacks, SourceSystem eq 'stripe', or a ReceivedAtUtc range — and to page/order. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InboxApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  inbox_message_dto_collection_query_parameters: OpenapiClient::InboxMessageDtoCollectionQueryParameters.new # InboxMessageDtoCollectionQueryParameters | 
}

begin
  # List inbox messages
  result = api_instance.get_inbox_messages(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->get_inbox_messages: #{e}"
end
```

#### Using the get_inbox_messages_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InboxMessageDtoIReadOnlyListEnvelope>, Integer, Hash)> get_inbox_messages_with_http_info(opts)

```ruby
begin
  # List inbox messages
  data, status_code, headers = api_instance.get_inbox_messages_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InboxMessageDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->get_inbox_messages_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **inbox_message_dto_collection_query_parameters** | [**InboxMessageDtoCollectionQueryParameters**](InboxMessageDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**InboxMessageDtoIReadOnlyListEnvelope**](InboxMessageDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_inbox_messages_count

> <Int32Envelope> get_inbox_messages_count(opts)

Count inbox messages

Returns the count of durable-inbox messages under the same OData shaping as the list read (e.g. $filter=Status eq 'Quarantined'). Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InboxApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  inbox_message_dto_collection_query_parameters: OpenapiClient::InboxMessageDtoCollectionQueryParameters.new # InboxMessageDtoCollectionQueryParameters | 
}

begin
  # Count inbox messages
  result = api_instance.get_inbox_messages_count(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->get_inbox_messages_count: #{e}"
end
```

#### Using the get_inbox_messages_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_inbox_messages_count_with_http_info(opts)

```ruby
begin
  # Count inbox messages
  data, status_code, headers = api_instance.get_inbox_messages_count_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->get_inbox_messages_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **inbox_message_dto_collection_query_parameters** | [**InboxMessageDtoCollectionQueryParameters**](InboxMessageDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## quarantine_inbox_message

> <EmptyEnvelope> quarantine_inbox_message(id, opts)

Manually quarantine an inbox message

Manually holds a non-terminal message for review in the terminal Quarantined state (e.g. an operator judges it suspicious). The reason is audit-critical. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InboxApi.new
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  inbox_admin_reason_dto: OpenapiClient::InboxAdminReasonDto.new({reason: 'reason_example'}) # InboxAdminReasonDto | 
}

begin
  # Manually quarantine an inbox message
  result = api_instance.quarantine_inbox_message(id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->quarantine_inbox_message: #{e}"
end
```

#### Using the quarantine_inbox_message_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> quarantine_inbox_message_with_http_info(id, opts)

```ruby
begin
  # Manually quarantine an inbox message
  data, status_code, headers = api_instance.quarantine_inbox_message_with_http_info(id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->quarantine_inbox_message_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **inbox_admin_reason_dto** | [**InboxAdminReasonDto**](InboxAdminReasonDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## release_inbox_message_lease

> <EmptyEnvelope> release_inbox_message_lease(id, opts)

Release a stuck inbox lease

Force-releases the lease on a message wedged in Processing (a crashed/hung processor) and returns it to the claimable Accepted state, due now, so the next poll re-drives it. The in-flight attempt is NOT counted — a crash is not a business failure. Only a Processing message can have its lease released. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InboxApi.new
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Release a stuck inbox lease
  result = api_instance.release_inbox_message_lease(id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->release_inbox_message_lease: #{e}"
end
```

#### Using the release_inbox_message_lease_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> release_inbox_message_lease_with_http_info(id, opts)

```ruby
begin
  # Release a stuck inbox lease
  data, status_code, headers = api_instance.release_inbox_message_lease_with_http_info(id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->release_inbox_message_lease_with_http_info: #{e}"
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


## replay_inbox_message

> <InboxReplayResultDtoEnvelope> replay_inbox_message(id, opts)

Replay a terminal inbox message as a new generation

Replays a terminal message as a NEW processing generation over its immutable received evidence — the inbox's recovery lever (distinct from the outbox's same-row requeue). A selected replay-generation row is resolved back to its lineage root before replaying, so numbering stays global and collision-free; the new row is claimable at once with a fresh retry budget, and the root's evidence and budget are never mutated. Legal only from a terminal state whose authenticity passed. Returns the new generation's identity. The reason is audit-critical. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InboxApi.new
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  inbox_admin_reason_dto: OpenapiClient::InboxAdminReasonDto.new({reason: 'reason_example'}) # InboxAdminReasonDto | 
}

begin
  # Replay a terminal inbox message as a new generation
  result = api_instance.replay_inbox_message(id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->replay_inbox_message: #{e}"
end
```

#### Using the replay_inbox_message_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InboxReplayResultDtoEnvelope>, Integer, Hash)> replay_inbox_message_with_http_info(id, opts)

```ruby
begin
  # Replay a terminal inbox message as a new generation
  data, status_code, headers = api_instance.replay_inbox_message_with_http_info(id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InboxReplayResultDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InboxApi->replay_inbox_message_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **inbox_admin_reason_dto** | [**InboxAdminReasonDto**](InboxAdminReasonDto.md) |  | [optional] |

### Return type

[**InboxReplayResultDtoEnvelope**](InboxReplayResultDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

