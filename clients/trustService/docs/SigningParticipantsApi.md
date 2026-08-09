# OpenapiClient::SigningParticipantsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_signing_participant_by_id_async**](SigningParticipantsApi.md#get_signing_participant_by_id_async) | **GET** /api/v2/TrustService/SigningParticipants/{id} | Get signing participant by ID |
| [**get_signing_participants_async**](SigningParticipantsApi.md#get_signing_participants_async) | **GET** /api/v2/TrustService/SigningParticipants | Get all signing participants |
| [**get_signing_participants_count_async**](SigningParticipantsApi.md#get_signing_participants_count_async) | **GET** /api/v2/TrustService/SigningParticipants/Count | Get signing participants count |
| [**mark_viewed_async**](SigningParticipantsApi.md#mark_viewed_async) | **POST** /api/v2/TrustService/SigningParticipants/{id}/viewed | Mark a participant as having viewed the request |
| [**record_outcome_async**](SigningParticipantsApi.md#record_outcome_async) | **POST** /api/v2/TrustService/SigningParticipants/{id}/outcome | Record a manual/external participant outcome |


## get_signing_participant_by_id_async

> <SigningParticipantDto> get_signing_participant_by_id_async(tenant_id, id, opts)

Get signing participant by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningParticipantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = 'id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get signing participant by ID
  result = api_instance.get_signing_participant_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningParticipantsApi->get_signing_participant_by_id_async: #{e}"
end
```

#### Using the get_signing_participant_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SigningParticipantDto>, Integer, Hash)> get_signing_participant_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get signing participant by ID
  data, status_code, headers = api_instance.get_signing_participant_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SigningParticipantDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningParticipantsApi->get_signing_participant_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SigningParticipantDto**](SigningParticipantDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_signing_participants_async

> <SigningParticipantDtoListEnvelope> get_signing_participants_async(tenant_id, opts)

Get all signing participants

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningParticipantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signing_participant_dto_collection_query_parameters: OpenapiClient::SigningParticipantDtoCollectionQueryParameters.new # SigningParticipantDtoCollectionQueryParameters | 
}

begin
  # Get all signing participants
  result = api_instance.get_signing_participants_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningParticipantsApi->get_signing_participants_async: #{e}"
end
```

#### Using the get_signing_participants_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SigningParticipantDtoListEnvelope>, Integer, Hash)> get_signing_participants_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all signing participants
  data, status_code, headers = api_instance.get_signing_participants_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SigningParticipantDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningParticipantsApi->get_signing_participants_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signing_participant_dto_collection_query_parameters** | [**SigningParticipantDtoCollectionQueryParameters**](SigningParticipantDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**SigningParticipantDtoListEnvelope**](SigningParticipantDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_signing_participants_count_async

> <Int32Envelope> get_signing_participants_count_async(tenant_id, opts)

Get signing participants count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningParticipantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signing_participant_dto_collection_query_parameters: OpenapiClient::SigningParticipantDtoCollectionQueryParameters.new # SigningParticipantDtoCollectionQueryParameters | 
}

begin
  # Get signing participants count
  result = api_instance.get_signing_participants_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningParticipantsApi->get_signing_participants_count_async: #{e}"
end
```

#### Using the get_signing_participants_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_signing_participants_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get signing participants count
  data, status_code, headers = api_instance.get_signing_participants_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningParticipantsApi->get_signing_participants_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signing_participant_dto_collection_query_parameters** | [**SigningParticipantDtoCollectionQueryParameters**](SigningParticipantDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## mark_viewed_async

> mark_viewed_async(tenant_id, id, opts)

Mark a participant as having viewed the request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningParticipantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = 'id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Mark a participant as having viewed the request
  api_instance.mark_viewed_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningParticipantsApi->mark_viewed_async: #{e}"
end
```

#### Using the mark_viewed_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> mark_viewed_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Mark a participant as having viewed the request
  data, status_code, headers = api_instance.mark_viewed_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningParticipantsApi->mark_viewed_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## record_outcome_async

> record_outcome_async(tenant_id, id, opts)

Record a manual/external participant outcome

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningParticipantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = 'id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  record_signing_participant_outcome_dto: OpenapiClient::RecordSigningParticipantOutcomeDto.new({outcome: 'Pending'}) # RecordSigningParticipantOutcomeDto | 
}

begin
  # Record a manual/external participant outcome
  api_instance.record_outcome_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningParticipantsApi->record_outcome_async: #{e}"
end
```

#### Using the record_outcome_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> record_outcome_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Record a manual/external participant outcome
  data, status_code, headers = api_instance.record_outcome_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningParticipantsApi->record_outcome_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **record_signing_participant_outcome_dto** | [**RecordSigningParticipantOutcomeDto**](RecordSigningParticipantOutcomeDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

