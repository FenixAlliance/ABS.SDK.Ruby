# OpenapiClient::TrucksApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**arrive_trip_async**](TrucksApi.md#arrive_trip_async) | **POST** /api/v2/LogisticsService/Trucks/{truckId}/Trips/{tripId}/Arrive | Arrive a trip |
| [**cancel_trip_async**](TrucksApi.md#cancel_trip_async) | **POST** /api/v2/LogisticsService/Trucks/{truckId}/Trips/{tripId}/Cancel | Cancel a trip |
| [**create_truck_async**](TrucksApi.md#create_truck_async) | **POST** /api/v2/LogisticsService/Trucks | Create a truck |
| [**create_truck_trip_async**](TrucksApi.md#create_truck_trip_async) | **POST** /api/v2/LogisticsService/Trucks/{truckId}/Trips | Create a truck trip |
| [**delete_truck_async**](TrucksApi.md#delete_truck_async) | **DELETE** /api/v2/LogisticsService/Trucks/{truckId} | Delete a truck |
| [**delete_truck_trip_async**](TrucksApi.md#delete_truck_trip_async) | **DELETE** /api/v2/LogisticsService/Trucks/{truckId}/Trips/{tripId} | Delete a truck trip |
| [**deliver_trip_async**](TrucksApi.md#deliver_trip_async) | **POST** /api/v2/LogisticsService/Trucks/{truckId}/Trips/{tripId}/Deliver | Deliver a trip |
| [**depart_trip_async**](TrucksApi.md#depart_trip_async) | **POST** /api/v2/LogisticsService/Trucks/{truckId}/Trips/{tripId}/Depart | Depart a trip |
| [**dispatch_trip_async**](TrucksApi.md#dispatch_trip_async) | **POST** /api/v2/LogisticsService/Trucks/{truckId}/Trips/{tripId}/Dispatch | Dispatch a trip |
| [**get_truck_by_id_async**](TrucksApi.md#get_truck_by_id_async) | **GET** /api/v2/LogisticsService/Trucks/{truckId} | Get truck by ID |
| [**get_truck_trips_async**](TrucksApi.md#get_truck_trips_async) | **GET** /api/v2/LogisticsService/Trucks/{truckId}/Trips | Get truck trips |
| [**get_truck_trips_count_async**](TrucksApi.md#get_truck_trips_count_async) | **GET** /api/v2/LogisticsService/Trucks/{truckId}/Trips/Count | Get truck trips count |
| [**get_trucks_async**](TrucksApi.md#get_trucks_async) | **GET** /api/v2/LogisticsService/Trucks | Get all trucks |
| [**get_trucks_count_async**](TrucksApi.md#get_trucks_count_async) | **GET** /api/v2/LogisticsService/Trucks/Count | Get trucks count |
| [**update_truck_async**](TrucksApi.md#update_truck_async) | **PUT** /api/v2/LogisticsService/Trucks/{truckId} | Update a truck |
| [**update_truck_trip_async**](TrucksApi.md#update_truck_trip_async) | **PUT** /api/v2/LogisticsService/Trucks/{truckId}/Trips/{tripId} | Update a truck trip |


## arrive_trip_async

> <EmptyEnvelope> arrive_trip_async(tenant_id, truck_id, trip_id, opts)

Arrive a trip

Marks a truck trip as arrived.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrucksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
truck_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
trip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Arrive a trip
  result = api_instance.arrive_trip_async(tenant_id, truck_id, trip_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->arrive_trip_async: #{e}"
end
```

#### Using the arrive_trip_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> arrive_trip_async_with_http_info(tenant_id, truck_id, trip_id, opts)

```ruby
begin
  # Arrive a trip
  data, status_code, headers = api_instance.arrive_trip_async_with_http_info(tenant_id, truck_id, trip_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->arrive_trip_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **truck_id** | **String** |  |  |
| **trip_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## cancel_trip_async

> <EmptyEnvelope> cancel_trip_async(tenant_id, truck_id, trip_id, opts)

Cancel a trip

Cancels a truck trip.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrucksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
truck_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
trip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Cancel a trip
  result = api_instance.cancel_trip_async(tenant_id, truck_id, trip_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->cancel_trip_async: #{e}"
end
```

#### Using the cancel_trip_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> cancel_trip_async_with_http_info(tenant_id, truck_id, trip_id, opts)

```ruby
begin
  # Cancel a trip
  data, status_code, headers = api_instance.cancel_trip_async_with_http_info(tenant_id, truck_id, trip_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->cancel_trip_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **truck_id** | **String** |  |  |
| **trip_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_truck_async

> <EmptyEnvelope> create_truck_async(tenant_id, opts)

Create a truck

Creates a new truck for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrucksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  truck_create_dto: OpenapiClient::TruckCreateDto.new # TruckCreateDto | 
}

begin
  # Create a truck
  result = api_instance.create_truck_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->create_truck_async: #{e}"
end
```

#### Using the create_truck_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_truck_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a truck
  data, status_code, headers = api_instance.create_truck_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->create_truck_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **truck_create_dto** | [**TruckCreateDto**](TruckCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_truck_trip_async

> <EmptyEnvelope> create_truck_trip_async(tenant_id, truck_id, opts)

Create a truck trip

Creates a new trip for a truck.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrucksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
truck_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  truck_trip_create_dto: OpenapiClient::TruckTripCreateDto.new # TruckTripCreateDto | 
}

begin
  # Create a truck trip
  result = api_instance.create_truck_trip_async(tenant_id, truck_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->create_truck_trip_async: #{e}"
end
```

#### Using the create_truck_trip_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_truck_trip_async_with_http_info(tenant_id, truck_id, opts)

```ruby
begin
  # Create a truck trip
  data, status_code, headers = api_instance.create_truck_trip_async_with_http_info(tenant_id, truck_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->create_truck_trip_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **truck_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **truck_trip_create_dto** | [**TruckTripCreateDto**](TruckTripCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_truck_async

> <EmptyEnvelope> delete_truck_async(tenant_id, truck_id, opts)

Delete a truck

Deletes a truck.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrucksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
truck_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a truck
  result = api_instance.delete_truck_async(tenant_id, truck_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->delete_truck_async: #{e}"
end
```

#### Using the delete_truck_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_truck_async_with_http_info(tenant_id, truck_id, opts)

```ruby
begin
  # Delete a truck
  data, status_code, headers = api_instance.delete_truck_async_with_http_info(tenant_id, truck_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->delete_truck_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **truck_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_truck_trip_async

> <EmptyEnvelope> delete_truck_trip_async(tenant_id, truck_id, trip_id, opts)

Delete a truck trip

Deletes a truck trip.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrucksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
truck_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
trip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a truck trip
  result = api_instance.delete_truck_trip_async(tenant_id, truck_id, trip_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->delete_truck_trip_async: #{e}"
end
```

#### Using the delete_truck_trip_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_truck_trip_async_with_http_info(tenant_id, truck_id, trip_id, opts)

```ruby
begin
  # Delete a truck trip
  data, status_code, headers = api_instance.delete_truck_trip_async_with_http_info(tenant_id, truck_id, trip_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->delete_truck_trip_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **truck_id** | **String** |  |  |
| **trip_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## deliver_trip_async

> <EmptyEnvelope> deliver_trip_async(tenant_id, truck_id, trip_id, opts)

Deliver a trip

Marks a truck trip as delivered.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrucksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
truck_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
trip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deliver a trip
  result = api_instance.deliver_trip_async(tenant_id, truck_id, trip_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->deliver_trip_async: #{e}"
end
```

#### Using the deliver_trip_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> deliver_trip_async_with_http_info(tenant_id, truck_id, trip_id, opts)

```ruby
begin
  # Deliver a trip
  data, status_code, headers = api_instance.deliver_trip_async_with_http_info(tenant_id, truck_id, trip_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->deliver_trip_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **truck_id** | **String** |  |  |
| **trip_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## depart_trip_async

> <EmptyEnvelope> depart_trip_async(tenant_id, truck_id, trip_id, opts)

Depart a trip

Marks a truck trip as departed.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrucksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
truck_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
trip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Depart a trip
  result = api_instance.depart_trip_async(tenant_id, truck_id, trip_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->depart_trip_async: #{e}"
end
```

#### Using the depart_trip_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> depart_trip_async_with_http_info(tenant_id, truck_id, trip_id, opts)

```ruby
begin
  # Depart a trip
  data, status_code, headers = api_instance.depart_trip_async_with_http_info(tenant_id, truck_id, trip_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->depart_trip_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **truck_id** | **String** |  |  |
| **trip_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## dispatch_trip_async

> <EmptyEnvelope> dispatch_trip_async(tenant_id, truck_id, trip_id, opts)

Dispatch a trip

Dispatches a truck trip.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrucksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
truck_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
trip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Dispatch a trip
  result = api_instance.dispatch_trip_async(tenant_id, truck_id, trip_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->dispatch_trip_async: #{e}"
end
```

#### Using the dispatch_trip_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> dispatch_trip_async_with_http_info(tenant_id, truck_id, trip_id, opts)

```ruby
begin
  # Dispatch a trip
  data, status_code, headers = api_instance.dispatch_trip_async_with_http_info(tenant_id, truck_id, trip_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->dispatch_trip_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **truck_id** | **String** |  |  |
| **trip_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_truck_by_id_async

> <TruckDtoEnvelope> get_truck_by_id_async(tenant_id, truck_id, opts)

Get truck by ID

Retrieves a specific truck by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrucksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
truck_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get truck by ID
  result = api_instance.get_truck_by_id_async(tenant_id, truck_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->get_truck_by_id_async: #{e}"
end
```

#### Using the get_truck_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TruckDtoEnvelope>, Integer, Hash)> get_truck_by_id_async_with_http_info(tenant_id, truck_id, opts)

```ruby
begin
  # Get truck by ID
  data, status_code, headers = api_instance.get_truck_by_id_async_with_http_info(tenant_id, truck_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TruckDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->get_truck_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **truck_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TruckDtoEnvelope**](TruckDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_truck_trips_async

> <TruckTripDtoListEnvelope> get_truck_trips_async(tenant_id, truck_id, opts)

Get truck trips

Retrieves all trips for a specific truck.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrucksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
truck_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get truck trips
  result = api_instance.get_truck_trips_async(tenant_id, truck_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->get_truck_trips_async: #{e}"
end
```

#### Using the get_truck_trips_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TruckTripDtoListEnvelope>, Integer, Hash)> get_truck_trips_async_with_http_info(tenant_id, truck_id, opts)

```ruby
begin
  # Get truck trips
  data, status_code, headers = api_instance.get_truck_trips_async_with_http_info(tenant_id, truck_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TruckTripDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->get_truck_trips_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **truck_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TruckTripDtoListEnvelope**](TruckTripDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_truck_trips_count_async

> <Int32Envelope> get_truck_trips_count_async(tenant_id, truck_id, opts)

Get truck trips count

Returns the count of trips for a specific truck.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrucksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
truck_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get truck trips count
  result = api_instance.get_truck_trips_count_async(tenant_id, truck_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->get_truck_trips_count_async: #{e}"
end
```

#### Using the get_truck_trips_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_truck_trips_count_async_with_http_info(tenant_id, truck_id, opts)

```ruby
begin
  # Get truck trips count
  data, status_code, headers = api_instance.get_truck_trips_count_async_with_http_info(tenant_id, truck_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->get_truck_trips_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **truck_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_trucks_async

> <TruckDtoListEnvelope> get_trucks_async(tenant_id, opts)

Get all trucks

Retrieves all trucks for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrucksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all trucks
  result = api_instance.get_trucks_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->get_trucks_async: #{e}"
end
```

#### Using the get_trucks_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TruckDtoListEnvelope>, Integer, Hash)> get_trucks_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all trucks
  data, status_code, headers = api_instance.get_trucks_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TruckDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->get_trucks_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TruckDtoListEnvelope**](TruckDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_trucks_count_async

> <Int32Envelope> get_trucks_count_async(tenant_id, opts)

Get trucks count

Returns the count of trucks for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrucksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get trucks count
  result = api_instance.get_trucks_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->get_trucks_count_async: #{e}"
end
```

#### Using the get_trucks_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_trucks_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get trucks count
  data, status_code, headers = api_instance.get_trucks_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->get_trucks_count_async_with_http_info: #{e}"
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


## update_truck_async

> <EmptyEnvelope> update_truck_async(tenant_id, truck_id, opts)

Update a truck

Updates an existing truck.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrucksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
truck_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  truck_update_dto: OpenapiClient::TruckUpdateDto.new # TruckUpdateDto | 
}

begin
  # Update a truck
  result = api_instance.update_truck_async(tenant_id, truck_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->update_truck_async: #{e}"
end
```

#### Using the update_truck_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_truck_async_with_http_info(tenant_id, truck_id, opts)

```ruby
begin
  # Update a truck
  data, status_code, headers = api_instance.update_truck_async_with_http_info(tenant_id, truck_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->update_truck_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **truck_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **truck_update_dto** | [**TruckUpdateDto**](TruckUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_truck_trip_async

> <EmptyEnvelope> update_truck_trip_async(tenant_id, truck_id, trip_id, opts)

Update a truck trip

Updates an existing truck trip.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrucksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
truck_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
trip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  truck_trip_update_dto: OpenapiClient::TruckTripUpdateDto.new # TruckTripUpdateDto | 
}

begin
  # Update a truck trip
  result = api_instance.update_truck_trip_async(tenant_id, truck_id, trip_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->update_truck_trip_async: #{e}"
end
```

#### Using the update_truck_trip_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_truck_trip_async_with_http_info(tenant_id, truck_id, trip_id, opts)

```ruby
begin
  # Update a truck trip
  data, status_code, headers = api_instance.update_truck_trip_async_with_http_info(tenant_id, truck_id, trip_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrucksApi->update_truck_trip_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **truck_id** | **String** |  |  |
| **trip_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **truck_trip_update_dto** | [**TruckTripUpdateDto**](TruckTripUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

