# OpenapiClient::ProofsOfDeliveryApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**add_proof_of_delivery_line_async**](ProofsOfDeliveryApi.md#add_proof_of_delivery_line_async) | **POST** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/Lines | Add a line to proof of delivery |
| [**attach_delivery_note_async**](ProofsOfDeliveryApi.md#attach_delivery_note_async) | **POST** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/DeliveryNotes/{noteId} | Attach a delivery note |
| [**create_proof_of_delivery_async**](ProofsOfDeliveryApi.md#create_proof_of_delivery_async) | **POST** /api/v2/LogisticsService/ProofsOfDelivery | Create a proof of delivery |
| [**delete_proof_of_delivery_async**](ProofsOfDeliveryApi.md#delete_proof_of_delivery_async) | **DELETE** /api/v2/LogisticsService/ProofsOfDelivery/{podId} | Delete a proof of delivery |
| [**detach_delivery_note_async**](ProofsOfDeliveryApi.md#detach_delivery_note_async) | **DELETE** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/DeliveryNotes/{noteId} | Detach a delivery note |
| [**dispute_proof_of_delivery_async**](ProofsOfDeliveryApi.md#dispute_proof_of_delivery_async) | **POST** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/Dispute | Dispute a proof of delivery |
| [**get_proof_of_delivery_by_id_async**](ProofsOfDeliveryApi.md#get_proof_of_delivery_by_id_async) | **GET** /api/v2/LogisticsService/ProofsOfDelivery/{podId} | Get proof of delivery by ID |
| [**get_proof_of_delivery_delivery_notes_async**](ProofsOfDeliveryApi.md#get_proof_of_delivery_delivery_notes_async) | **GET** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/DeliveryNotes | Get attached delivery notes |
| [**get_proof_of_delivery_delivery_notes_count_async**](ProofsOfDeliveryApi.md#get_proof_of_delivery_delivery_notes_count_async) | **GET** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/DeliveryNotes/Count | Get delivery notes count |
| [**get_proof_of_delivery_lines_async**](ProofsOfDeliveryApi.md#get_proof_of_delivery_lines_async) | **GET** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/Lines | Get proof of delivery lines |
| [**get_proof_of_delivery_lines_count_async**](ProofsOfDeliveryApi.md#get_proof_of_delivery_lines_count_async) | **GET** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/Lines/Count | Get proof of delivery lines count |
| [**get_proofs_of_delivery_async**](ProofsOfDeliveryApi.md#get_proofs_of_delivery_async) | **GET** /api/v2/LogisticsService/ProofsOfDelivery | Get all proofs of delivery |
| [**get_proofs_of_delivery_count_async**](ProofsOfDeliveryApi.md#get_proofs_of_delivery_count_async) | **GET** /api/v2/LogisticsService/ProofsOfDelivery/Count | Get proofs of delivery count |
| [**reject_proof_of_delivery_async**](ProofsOfDeliveryApi.md#reject_proof_of_delivery_async) | **POST** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/Reject | Reject a proof of delivery |
| [**remove_proof_of_delivery_line_async**](ProofsOfDeliveryApi.md#remove_proof_of_delivery_line_async) | **DELETE** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/Lines/{lineId} | Remove a proof of delivery line |
| [**sign_proof_of_delivery_async**](ProofsOfDeliveryApi.md#sign_proof_of_delivery_async) | **POST** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/Sign | Sign a proof of delivery |
| [**update_proof_of_delivery_async**](ProofsOfDeliveryApi.md#update_proof_of_delivery_async) | **PUT** /api/v2/LogisticsService/ProofsOfDelivery/{podId} | Update a proof of delivery |
| [**update_proof_of_delivery_line_async**](ProofsOfDeliveryApi.md#update_proof_of_delivery_line_async) | **PUT** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/Lines/{lineId} | Update a proof of delivery line |


## add_proof_of_delivery_line_async

> <EmptyEnvelope> add_proof_of_delivery_line_async(tenant_id, pod_id, opts)

Add a line to proof of delivery

Adds a new line to a proof of delivery.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProofsOfDeliveryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pod_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  proof_of_delivery_line_create_dto: OpenapiClient::ProofOfDeliveryLineCreateDto.new # ProofOfDeliveryLineCreateDto | 
}

begin
  # Add a line to proof of delivery
  result = api_instance.add_proof_of_delivery_line_async(tenant_id, pod_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->add_proof_of_delivery_line_async: #{e}"
end
```

#### Using the add_proof_of_delivery_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> add_proof_of_delivery_line_async_with_http_info(tenant_id, pod_id, opts)

```ruby
begin
  # Add a line to proof of delivery
  data, status_code, headers = api_instance.add_proof_of_delivery_line_async_with_http_info(tenant_id, pod_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->add_proof_of_delivery_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pod_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **proof_of_delivery_line_create_dto** | [**ProofOfDeliveryLineCreateDto**](ProofOfDeliveryLineCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## attach_delivery_note_async

> <EmptyEnvelope> attach_delivery_note_async(tenant_id, pod_id, note_id, opts)

Attach a delivery note

Attaches a delivery note to a proof of delivery.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProofsOfDeliveryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pod_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
note_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Attach a delivery note
  result = api_instance.attach_delivery_note_async(tenant_id, pod_id, note_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->attach_delivery_note_async: #{e}"
end
```

#### Using the attach_delivery_note_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> attach_delivery_note_async_with_http_info(tenant_id, pod_id, note_id, opts)

```ruby
begin
  # Attach a delivery note
  data, status_code, headers = api_instance.attach_delivery_note_async_with_http_info(tenant_id, pod_id, note_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->attach_delivery_note_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pod_id** | **String** |  |  |
| **note_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_proof_of_delivery_async

> <EmptyEnvelope> create_proof_of_delivery_async(tenant_id, opts)

Create a proof of delivery

Creates a new proof of delivery for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProofsOfDeliveryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  proof_of_delivery_create_dto: OpenapiClient::ProofOfDeliveryCreateDto.new # ProofOfDeliveryCreateDto | 
}

begin
  # Create a proof of delivery
  result = api_instance.create_proof_of_delivery_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->create_proof_of_delivery_async: #{e}"
end
```

#### Using the create_proof_of_delivery_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_proof_of_delivery_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a proof of delivery
  data, status_code, headers = api_instance.create_proof_of_delivery_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->create_proof_of_delivery_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **proof_of_delivery_create_dto** | [**ProofOfDeliveryCreateDto**](ProofOfDeliveryCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_proof_of_delivery_async

> <EmptyEnvelope> delete_proof_of_delivery_async(tenant_id, pod_id, opts)

Delete a proof of delivery

Deletes a proof of delivery.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProofsOfDeliveryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pod_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a proof of delivery
  result = api_instance.delete_proof_of_delivery_async(tenant_id, pod_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->delete_proof_of_delivery_async: #{e}"
end
```

#### Using the delete_proof_of_delivery_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_proof_of_delivery_async_with_http_info(tenant_id, pod_id, opts)

```ruby
begin
  # Delete a proof of delivery
  data, status_code, headers = api_instance.delete_proof_of_delivery_async_with_http_info(tenant_id, pod_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->delete_proof_of_delivery_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pod_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## detach_delivery_note_async

> <EmptyEnvelope> detach_delivery_note_async(tenant_id, pod_id, note_id, opts)

Detach a delivery note

Detaches a delivery note from a proof of delivery.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProofsOfDeliveryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pod_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
note_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Detach a delivery note
  result = api_instance.detach_delivery_note_async(tenant_id, pod_id, note_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->detach_delivery_note_async: #{e}"
end
```

#### Using the detach_delivery_note_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> detach_delivery_note_async_with_http_info(tenant_id, pod_id, note_id, opts)

```ruby
begin
  # Detach a delivery note
  data, status_code, headers = api_instance.detach_delivery_note_async_with_http_info(tenant_id, pod_id, note_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->detach_delivery_note_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pod_id** | **String** |  |  |
| **note_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## dispute_proof_of_delivery_async

> <EmptyEnvelope> dispute_proof_of_delivery_async(tenant_id, pod_id, opts)

Dispute a proof of delivery

Disputes a proof of delivery.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProofsOfDeliveryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pod_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  dispute_proof_of_delivery_request: OpenapiClient::DisputeProofOfDeliveryRequest.new # DisputeProofOfDeliveryRequest | 
}

begin
  # Dispute a proof of delivery
  result = api_instance.dispute_proof_of_delivery_async(tenant_id, pod_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->dispute_proof_of_delivery_async: #{e}"
end
```

#### Using the dispute_proof_of_delivery_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> dispute_proof_of_delivery_async_with_http_info(tenant_id, pod_id, opts)

```ruby
begin
  # Dispute a proof of delivery
  data, status_code, headers = api_instance.dispute_proof_of_delivery_async_with_http_info(tenant_id, pod_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->dispute_proof_of_delivery_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pod_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **dispute_proof_of_delivery_request** | [**DisputeProofOfDeliveryRequest**](DisputeProofOfDeliveryRequest.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_proof_of_delivery_by_id_async

> <ProofOfDeliveryDtoEnvelope> get_proof_of_delivery_by_id_async(tenant_id, pod_id, opts)

Get proof of delivery by ID

Retrieves a specific proof of delivery by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProofsOfDeliveryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pod_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get proof of delivery by ID
  result = api_instance.get_proof_of_delivery_by_id_async(tenant_id, pod_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->get_proof_of_delivery_by_id_async: #{e}"
end
```

#### Using the get_proof_of_delivery_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ProofOfDeliveryDtoEnvelope>, Integer, Hash)> get_proof_of_delivery_by_id_async_with_http_info(tenant_id, pod_id, opts)

```ruby
begin
  # Get proof of delivery by ID
  data, status_code, headers = api_instance.get_proof_of_delivery_by_id_async_with_http_info(tenant_id, pod_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ProofOfDeliveryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->get_proof_of_delivery_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pod_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ProofOfDeliveryDtoEnvelope**](ProofOfDeliveryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_proof_of_delivery_delivery_notes_async

> <DeliveryNoteDtoListEnvelope> get_proof_of_delivery_delivery_notes_async(tenant_id, pod_id, opts)

Get attached delivery notes

Retrieves all delivery notes attached to a proof of delivery.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProofsOfDeliveryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pod_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get attached delivery notes
  result = api_instance.get_proof_of_delivery_delivery_notes_async(tenant_id, pod_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->get_proof_of_delivery_delivery_notes_async: #{e}"
end
```

#### Using the get_proof_of_delivery_delivery_notes_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<DeliveryNoteDtoListEnvelope>, Integer, Hash)> get_proof_of_delivery_delivery_notes_async_with_http_info(tenant_id, pod_id, opts)

```ruby
begin
  # Get attached delivery notes
  data, status_code, headers = api_instance.get_proof_of_delivery_delivery_notes_async_with_http_info(tenant_id, pod_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <DeliveryNoteDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->get_proof_of_delivery_delivery_notes_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pod_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**DeliveryNoteDtoListEnvelope**](DeliveryNoteDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_proof_of_delivery_delivery_notes_count_async

> <Int32Envelope> get_proof_of_delivery_delivery_notes_count_async(tenant_id, pod_id, opts)

Get delivery notes count

Returns the count of delivery notes attached to a proof of delivery.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProofsOfDeliveryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pod_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get delivery notes count
  result = api_instance.get_proof_of_delivery_delivery_notes_count_async(tenant_id, pod_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->get_proof_of_delivery_delivery_notes_count_async: #{e}"
end
```

#### Using the get_proof_of_delivery_delivery_notes_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_proof_of_delivery_delivery_notes_count_async_with_http_info(tenant_id, pod_id, opts)

```ruby
begin
  # Get delivery notes count
  data, status_code, headers = api_instance.get_proof_of_delivery_delivery_notes_count_async_with_http_info(tenant_id, pod_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->get_proof_of_delivery_delivery_notes_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pod_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_proof_of_delivery_lines_async

> <ProofOfDeliveryLineDtoListEnvelope> get_proof_of_delivery_lines_async(tenant_id, pod_id, opts)

Get proof of delivery lines

Retrieves all lines for a specific proof of delivery.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProofsOfDeliveryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pod_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get proof of delivery lines
  result = api_instance.get_proof_of_delivery_lines_async(tenant_id, pod_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->get_proof_of_delivery_lines_async: #{e}"
end
```

#### Using the get_proof_of_delivery_lines_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ProofOfDeliveryLineDtoListEnvelope>, Integer, Hash)> get_proof_of_delivery_lines_async_with_http_info(tenant_id, pod_id, opts)

```ruby
begin
  # Get proof of delivery lines
  data, status_code, headers = api_instance.get_proof_of_delivery_lines_async_with_http_info(tenant_id, pod_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ProofOfDeliveryLineDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->get_proof_of_delivery_lines_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pod_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ProofOfDeliveryLineDtoListEnvelope**](ProofOfDeliveryLineDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_proof_of_delivery_lines_count_async

> <Int32Envelope> get_proof_of_delivery_lines_count_async(tenant_id, pod_id, opts)

Get proof of delivery lines count

Returns the count of lines for a specific proof of delivery.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProofsOfDeliveryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pod_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get proof of delivery lines count
  result = api_instance.get_proof_of_delivery_lines_count_async(tenant_id, pod_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->get_proof_of_delivery_lines_count_async: #{e}"
end
```

#### Using the get_proof_of_delivery_lines_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_proof_of_delivery_lines_count_async_with_http_info(tenant_id, pod_id, opts)

```ruby
begin
  # Get proof of delivery lines count
  data, status_code, headers = api_instance.get_proof_of_delivery_lines_count_async_with_http_info(tenant_id, pod_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->get_proof_of_delivery_lines_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pod_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_proofs_of_delivery_async

> <ProofOfDeliveryDtoListEnvelope> get_proofs_of_delivery_async(tenant_id, opts)

Get all proofs of delivery

Retrieves all proofs of delivery for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProofsOfDeliveryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all proofs of delivery
  result = api_instance.get_proofs_of_delivery_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->get_proofs_of_delivery_async: #{e}"
end
```

#### Using the get_proofs_of_delivery_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ProofOfDeliveryDtoListEnvelope>, Integer, Hash)> get_proofs_of_delivery_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all proofs of delivery
  data, status_code, headers = api_instance.get_proofs_of_delivery_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ProofOfDeliveryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->get_proofs_of_delivery_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ProofOfDeliveryDtoListEnvelope**](ProofOfDeliveryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_proofs_of_delivery_count_async

> <Int32Envelope> get_proofs_of_delivery_count_async(tenant_id, opts)

Get proofs of delivery count

Returns the count of proofs of delivery for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProofsOfDeliveryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get proofs of delivery count
  result = api_instance.get_proofs_of_delivery_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->get_proofs_of_delivery_count_async: #{e}"
end
```

#### Using the get_proofs_of_delivery_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_proofs_of_delivery_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get proofs of delivery count
  data, status_code, headers = api_instance.get_proofs_of_delivery_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->get_proofs_of_delivery_count_async_with_http_info: #{e}"
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


## reject_proof_of_delivery_async

> <EmptyEnvelope> reject_proof_of_delivery_async(tenant_id, pod_id, opts)

Reject a proof of delivery

Rejects a proof of delivery.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProofsOfDeliveryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pod_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  reject_proof_of_delivery_request: OpenapiClient::RejectProofOfDeliveryRequest.new # RejectProofOfDeliveryRequest | 
}

begin
  # Reject a proof of delivery
  result = api_instance.reject_proof_of_delivery_async(tenant_id, pod_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->reject_proof_of_delivery_async: #{e}"
end
```

#### Using the reject_proof_of_delivery_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> reject_proof_of_delivery_async_with_http_info(tenant_id, pod_id, opts)

```ruby
begin
  # Reject a proof of delivery
  data, status_code, headers = api_instance.reject_proof_of_delivery_async_with_http_info(tenant_id, pod_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->reject_proof_of_delivery_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pod_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **reject_proof_of_delivery_request** | [**RejectProofOfDeliveryRequest**](RejectProofOfDeliveryRequest.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## remove_proof_of_delivery_line_async

> <EmptyEnvelope> remove_proof_of_delivery_line_async(tenant_id, pod_id, line_id, opts)

Remove a proof of delivery line

Removes a line from a proof of delivery.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProofsOfDeliveryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pod_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove a proof of delivery line
  result = api_instance.remove_proof_of_delivery_line_async(tenant_id, pod_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->remove_proof_of_delivery_line_async: #{e}"
end
```

#### Using the remove_proof_of_delivery_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> remove_proof_of_delivery_line_async_with_http_info(tenant_id, pod_id, line_id, opts)

```ruby
begin
  # Remove a proof of delivery line
  data, status_code, headers = api_instance.remove_proof_of_delivery_line_async_with_http_info(tenant_id, pod_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->remove_proof_of_delivery_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pod_id** | **String** |  |  |
| **line_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## sign_proof_of_delivery_async

> <EmptyEnvelope> sign_proof_of_delivery_async(tenant_id, pod_id, opts)

Sign a proof of delivery

Signs a proof of delivery.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProofsOfDeliveryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pod_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  sign_proof_of_delivery_request: OpenapiClient::SignProofOfDeliveryRequest.new # SignProofOfDeliveryRequest | 
}

begin
  # Sign a proof of delivery
  result = api_instance.sign_proof_of_delivery_async(tenant_id, pod_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->sign_proof_of_delivery_async: #{e}"
end
```

#### Using the sign_proof_of_delivery_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> sign_proof_of_delivery_async_with_http_info(tenant_id, pod_id, opts)

```ruby
begin
  # Sign a proof of delivery
  data, status_code, headers = api_instance.sign_proof_of_delivery_async_with_http_info(tenant_id, pod_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->sign_proof_of_delivery_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pod_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **sign_proof_of_delivery_request** | [**SignProofOfDeliveryRequest**](SignProofOfDeliveryRequest.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_proof_of_delivery_async

> <EmptyEnvelope> update_proof_of_delivery_async(tenant_id, pod_id, opts)

Update a proof of delivery

Updates an existing proof of delivery.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProofsOfDeliveryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pod_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  proof_of_delivery_update_dto: OpenapiClient::ProofOfDeliveryUpdateDto.new # ProofOfDeliveryUpdateDto | 
}

begin
  # Update a proof of delivery
  result = api_instance.update_proof_of_delivery_async(tenant_id, pod_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->update_proof_of_delivery_async: #{e}"
end
```

#### Using the update_proof_of_delivery_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_proof_of_delivery_async_with_http_info(tenant_id, pod_id, opts)

```ruby
begin
  # Update a proof of delivery
  data, status_code, headers = api_instance.update_proof_of_delivery_async_with_http_info(tenant_id, pod_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->update_proof_of_delivery_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pod_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **proof_of_delivery_update_dto** | [**ProofOfDeliveryUpdateDto**](ProofOfDeliveryUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_proof_of_delivery_line_async

> <EmptyEnvelope> update_proof_of_delivery_line_async(tenant_id, pod_id, line_id, opts)

Update a proof of delivery line

Updates an existing line on a proof of delivery.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProofsOfDeliveryApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pod_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  proof_of_delivery_line_update_dto: OpenapiClient::ProofOfDeliveryLineUpdateDto.new # ProofOfDeliveryLineUpdateDto | 
}

begin
  # Update a proof of delivery line
  result = api_instance.update_proof_of_delivery_line_async(tenant_id, pod_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->update_proof_of_delivery_line_async: #{e}"
end
```

#### Using the update_proof_of_delivery_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_proof_of_delivery_line_async_with_http_info(tenant_id, pod_id, line_id, opts)

```ruby
begin
  # Update a proof of delivery line
  data, status_code, headers = api_instance.update_proof_of_delivery_line_async_with_http_info(tenant_id, pod_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProofsOfDeliveryApi->update_proof_of_delivery_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pod_id** | **String** |  |  |
| **line_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **proof_of_delivery_line_update_dto** | [**ProofOfDeliveryLineUpdateDto**](ProofOfDeliveryLineUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

