# OpenapiClient::SigningRequestsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**add_participant_async**](SigningRequestsApi.md#add_participant_async) | **POST** /api/v2/TrustService/SigningRequests/{id}/participants | Add a participant to a signing request |
| [**create_from_document_async**](SigningRequestsApi.md#create_from_document_async) | **POST** /api/v2/TrustService/SigningRequests/from-document/{signedDocumentId} | Create a signing request from a frozen document |
| [**execute_provider_async**](SigningRequestsApi.md#execute_provider_async) | **POST** /api/v2/TrustService/SigningRequests/{id}/execute-provider | Run a signing provider to produce + finalize the signed artifact |
| [**expire_async**](SigningRequestsApi.md#expire_async) | **POST** /api/v2/TrustService/SigningRequests/{id}/expire | Expire a signing request |
| [**finalize_async**](SigningRequestsApi.md#finalize_async) | **POST** /api/v2/TrustService/SigningRequests/{id}/finalize | Finalize a completed request into a signed artifact |
| [**get_signing_request_by_id_async**](SigningRequestsApi.md#get_signing_request_by_id_async) | **GET** /api/v2/TrustService/SigningRequests/{id} | Get signing request by ID |
| [**get_signing_request_participants_async**](SigningRequestsApi.md#get_signing_request_participants_async) | **GET** /api/v2/TrustService/SigningRequests/{id}/Participants | Get participants of a signing request |
| [**get_signing_requests_async**](SigningRequestsApi.md#get_signing_requests_async) | **GET** /api/v2/TrustService/SigningRequests | Get all signing requests |
| [**get_signing_requests_count_async**](SigningRequestsApi.md#get_signing_requests_count_async) | **GET** /api/v2/TrustService/SigningRequests/Count | Get signing requests count |
| [**prepare_and_create_async**](SigningRequestsApi.md#prepare_and_create_async) | **POST** /api/v2/TrustService/SigningRequests/prepare-and-create | Create, store, freeze a document and open a signing request in one call |
| [**send_async**](SigningRequestsApi.md#send_async) | **POST** /api/v2/TrustService/SigningRequests/{id}/send | Send a signing request |
| [**void_async**](SigningRequestsApi.md#void_async) | **POST** /api/v2/TrustService/SigningRequests/{id}/void | Void a signing request |


## add_participant_async

> <SigningParticipantDto> add_participant_async(tenant_id, id, opts)

Add a participant to a signing request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = 'id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  create_signing_participant_dto: OpenapiClient::CreateSigningParticipantDto.new({contact_id: 'contact_id_example'}) # CreateSigningParticipantDto | 
}

begin
  # Add a participant to a signing request
  result = api_instance.add_participant_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->add_participant_async: #{e}"
end
```

#### Using the add_participant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SigningParticipantDto>, Integer, Hash)> add_participant_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Add a participant to a signing request
  data, status_code, headers = api_instance.add_participant_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SigningParticipantDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->add_participant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **create_signing_participant_dto** | [**CreateSigningParticipantDto**](CreateSigningParticipantDto.md) |  | [optional] |

### Return type

[**SigningParticipantDto**](SigningParticipantDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_from_document_async

> <SigningRequestDto> create_from_document_async(tenant_id, signed_document_id, opts)

Create a signing request from a frozen document

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
signed_document_id = 'signed_document_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  create_signing_request_dto: OpenapiClient::CreateSigningRequestDto.new # CreateSigningRequestDto | 
}

begin
  # Create a signing request from a frozen document
  result = api_instance.create_from_document_async(tenant_id, signed_document_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->create_from_document_async: #{e}"
end
```

#### Using the create_from_document_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SigningRequestDto>, Integer, Hash)> create_from_document_async_with_http_info(tenant_id, signed_document_id, opts)

```ruby
begin
  # Create a signing request from a frozen document
  data, status_code, headers = api_instance.create_from_document_async_with_http_info(tenant_id, signed_document_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SigningRequestDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->create_from_document_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **signed_document_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **create_signing_request_dto** | [**CreateSigningRequestDto**](CreateSigningRequestDto.md) |  | [optional] |

### Return type

[**SigningRequestDto**](SigningRequestDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## execute_provider_async

> execute_provider_async(tenant_id, id, opts)

Run a signing provider to produce + finalize the signed artifact

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = 'id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  execute_signing_request_dto: OpenapiClient::ExecuteSigningRequestDto.new({provider_name: 'provider_name_example'}) # ExecuteSigningRequestDto | 
}

begin
  # Run a signing provider to produce + finalize the signed artifact
  api_instance.execute_provider_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->execute_provider_async: #{e}"
end
```

#### Using the execute_provider_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> execute_provider_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Run a signing provider to produce + finalize the signed artifact
  data, status_code, headers = api_instance.execute_provider_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->execute_provider_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **execute_signing_request_dto** | [**ExecuteSigningRequestDto**](ExecuteSigningRequestDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## expire_async

> expire_async(tenant_id, id, opts)

Expire a signing request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = 'id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Expire a signing request
  api_instance.expire_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->expire_async: #{e}"
end
```

#### Using the expire_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> expire_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Expire a signing request
  data, status_code, headers = api_instance.expire_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->expire_async_with_http_info: #{e}"
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


## finalize_async

> finalize_async(tenant_id, id, opts)

Finalize a completed request into a signed artifact

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = 'id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  finalize_signing_request_dto: OpenapiClient::FinalizeSigningRequestDto.new({signed_file_upload_id: 'signed_file_upload_id_example'}) # FinalizeSigningRequestDto | 
}

begin
  # Finalize a completed request into a signed artifact
  api_instance.finalize_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->finalize_async: #{e}"
end
```

#### Using the finalize_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> finalize_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Finalize a completed request into a signed artifact
  data, status_code, headers = api_instance.finalize_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->finalize_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **finalize_signing_request_dto** | [**FinalizeSigningRequestDto**](FinalizeSigningRequestDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_signing_request_by_id_async

> <SigningRequestDto> get_signing_request_by_id_async(tenant_id, id, opts)

Get signing request by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = 'id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get signing request by ID
  result = api_instance.get_signing_request_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->get_signing_request_by_id_async: #{e}"
end
```

#### Using the get_signing_request_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SigningRequestDto>, Integer, Hash)> get_signing_request_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get signing request by ID
  data, status_code, headers = api_instance.get_signing_request_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SigningRequestDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->get_signing_request_by_id_async_with_http_info: #{e}"
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

[**SigningRequestDto**](SigningRequestDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_signing_request_participants_async

> <SigningParticipantDtoListEnvelope> get_signing_request_participants_async(tenant_id, id, opts)

Get participants of a signing request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = 'id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get participants of a signing request
  result = api_instance.get_signing_request_participants_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->get_signing_request_participants_async: #{e}"
end
```

#### Using the get_signing_request_participants_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SigningParticipantDtoListEnvelope>, Integer, Hash)> get_signing_request_participants_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get participants of a signing request
  data, status_code, headers = api_instance.get_signing_request_participants_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SigningParticipantDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->get_signing_request_participants_async_with_http_info: #{e}"
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

[**SigningParticipantDtoListEnvelope**](SigningParticipantDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_signing_requests_async

> <SigningRequestDtoListEnvelope> get_signing_requests_async(tenant_id, opts)

Get all signing requests

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signing_request_dto_collection_query_parameters: OpenapiClient::SigningRequestDtoCollectionQueryParameters.new # SigningRequestDtoCollectionQueryParameters | 
}

begin
  # Get all signing requests
  result = api_instance.get_signing_requests_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->get_signing_requests_async: #{e}"
end
```

#### Using the get_signing_requests_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SigningRequestDtoListEnvelope>, Integer, Hash)> get_signing_requests_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all signing requests
  data, status_code, headers = api_instance.get_signing_requests_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SigningRequestDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->get_signing_requests_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signing_request_dto_collection_query_parameters** | [**SigningRequestDtoCollectionQueryParameters**](SigningRequestDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**SigningRequestDtoListEnvelope**](SigningRequestDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_signing_requests_count_async

> <Int32Envelope> get_signing_requests_count_async(tenant_id, opts)

Get signing requests count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signing_request_dto_collection_query_parameters: OpenapiClient::SigningRequestDtoCollectionQueryParameters.new # SigningRequestDtoCollectionQueryParameters | 
}

begin
  # Get signing requests count
  result = api_instance.get_signing_requests_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->get_signing_requests_count_async: #{e}"
end
```

#### Using the get_signing_requests_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_signing_requests_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get signing requests count
  data, status_code, headers = api_instance.get_signing_requests_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->get_signing_requests_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signing_request_dto_collection_query_parameters** | [**SigningRequestDtoCollectionQueryParameters**](SigningRequestDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## prepare_and_create_async

> <SigningRequestDto> prepare_and_create_async(tenant_id, opts)

Create, store, freeze a document and open a signing request in one call

Server-owned flow (T-UX4): creates a SignedDocument from the uploaded source, stores it, freezes it, then creates a signing request over the frozen artifact and attaches its signers — all in one unit of work. Evidence truth (status/hashes/ids/tokens) is server-produced; the caller supplies intent only. The server generates the new document id.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  file: File.new('/path/to/some/file'), # File | 
  title: 'title_example', # String | 
  contact_id: 'contact_id_example', # String | 
  routing_mode: 'Parallel', # String | 
  expires_at_utc: Time.parse('2013-10-20T19:20:30+01:00'), # Time | 
  message: 'message_example', # String | 
  correlation_id: 'correlation_id_example', # String | 
  external_reference: 'external_reference_example', # String | 
  signers: 'signers_example' # String | 
}

begin
  # Create, store, freeze a document and open a signing request in one call
  result = api_instance.prepare_and_create_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->prepare_and_create_async: #{e}"
end
```

#### Using the prepare_and_create_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SigningRequestDto>, Integer, Hash)> prepare_and_create_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create, store, freeze a document and open a signing request in one call
  data, status_code, headers = api_instance.prepare_and_create_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SigningRequestDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->prepare_and_create_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **file** | **File** |  | [optional] |
| **title** | **String** |  | [optional] |
| **contact_id** | **String** |  | [optional] |
| **routing_mode** | **String** |  | [optional] |
| **expires_at_utc** | **Time** |  | [optional] |
| **message** | **String** |  | [optional] |
| **correlation_id** | **String** |  | [optional] |
| **external_reference** | **String** |  | [optional] |
| **signers** | **String** |  | [optional] |

### Return type

[**SigningRequestDto**](SigningRequestDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data, application/json, application/xml
- **Accept**: application/json, application/xml


## send_async

> send_async(tenant_id, id, opts)

Send a signing request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = 'id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Send a signing request
  api_instance.send_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->send_async: #{e}"
end
```

#### Using the send_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> send_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Send a signing request
  data, status_code, headers = api_instance.send_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->send_async_with_http_info: #{e}"
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


## void_async

> void_async(tenant_id, id, opts)

Void a signing request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningRequestsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = 'id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  void_signing_request_dto: OpenapiClient::VoidSigningRequestDto.new # VoidSigningRequestDto | 
}

begin
  # Void a signing request
  api_instance.void_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->void_async: #{e}"
end
```

#### Using the void_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> void_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Void a signing request
  data, status_code, headers = api_instance.void_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningRequestsApi->void_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **void_signing_request_dto** | [**VoidSigningRequestDto**](VoidSigningRequestDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: Not defined

