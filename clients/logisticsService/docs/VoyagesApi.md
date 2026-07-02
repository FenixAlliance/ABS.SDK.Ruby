# OpenapiClient::VoyagesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**cancel_voyage_async**](VoyagesApi.md#cancel_voyage_async) | **POST** /api/v2/LogisticsService/Voyages/{voyageId}/Cancel | Cancel a voyage |
| [**complete_voyage_async**](VoyagesApi.md#complete_voyage_async) | **POST** /api/v2/LogisticsService/Voyages/{voyageId}/Complete | Complete a voyage |
| [**create_voyage_async**](VoyagesApi.md#create_voyage_async) | **POST** /api/v2/LogisticsService/Voyages | Create a voyage |
| [**create_voyage_port_call_async**](VoyagesApi.md#create_voyage_port_call_async) | **POST** /api/v2/LogisticsService/Voyages/{voyageId}/PortCalls | Create a port call |
| [**delete_voyage_async**](VoyagesApi.md#delete_voyage_async) | **DELETE** /api/v2/LogisticsService/Voyages/{voyageId} | Delete a voyage |
| [**delete_voyage_port_call_async**](VoyagesApi.md#delete_voyage_port_call_async) | **DELETE** /api/v2/LogisticsService/Voyages/{voyageId}/PortCalls/{portCallId} | Delete a port call |
| [**get_voyage_by_id_async**](VoyagesApi.md#get_voyage_by_id_async) | **GET** /api/v2/LogisticsService/Voyages/{voyageId} | Get voyage by ID |
| [**get_voyage_port_calls_async**](VoyagesApi.md#get_voyage_port_calls_async) | **GET** /api/v2/LogisticsService/Voyages/{voyageId}/PortCalls | Get voyage port calls |
| [**get_voyage_port_calls_count_async**](VoyagesApi.md#get_voyage_port_calls_count_async) | **GET** /api/v2/LogisticsService/Voyages/{voyageId}/PortCalls/Count | Get voyage port calls count |
| [**get_voyages_async**](VoyagesApi.md#get_voyages_async) | **GET** /api/v2/LogisticsService/Voyages | Get all voyages |
| [**get_voyages_count_async**](VoyagesApi.md#get_voyages_count_async) | **GET** /api/v2/LogisticsService/Voyages/Count | Get voyages count |
| [**patch_voyage_async**](VoyagesApi.md#patch_voyage_async) | **PATCH** /api/v2/LogisticsService/Voyages/{voyageId} | Patch a voyage |
| [**patch_voyage_port_call_async**](VoyagesApi.md#patch_voyage_port_call_async) | **PATCH** /api/v2/LogisticsService/Voyages/{voyageId}/PortCalls/{portCallId} | Patch a voyage port call |
| [**start_voyage_async**](VoyagesApi.md#start_voyage_async) | **POST** /api/v2/LogisticsService/Voyages/{voyageId}/Start | Start a voyage |
| [**update_voyage_async**](VoyagesApi.md#update_voyage_async) | **PUT** /api/v2/LogisticsService/Voyages/{voyageId} | Update a voyage |
| [**update_voyage_port_call_async**](VoyagesApi.md#update_voyage_port_call_async) | **PUT** /api/v2/LogisticsService/Voyages/{voyageId}/PortCalls/{portCallId} | Update a port call |


## cancel_voyage_async

> <EmptyEnvelope> cancel_voyage_async(tenant_id, voyage_id, opts)

Cancel a voyage

Cancels a voyage.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VoyagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
voyage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Cancel a voyage
  result = api_instance.cancel_voyage_async(tenant_id, voyage_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->cancel_voyage_async: #{e}"
end
```

#### Using the cancel_voyage_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> cancel_voyage_async_with_http_info(tenant_id, voyage_id, opts)

```ruby
begin
  # Cancel a voyage
  data, status_code, headers = api_instance.cancel_voyage_async_with_http_info(tenant_id, voyage_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->cancel_voyage_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **voyage_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## complete_voyage_async

> <EmptyEnvelope> complete_voyage_async(tenant_id, voyage_id, opts)

Complete a voyage

Marks a voyage as completed.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VoyagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
voyage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Complete a voyage
  result = api_instance.complete_voyage_async(tenant_id, voyage_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->complete_voyage_async: #{e}"
end
```

#### Using the complete_voyage_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> complete_voyage_async_with_http_info(tenant_id, voyage_id, opts)

```ruby
begin
  # Complete a voyage
  data, status_code, headers = api_instance.complete_voyage_async_with_http_info(tenant_id, voyage_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->complete_voyage_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **voyage_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_voyage_async

> <EmptyEnvelope> create_voyage_async(tenant_id, opts)

Create a voyage

Creates a new voyage for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VoyagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  voyage_create_dto: OpenapiClient::VoyageCreateDto.new # VoyageCreateDto | 
}

begin
  # Create a voyage
  result = api_instance.create_voyage_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->create_voyage_async: #{e}"
end
```

#### Using the create_voyage_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_voyage_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a voyage
  data, status_code, headers = api_instance.create_voyage_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->create_voyage_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **voyage_create_dto** | [**VoyageCreateDto**](VoyageCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_voyage_port_call_async

> <EmptyEnvelope> create_voyage_port_call_async(tenant_id, voyage_id, opts)

Create a port call

Creates a new port call for a voyage.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VoyagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
voyage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  voyage_port_call_create_dto: OpenapiClient::VoyagePortCallCreateDto.new # VoyagePortCallCreateDto | 
}

begin
  # Create a port call
  result = api_instance.create_voyage_port_call_async(tenant_id, voyage_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->create_voyage_port_call_async: #{e}"
end
```

#### Using the create_voyage_port_call_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_voyage_port_call_async_with_http_info(tenant_id, voyage_id, opts)

```ruby
begin
  # Create a port call
  data, status_code, headers = api_instance.create_voyage_port_call_async_with_http_info(tenant_id, voyage_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->create_voyage_port_call_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **voyage_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **voyage_port_call_create_dto** | [**VoyagePortCallCreateDto**](VoyagePortCallCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_voyage_async

> <EmptyEnvelope> delete_voyage_async(tenant_id, voyage_id, opts)

Delete a voyage

Deletes a voyage.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VoyagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
voyage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a voyage
  result = api_instance.delete_voyage_async(tenant_id, voyage_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->delete_voyage_async: #{e}"
end
```

#### Using the delete_voyage_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_voyage_async_with_http_info(tenant_id, voyage_id, opts)

```ruby
begin
  # Delete a voyage
  data, status_code, headers = api_instance.delete_voyage_async_with_http_info(tenant_id, voyage_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->delete_voyage_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **voyage_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_voyage_port_call_async

> <EmptyEnvelope> delete_voyage_port_call_async(tenant_id, voyage_id, port_call_id, opts)

Delete a port call

Deletes a port call.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VoyagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
voyage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
port_call_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a port call
  result = api_instance.delete_voyage_port_call_async(tenant_id, voyage_id, port_call_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->delete_voyage_port_call_async: #{e}"
end
```

#### Using the delete_voyage_port_call_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_voyage_port_call_async_with_http_info(tenant_id, voyage_id, port_call_id, opts)

```ruby
begin
  # Delete a port call
  data, status_code, headers = api_instance.delete_voyage_port_call_async_with_http_info(tenant_id, voyage_id, port_call_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->delete_voyage_port_call_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **voyage_id** | **String** |  |  |
| **port_call_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_voyage_by_id_async

> <VoyageDtoEnvelope> get_voyage_by_id_async(tenant_id, voyage_id, opts)

Get voyage by ID

Retrieves a specific voyage by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VoyagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
voyage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get voyage by ID
  result = api_instance.get_voyage_by_id_async(tenant_id, voyage_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->get_voyage_by_id_async: #{e}"
end
```

#### Using the get_voyage_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<VoyageDtoEnvelope>, Integer, Hash)> get_voyage_by_id_async_with_http_info(tenant_id, voyage_id, opts)

```ruby
begin
  # Get voyage by ID
  data, status_code, headers = api_instance.get_voyage_by_id_async_with_http_info(tenant_id, voyage_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <VoyageDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->get_voyage_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **voyage_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**VoyageDtoEnvelope**](VoyageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_voyage_port_calls_async

> <VoyagePortCallDtoListEnvelope> get_voyage_port_calls_async(tenant_id, voyage_id, opts)

Get voyage port calls

Retrieves all port calls for a specific voyage.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VoyagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
voyage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get voyage port calls
  result = api_instance.get_voyage_port_calls_async(tenant_id, voyage_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->get_voyage_port_calls_async: #{e}"
end
```

#### Using the get_voyage_port_calls_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<VoyagePortCallDtoListEnvelope>, Integer, Hash)> get_voyage_port_calls_async_with_http_info(tenant_id, voyage_id, opts)

```ruby
begin
  # Get voyage port calls
  data, status_code, headers = api_instance.get_voyage_port_calls_async_with_http_info(tenant_id, voyage_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <VoyagePortCallDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->get_voyage_port_calls_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **voyage_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**VoyagePortCallDtoListEnvelope**](VoyagePortCallDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_voyage_port_calls_count_async

> <Int32Envelope> get_voyage_port_calls_count_async(tenant_id, voyage_id, opts)

Get voyage port calls count

Returns the count of port calls for a specific voyage.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VoyagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
voyage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get voyage port calls count
  result = api_instance.get_voyage_port_calls_count_async(tenant_id, voyage_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->get_voyage_port_calls_count_async: #{e}"
end
```

#### Using the get_voyage_port_calls_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_voyage_port_calls_count_async_with_http_info(tenant_id, voyage_id, opts)

```ruby
begin
  # Get voyage port calls count
  data, status_code, headers = api_instance.get_voyage_port_calls_count_async_with_http_info(tenant_id, voyage_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->get_voyage_port_calls_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **voyage_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_voyages_async

> <VoyageDtoListEnvelope> get_voyages_async(tenant_id, opts)

Get all voyages

Retrieves all voyages for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VoyagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all voyages
  result = api_instance.get_voyages_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->get_voyages_async: #{e}"
end
```

#### Using the get_voyages_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<VoyageDtoListEnvelope>, Integer, Hash)> get_voyages_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all voyages
  data, status_code, headers = api_instance.get_voyages_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <VoyageDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->get_voyages_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**VoyageDtoListEnvelope**](VoyageDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_voyages_count_async

> <Int32Envelope> get_voyages_count_async(tenant_id, opts)

Get voyages count

Returns the count of voyages for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VoyagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get voyages count
  result = api_instance.get_voyages_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->get_voyages_count_async: #{e}"
end
```

#### Using the get_voyages_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_voyages_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get voyages count
  data, status_code, headers = api_instance.get_voyages_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->get_voyages_count_async_with_http_info: #{e}"
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


## patch_voyage_async

> <EmptyEnvelope> patch_voyage_async(tenant_id, voyage_id, opts)

Patch a voyage

Partially updates an existing voyage using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VoyagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
voyage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a voyage
  result = api_instance.patch_voyage_async(tenant_id, voyage_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->patch_voyage_async: #{e}"
end
```

#### Using the patch_voyage_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_voyage_async_with_http_info(tenant_id, voyage_id, opts)

```ruby
begin
  # Patch a voyage
  data, status_code, headers = api_instance.patch_voyage_async_with_http_info(tenant_id, voyage_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->patch_voyage_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **voyage_id** | **String** |  |  |
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


## patch_voyage_port_call_async

> <EmptyEnvelope> patch_voyage_port_call_async(tenant_id, voyage_id, port_call_id, opts)

Patch a voyage port call

Partially updates an existing voyage port call using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VoyagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
voyage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
port_call_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a voyage port call
  result = api_instance.patch_voyage_port_call_async(tenant_id, voyage_id, port_call_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->patch_voyage_port_call_async: #{e}"
end
```

#### Using the patch_voyage_port_call_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_voyage_port_call_async_with_http_info(tenant_id, voyage_id, port_call_id, opts)

```ruby
begin
  # Patch a voyage port call
  data, status_code, headers = api_instance.patch_voyage_port_call_async_with_http_info(tenant_id, voyage_id, port_call_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->patch_voyage_port_call_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **voyage_id** | **String** |  |  |
| **port_call_id** | **String** |  |  |
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


## start_voyage_async

> <EmptyEnvelope> start_voyage_async(tenant_id, voyage_id, opts)

Start a voyage

Starts a voyage.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VoyagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
voyage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Start a voyage
  result = api_instance.start_voyage_async(tenant_id, voyage_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->start_voyage_async: #{e}"
end
```

#### Using the start_voyage_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> start_voyage_async_with_http_info(tenant_id, voyage_id, opts)

```ruby
begin
  # Start a voyage
  data, status_code, headers = api_instance.start_voyage_async_with_http_info(tenant_id, voyage_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->start_voyage_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **voyage_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_voyage_async

> <EmptyEnvelope> update_voyage_async(tenant_id, voyage_id, opts)

Update a voyage

Updates an existing voyage.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VoyagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
voyage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  voyage_update_dto: OpenapiClient::VoyageUpdateDto.new # VoyageUpdateDto | 
}

begin
  # Update a voyage
  result = api_instance.update_voyage_async(tenant_id, voyage_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->update_voyage_async: #{e}"
end
```

#### Using the update_voyage_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_voyage_async_with_http_info(tenant_id, voyage_id, opts)

```ruby
begin
  # Update a voyage
  data, status_code, headers = api_instance.update_voyage_async_with_http_info(tenant_id, voyage_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->update_voyage_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **voyage_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **voyage_update_dto** | [**VoyageUpdateDto**](VoyageUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_voyage_port_call_async

> <EmptyEnvelope> update_voyage_port_call_async(tenant_id, voyage_id, port_call_id, opts)

Update a port call

Updates an existing port call.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::VoyagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
voyage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
port_call_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  voyage_port_call_update_dto: OpenapiClient::VoyagePortCallUpdateDto.new # VoyagePortCallUpdateDto | 
}

begin
  # Update a port call
  result = api_instance.update_voyage_port_call_async(tenant_id, voyage_id, port_call_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->update_voyage_port_call_async: #{e}"
end
```

#### Using the update_voyage_port_call_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_voyage_port_call_async_with_http_info(tenant_id, voyage_id, port_call_id, opts)

```ruby
begin
  # Update a port call
  data, status_code, headers = api_instance.update_voyage_port_call_async_with_http_info(tenant_id, voyage_id, port_call_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling VoyagesApi->update_voyage_port_call_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **voyage_id** | **String** |  |  |
| **port_call_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **voyage_port_call_update_dto** | [**VoyagePortCallUpdateDto**](VoyagePortCallUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

