# OpenapiClient::ShipmentsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_shipment_async**](ShipmentsApi.md#create_shipment_async) | **POST** /api/v2/ShipmentsService/Shipments | Create a shipment |
| [**delete_shipment_async**](ShipmentsApi.md#delete_shipment_async) | **DELETE** /api/v2/ShipmentsService/Shipments/{shipmentId} | Delete a shipment |
| [**get_shipment_by_id_async**](ShipmentsApi.md#get_shipment_by_id_async) | **GET** /api/v2/ShipmentsService/Shipments/{shipmentId} | Get shipment by ID |
| [**get_shipments_async**](ShipmentsApi.md#get_shipments_async) | **GET** /api/v2/ShipmentsService/Shipments | Get all shipments |
| [**get_shipments_count_async**](ShipmentsApi.md#get_shipments_count_async) | **GET** /api/v2/ShipmentsService/Shipments/Count | Get shipments count |
| [**update_shipment_async**](ShipmentsApi.md#update_shipment_async) | **PUT** /api/v2/ShipmentsService/Shipments/{shipmentId} | Update a shipment |


## create_shipment_async

> create_shipment_async(tenant_id, opts)

Create a shipment

Creates a new shipment for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShipmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipment_create_dto: OpenapiClient::ShipmentCreateDto.new # ShipmentCreateDto | 
}

begin
  # Create a shipment
  api_instance.create_shipment_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShipmentsApi->create_shipment_async: #{e}"
end
```

#### Using the create_shipment_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_shipment_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a shipment
  data, status_code, headers = api_instance.create_shipment_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShipmentsApi->create_shipment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipment_create_dto** | [**ShipmentCreateDto**](ShipmentCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_shipment_async

> delete_shipment_async(tenant_id, shipment_id, opts)

Delete a shipment

Deletes a shipment.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShipmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
shipment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a shipment
  api_instance.delete_shipment_async(tenant_id, shipment_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShipmentsApi->delete_shipment_async: #{e}"
end
```

#### Using the delete_shipment_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_shipment_async_with_http_info(tenant_id, shipment_id, opts)

```ruby
begin
  # Delete a shipment
  data, status_code, headers = api_instance.delete_shipment_async_with_http_info(tenant_id, shipment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShipmentsApi->delete_shipment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **shipment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shipment_by_id_async

> <ShipmentDtoEnvelope> get_shipment_by_id_async(tenant_id, shipment_id, opts)

Get shipment by ID

Retrieves a specific shipment by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShipmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
shipment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get shipment by ID
  result = api_instance.get_shipment_by_id_async(tenant_id, shipment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShipmentsApi->get_shipment_by_id_async: #{e}"
end
```

#### Using the get_shipment_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShipmentDtoEnvelope>, Integer, Hash)> get_shipment_by_id_async_with_http_info(tenant_id, shipment_id, opts)

```ruby
begin
  # Get shipment by ID
  data, status_code, headers = api_instance.get_shipment_by_id_async_with_http_info(tenant_id, shipment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShipmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShipmentsApi->get_shipment_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **shipment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShipmentDtoEnvelope**](ShipmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shipments_async

> <ShipmentDtoListEnvelope> get_shipments_async(tenant_id, opts)

Get all shipments

Retrieves all shipments for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShipmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all shipments
  result = api_instance.get_shipments_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShipmentsApi->get_shipments_async: #{e}"
end
```

#### Using the get_shipments_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShipmentDtoListEnvelope>, Integer, Hash)> get_shipments_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all shipments
  data, status_code, headers = api_instance.get_shipments_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShipmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShipmentsApi->get_shipments_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShipmentDtoListEnvelope**](ShipmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shipments_count_async

> <Int32Envelope> get_shipments_count_async(tenant_id, opts)

Get shipments count

Returns the count of shipments for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShipmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get shipments count
  result = api_instance.get_shipments_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShipmentsApi->get_shipments_count_async: #{e}"
end
```

#### Using the get_shipments_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_shipments_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get shipments count
  data, status_code, headers = api_instance.get_shipments_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShipmentsApi->get_shipments_count_async_with_http_info: #{e}"
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


## update_shipment_async

> update_shipment_async(tenant_id, shipment_id, opts)

Update a shipment

Updates an existing shipment.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShipmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
shipment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shipment_update_dto: OpenapiClient::ShipmentUpdateDto.new # ShipmentUpdateDto | 
}

begin
  # Update a shipment
  api_instance.update_shipment_async(tenant_id, shipment_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShipmentsApi->update_shipment_async: #{e}"
end
```

#### Using the update_shipment_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_shipment_async_with_http_info(tenant_id, shipment_id, opts)

```ruby
begin
  # Update a shipment
  data, status_code, headers = api_instance.update_shipment_async_with_http_info(tenant_id, shipment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShipmentsApi->update_shipment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **shipment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shipment_update_dto** | [**ShipmentUpdateDto**](ShipmentUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

