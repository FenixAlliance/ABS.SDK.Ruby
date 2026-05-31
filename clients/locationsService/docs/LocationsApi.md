# OpenapiClient::LocationsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_location_async**](LocationsApi.md#create_location_async) | **POST** /api/v2/LocationsService/Locations | Create Location |
| [**create_wallet_location_async**](LocationsApi.md#create_wallet_location_async) | **POST** /api/v2/LocationsService/Locations/wallet/{walletId} | Create Wallet Location |
| [**delete_location_async**](LocationsApi.md#delete_location_async) | **DELETE** /api/v2/LocationsService/Locations/{locationId} | Delete Location |
| [**delete_wallet_location_async**](LocationsApi.md#delete_wallet_location_async) | **DELETE** /api/v2/LocationsService/Locations/wallet/{walletId}/{locationId} | Delete Wallet Location |
| [**get_location_async**](LocationsApi.md#get_location_async) | **GET** /api/v2/LocationsService/Locations/{locationId} | Get Location |
| [**get_locations_async**](LocationsApi.md#get_locations_async) | **GET** /api/v2/LocationsService/Locations | Get Locations |
| [**get_locations_count_async**](LocationsApi.md#get_locations_count_async) | **GET** /api/v2/LocationsService/Locations/count | Get Locations Count |
| [**get_wallet_location_async**](LocationsApi.md#get_wallet_location_async) | **GET** /api/v2/LocationsService/Locations/wallet/{walletId}/{locationId} | Get Wallet Location |
| [**get_wallet_locations_async**](LocationsApi.md#get_wallet_locations_async) | **GET** /api/v2/LocationsService/Locations/wallet/{walletId} | Get Wallet Locations |
| [**get_wallet_locations_count_async**](LocationsApi.md#get_wallet_locations_count_async) | **GET** /api/v2/LocationsService/Locations/wallet/{walletId}/count | Get Wallet Locations Count |
| [**update_location_async**](LocationsApi.md#update_location_async) | **PUT** /api/v2/LocationsService/Locations/{locationId} | Update Location |
| [**update_wallet_location_async**](LocationsApi.md#update_wallet_location_async) | **PUT** /api/v2/LocationsService/Locations/wallet/{walletId}/{locationId} | Update Wallet Location |


## create_location_async

> <EmptyEnvelope> create_location_async(tenant_id, opts)

Create Location

Create a new location.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LocationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  location_create_dto: OpenapiClient::LocationCreateDto.new # LocationCreateDto | 
}

begin
  # Create Location
  result = api_instance.create_location_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->create_location_async: #{e}"
end
```

#### Using the create_location_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_location_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create Location
  data, status_code, headers = api_instance.create_location_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->create_location_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **location_create_dto** | [**LocationCreateDto**](LocationCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_wallet_location_async

> <EmptyEnvelope> create_wallet_location_async(wallet_id, opts)

Create Wallet Location

Create a new location for a specific wallet.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LocationsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  location_create_dto: OpenapiClient::LocationCreateDto.new # LocationCreateDto | 
}

begin
  # Create Wallet Location
  result = api_instance.create_wallet_location_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->create_wallet_location_async: #{e}"
end
```

#### Using the create_wallet_location_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_wallet_location_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Create Wallet Location
  data, status_code, headers = api_instance.create_wallet_location_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->create_wallet_location_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **location_create_dto** | [**LocationCreateDto**](LocationCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_location_async

> <EmptyEnvelope> delete_location_async(tenant_id, location_id)

Delete Location

Delete a specific location by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LocationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
location_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete Location
  result = api_instance.delete_location_async(tenant_id, location_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->delete_location_async: #{e}"
end
```

#### Using the delete_location_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_location_async_with_http_info(tenant_id, location_id)

```ruby
begin
  # Delete Location
  data, status_code, headers = api_instance.delete_location_async_with_http_info(tenant_id, location_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->delete_location_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **location_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_wallet_location_async

> <EmptyEnvelope> delete_wallet_location_async(wallet_id, location_id)

Delete Wallet Location

Delete a specific location of a wallet.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LocationsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
location_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete Wallet Location
  result = api_instance.delete_wallet_location_async(wallet_id, location_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->delete_wallet_location_async: #{e}"
end
```

#### Using the delete_wallet_location_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_wallet_location_async_with_http_info(wallet_id, location_id)

```ruby
begin
  # Delete Wallet Location
  data, status_code, headers = api_instance.delete_wallet_location_async_with_http_info(wallet_id, location_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->delete_wallet_location_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **location_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_location_async

> <LocationDtoEnvelope> get_location_async(tenant_id, location_id)

Get Location

Get details of a specific location by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LocationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
location_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get Location
  result = api_instance.get_location_async(tenant_id, location_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->get_location_async: #{e}"
end
```

#### Using the get_location_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LocationDtoEnvelope>, Integer, Hash)> get_location_async_with_http_info(tenant_id, location_id)

```ruby
begin
  # Get Location
  data, status_code, headers = api_instance.get_location_async_with_http_info(tenant_id, location_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LocationDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->get_location_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **location_id** | **String** |  |  |

### Return type

[**LocationDtoEnvelope**](LocationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_locations_async

> <LocationDtoIReadOnlyListEnvelope> get_locations_async(tenant_id)

Get Locations

Get all locations with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LocationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get Locations
  result = api_instance.get_locations_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->get_locations_async: #{e}"
end
```

#### Using the get_locations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LocationDtoIReadOnlyListEnvelope>, Integer, Hash)> get_locations_async_with_http_info(tenant_id)

```ruby
begin
  # Get Locations
  data, status_code, headers = api_instance.get_locations_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LocationDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->get_locations_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**LocationDtoIReadOnlyListEnvelope**](LocationDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_locations_count_async

> <Int32Envelope> get_locations_count_async(tenant_id)

Get Locations Count

Get the count of locations with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LocationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get Locations Count
  result = api_instance.get_locations_count_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->get_locations_count_async: #{e}"
end
```

#### Using the get_locations_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_locations_count_async_with_http_info(tenant_id)

```ruby
begin
  # Get Locations Count
  data, status_code, headers = api_instance.get_locations_count_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->get_locations_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_wallet_location_async

> <LocationDtoEnvelope> get_wallet_location_async(wallet_id, location_id)

Get Wallet Location

Get a specific location of a wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LocationsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
location_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get Wallet Location
  result = api_instance.get_wallet_location_async(wallet_id, location_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->get_wallet_location_async: #{e}"
end
```

#### Using the get_wallet_location_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LocationDtoEnvelope>, Integer, Hash)> get_wallet_location_async_with_http_info(wallet_id, location_id)

```ruby
begin
  # Get Wallet Location
  data, status_code, headers = api_instance.get_wallet_location_async_with_http_info(wallet_id, location_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LocationDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->get_wallet_location_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **location_id** | **String** |  |  |

### Return type

[**LocationDtoEnvelope**](LocationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_wallet_locations_async

> <LocationDtoIReadOnlyListEnvelope> get_wallet_locations_async(wallet_id)

Get Wallet Locations

Get locations for a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LocationsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get Wallet Locations
  result = api_instance.get_wallet_locations_async(wallet_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->get_wallet_locations_async: #{e}"
end
```

#### Using the get_wallet_locations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LocationDtoIReadOnlyListEnvelope>, Integer, Hash)> get_wallet_locations_async_with_http_info(wallet_id)

```ruby
begin
  # Get Wallet Locations
  data, status_code, headers = api_instance.get_wallet_locations_async_with_http_info(wallet_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LocationDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->get_wallet_locations_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |

### Return type

[**LocationDtoIReadOnlyListEnvelope**](LocationDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_wallet_locations_count_async

> <Int32Envelope> get_wallet_locations_count_async(wallet_id)

Get Wallet Locations Count

Get the count of locations for a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LocationsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get Wallet Locations Count
  result = api_instance.get_wallet_locations_count_async(wallet_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->get_wallet_locations_count_async: #{e}"
end
```

#### Using the get_wallet_locations_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_wallet_locations_count_async_with_http_info(wallet_id)

```ruby
begin
  # Get Wallet Locations Count
  data, status_code, headers = api_instance.get_wallet_locations_count_async_with_http_info(wallet_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->get_wallet_locations_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_location_async

> <EmptyEnvelope> update_location_async(tenant_id, location_id, opts)

Update Location

Update a specific location by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LocationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
location_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  location_update_dto: OpenapiClient::LocationUpdateDto.new # LocationUpdateDto | 
}

begin
  # Update Location
  result = api_instance.update_location_async(tenant_id, location_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->update_location_async: #{e}"
end
```

#### Using the update_location_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_location_async_with_http_info(tenant_id, location_id, opts)

```ruby
begin
  # Update Location
  data, status_code, headers = api_instance.update_location_async_with_http_info(tenant_id, location_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->update_location_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **location_id** | **String** |  |  |
| **location_update_dto** | [**LocationUpdateDto**](LocationUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_wallet_location_async

> <EmptyEnvelope> update_wallet_location_async(wallet_id, location_id, opts)

Update Wallet Location

Update a specific location of a wallet.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LocationsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
location_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  location_update_dto: OpenapiClient::LocationUpdateDto.new # LocationUpdateDto | 
}

begin
  # Update Wallet Location
  result = api_instance.update_wallet_location_async(wallet_id, location_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->update_wallet_location_async: #{e}"
end
```

#### Using the update_wallet_location_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_wallet_location_async_with_http_info(wallet_id, location_id, opts)

```ruby
begin
  # Update Wallet Location
  data, status_code, headers = api_instance.update_wallet_location_async_with_http_info(wallet_id, location_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocationsApi->update_wallet_location_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **location_id** | **String** |  |  |
| **location_update_dto** | [**LocationUpdateDto**](LocationUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

