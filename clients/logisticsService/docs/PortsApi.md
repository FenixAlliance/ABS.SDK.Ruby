# OpenapiClient::PortsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_port_async**](PortsApi.md#create_port_async) | **POST** /api/v2/LogisticsService/Ports | Create a port |
| [**delete_port_async**](PortsApi.md#delete_port_async) | **DELETE** /api/v2/LogisticsService/Ports/{portId} | Delete a port |
| [**get_port_by_id_async**](PortsApi.md#get_port_by_id_async) | **GET** /api/v2/LogisticsService/Ports/{portId} | Get port by ID |
| [**get_ports_async**](PortsApi.md#get_ports_async) | **GET** /api/v2/LogisticsService/Ports | Get all ports |
| [**get_ports_count_async**](PortsApi.md#get_ports_count_async) | **GET** /api/v2/LogisticsService/Ports/Count | Get ports count |
| [**patch_port_async**](PortsApi.md#patch_port_async) | **PATCH** /api/v2/LogisticsService/Ports/{portId} | Patch a port |
| [**update_port_async**](PortsApi.md#update_port_async) | **PUT** /api/v2/LogisticsService/Ports/{portId} | Update a port |


## create_port_async

> <EmptyEnvelope> create_port_async(tenant_id, opts)

Create a port

Creates a new port for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  port_create_dto: OpenapiClient::PortCreateDto.new({title: 'title_example', address1: 'address1_example'}) # PortCreateDto | 
}

begin
  # Create a port
  result = api_instance.create_port_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortsApi->create_port_async: #{e}"
end
```

#### Using the create_port_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_port_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a port
  data, status_code, headers = api_instance.create_port_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortsApi->create_port_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **port_create_dto** | [**PortCreateDto**](PortCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_port_async

> <EmptyEnvelope> delete_port_async(tenant_id, port_id, opts)

Delete a port

Deletes a port.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
port_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a port
  result = api_instance.delete_port_async(tenant_id, port_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortsApi->delete_port_async: #{e}"
end
```

#### Using the delete_port_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_port_async_with_http_info(tenant_id, port_id, opts)

```ruby
begin
  # Delete a port
  data, status_code, headers = api_instance.delete_port_async_with_http_info(tenant_id, port_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortsApi->delete_port_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **port_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_port_by_id_async

> <PortDtoEnvelope> get_port_by_id_async(tenant_id, port_id, opts)

Get port by ID

Retrieves a specific port by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
port_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get port by ID
  result = api_instance.get_port_by_id_async(tenant_id, port_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortsApi->get_port_by_id_async: #{e}"
end
```

#### Using the get_port_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PortDtoEnvelope>, Integer, Hash)> get_port_by_id_async_with_http_info(tenant_id, port_id, opts)

```ruby
begin
  # Get port by ID
  data, status_code, headers = api_instance.get_port_by_id_async_with_http_info(tenant_id, port_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PortDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortsApi->get_port_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **port_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PortDtoEnvelope**](PortDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_ports_async

> <PortDtoListEnvelope> get_ports_async(tenant_id, opts)

Get all ports

Retrieves all ports for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all ports
  result = api_instance.get_ports_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortsApi->get_ports_async: #{e}"
end
```

#### Using the get_ports_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PortDtoListEnvelope>, Integer, Hash)> get_ports_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all ports
  data, status_code, headers = api_instance.get_ports_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PortDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortsApi->get_ports_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PortDtoListEnvelope**](PortDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_ports_count_async

> <Int32Envelope> get_ports_count_async(tenant_id, opts)

Get ports count

Returns the count of ports for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get ports count
  result = api_instance.get_ports_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortsApi->get_ports_count_async: #{e}"
end
```

#### Using the get_ports_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_ports_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get ports count
  data, status_code, headers = api_instance.get_ports_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortsApi->get_ports_count_async_with_http_info: #{e}"
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


## patch_port_async

> <EmptyEnvelope> patch_port_async(tenant_id, port_id, opts)

Patch a port

Partially updates an existing port using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
port_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a port
  result = api_instance.patch_port_async(tenant_id, port_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortsApi->patch_port_async: #{e}"
end
```

#### Using the patch_port_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_port_async_with_http_info(tenant_id, port_id, opts)

```ruby
begin
  # Patch a port
  data, status_code, headers = api_instance.patch_port_async_with_http_info(tenant_id, port_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortsApi->patch_port_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **port_id** | **String** |  |  |
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


## update_port_async

> <EmptyEnvelope> update_port_async(tenant_id, port_id, opts)

Update a port

Updates an existing port.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
port_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  port_update_dto: OpenapiClient::PortUpdateDto.new # PortUpdateDto | 
}

begin
  # Update a port
  result = api_instance.update_port_async(tenant_id, port_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortsApi->update_port_async: #{e}"
end
```

#### Using the update_port_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_port_async_with_http_info(tenant_id, port_id, opts)

```ruby
begin
  # Update a port
  data, status_code, headers = api_instance.update_port_async_with_http_info(tenant_id, port_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortsApi->update_port_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **port_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **port_update_dto** | [**PortUpdateDto**](PortUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

