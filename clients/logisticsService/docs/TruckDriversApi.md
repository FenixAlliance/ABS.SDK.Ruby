# OpenapiClient::TruckDriversApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**activate_truck_driver_async**](TruckDriversApi.md#activate_truck_driver_async) | **POST** /api/v2/LogisticsService/TruckDrivers/{driverId}/Activate | Activate a truck driver |
| [**create_truck_driver_async**](TruckDriversApi.md#create_truck_driver_async) | **POST** /api/v2/LogisticsService/TruckDrivers | Create a truck driver |
| [**deactivate_truck_driver_async**](TruckDriversApi.md#deactivate_truck_driver_async) | **POST** /api/v2/LogisticsService/TruckDrivers/{driverId}/Deactivate | Deactivate a truck driver |
| [**delete_truck_driver_async**](TruckDriversApi.md#delete_truck_driver_async) | **DELETE** /api/v2/LogisticsService/TruckDrivers/{driverId} | Delete a truck driver |
| [**get_truck_driver_by_id_async**](TruckDriversApi.md#get_truck_driver_by_id_async) | **GET** /api/v2/LogisticsService/TruckDrivers/{driverId} | Get truck driver by ID |
| [**get_truck_drivers_async**](TruckDriversApi.md#get_truck_drivers_async) | **GET** /api/v2/LogisticsService/TruckDrivers | Get all truck drivers |
| [**get_truck_drivers_count_async**](TruckDriversApi.md#get_truck_drivers_count_async) | **GET** /api/v2/LogisticsService/TruckDrivers/Count | Get truck drivers count |
| [**patch_truck_driver_async**](TruckDriversApi.md#patch_truck_driver_async) | **PATCH** /api/v2/LogisticsService/TruckDrivers/{driverId} | Patch a truck driver |
| [**update_truck_driver_async**](TruckDriversApi.md#update_truck_driver_async) | **PUT** /api/v2/LogisticsService/TruckDrivers/{driverId} | Update a truck driver |


## activate_truck_driver_async

> <EmptyEnvelope> activate_truck_driver_async(tenant_id, driver_id, opts)

Activate a truck driver

Activates a truck driver.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TruckDriversApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
driver_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Activate a truck driver
  result = api_instance.activate_truck_driver_async(tenant_id, driver_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TruckDriversApi->activate_truck_driver_async: #{e}"
end
```

#### Using the activate_truck_driver_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> activate_truck_driver_async_with_http_info(tenant_id, driver_id, opts)

```ruby
begin
  # Activate a truck driver
  data, status_code, headers = api_instance.activate_truck_driver_async_with_http_info(tenant_id, driver_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TruckDriversApi->activate_truck_driver_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **driver_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_truck_driver_async

> <EmptyEnvelope> create_truck_driver_async(tenant_id, opts)

Create a truck driver

Creates a new truck driver for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TruckDriversApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  truck_driver_create_dto: OpenapiClient::TruckDriverCreateDto.new # TruckDriverCreateDto | 
}

begin
  # Create a truck driver
  result = api_instance.create_truck_driver_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TruckDriversApi->create_truck_driver_async: #{e}"
end
```

#### Using the create_truck_driver_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_truck_driver_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a truck driver
  data, status_code, headers = api_instance.create_truck_driver_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TruckDriversApi->create_truck_driver_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **truck_driver_create_dto** | [**TruckDriverCreateDto**](TruckDriverCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## deactivate_truck_driver_async

> <EmptyEnvelope> deactivate_truck_driver_async(tenant_id, driver_id, opts)

Deactivate a truck driver

Deactivates a truck driver.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TruckDriversApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
driver_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deactivate a truck driver
  result = api_instance.deactivate_truck_driver_async(tenant_id, driver_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TruckDriversApi->deactivate_truck_driver_async: #{e}"
end
```

#### Using the deactivate_truck_driver_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> deactivate_truck_driver_async_with_http_info(tenant_id, driver_id, opts)

```ruby
begin
  # Deactivate a truck driver
  data, status_code, headers = api_instance.deactivate_truck_driver_async_with_http_info(tenant_id, driver_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TruckDriversApi->deactivate_truck_driver_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **driver_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_truck_driver_async

> <EmptyEnvelope> delete_truck_driver_async(tenant_id, driver_id, opts)

Delete a truck driver

Deletes a truck driver.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TruckDriversApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
driver_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a truck driver
  result = api_instance.delete_truck_driver_async(tenant_id, driver_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TruckDriversApi->delete_truck_driver_async: #{e}"
end
```

#### Using the delete_truck_driver_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_truck_driver_async_with_http_info(tenant_id, driver_id, opts)

```ruby
begin
  # Delete a truck driver
  data, status_code, headers = api_instance.delete_truck_driver_async_with_http_info(tenant_id, driver_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TruckDriversApi->delete_truck_driver_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **driver_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_truck_driver_by_id_async

> <TruckDriverDtoEnvelope> get_truck_driver_by_id_async(tenant_id, driver_id, opts)

Get truck driver by ID

Retrieves a specific truck driver by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TruckDriversApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
driver_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get truck driver by ID
  result = api_instance.get_truck_driver_by_id_async(tenant_id, driver_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TruckDriversApi->get_truck_driver_by_id_async: #{e}"
end
```

#### Using the get_truck_driver_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TruckDriverDtoEnvelope>, Integer, Hash)> get_truck_driver_by_id_async_with_http_info(tenant_id, driver_id, opts)

```ruby
begin
  # Get truck driver by ID
  data, status_code, headers = api_instance.get_truck_driver_by_id_async_with_http_info(tenant_id, driver_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TruckDriverDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TruckDriversApi->get_truck_driver_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **driver_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TruckDriverDtoEnvelope**](TruckDriverDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_truck_drivers_async

> <TruckDriverDtoListEnvelope> get_truck_drivers_async(tenant_id, opts)

Get all truck drivers

Retrieves all truck drivers for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TruckDriversApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all truck drivers
  result = api_instance.get_truck_drivers_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TruckDriversApi->get_truck_drivers_async: #{e}"
end
```

#### Using the get_truck_drivers_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TruckDriverDtoListEnvelope>, Integer, Hash)> get_truck_drivers_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all truck drivers
  data, status_code, headers = api_instance.get_truck_drivers_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TruckDriverDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TruckDriversApi->get_truck_drivers_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TruckDriverDtoListEnvelope**](TruckDriverDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_truck_drivers_count_async

> <Int32Envelope> get_truck_drivers_count_async(tenant_id, opts)

Get truck drivers count

Returns the count of truck drivers for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TruckDriversApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get truck drivers count
  result = api_instance.get_truck_drivers_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TruckDriversApi->get_truck_drivers_count_async: #{e}"
end
```

#### Using the get_truck_drivers_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_truck_drivers_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get truck drivers count
  data, status_code, headers = api_instance.get_truck_drivers_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TruckDriversApi->get_truck_drivers_count_async_with_http_info: #{e}"
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


## patch_truck_driver_async

> <EmptyEnvelope> patch_truck_driver_async(tenant_id, driver_id, opts)

Patch a truck driver

Partially updates an existing truck driver using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TruckDriversApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
driver_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a truck driver
  result = api_instance.patch_truck_driver_async(tenant_id, driver_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TruckDriversApi->patch_truck_driver_async: #{e}"
end
```

#### Using the patch_truck_driver_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_truck_driver_async_with_http_info(tenant_id, driver_id, opts)

```ruby
begin
  # Patch a truck driver
  data, status_code, headers = api_instance.patch_truck_driver_async_with_http_info(tenant_id, driver_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TruckDriversApi->patch_truck_driver_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **driver_id** | **String** |  |  |
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


## update_truck_driver_async

> <EmptyEnvelope> update_truck_driver_async(tenant_id, driver_id, opts)

Update a truck driver

Updates an existing truck driver.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TruckDriversApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
driver_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  truck_driver_update_dto: OpenapiClient::TruckDriverUpdateDto.new # TruckDriverUpdateDto | 
}

begin
  # Update a truck driver
  result = api_instance.update_truck_driver_async(tenant_id, driver_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TruckDriversApi->update_truck_driver_async: #{e}"
end
```

#### Using the update_truck_driver_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_truck_driver_async_with_http_info(tenant_id, driver_id, opts)

```ruby
begin
  # Update a truck driver
  data, status_code, headers = api_instance.update_truck_driver_async_with_http_info(tenant_id, driver_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TruckDriversApi->update_truck_driver_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **driver_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **truck_driver_update_dto** | [**TruckDriverUpdateDto**](TruckDriverUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

