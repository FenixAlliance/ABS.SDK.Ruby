# OpenapiClient::PositionsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_tenant_position**](PositionsApi.md#create_tenant_position) | **POST** /api/v2/TenantsService/Positions | Create a new tenant position |
| [**delete_tenant_position**](PositionsApi.md#delete_tenant_position) | **DELETE** /api/v2/TenantsService/Positions/{tenantPositionId} | Delete a tenant position |
| [**get_tenant_position_by_id**](PositionsApi.md#get_tenant_position_by_id) | **GET** /api/v2/TenantsService/Positions/{tenantPositionId} | Retrieve a single tenant position by its ID |
| [**get_tenant_positions**](PositionsApi.md#get_tenant_positions) | **GET** /api/v2/TenantsService/Positions | Retrieve a list of tenant positions |
| [**get_tenant_positions_count**](PositionsApi.md#get_tenant_positions_count) | **GET** /api/v2/TenantsService/Positions/Count | Get the count of tenant positions |
| [**update_tenant_position**](PositionsApi.md#update_tenant_position) | **PUT** /api/v2/TenantsService/Positions/{tenantPositionId} | Update a tenant position |


## create_tenant_position

> <EmptyEnvelope> create_tenant_position(tenant_id, opts)

Create a new tenant position

Create a new tenant position

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PositionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_position_create_dto: OpenapiClient::TenantPositionCreateDto.new # TenantPositionCreateDto | 
}

begin
  # Create a new tenant position
  result = api_instance.create_tenant_position(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PositionsApi->create_tenant_position: #{e}"
end
```

#### Using the create_tenant_position_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tenant_position_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new tenant position
  data, status_code, headers = api_instance.create_tenant_position_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PositionsApi->create_tenant_position_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_position_create_dto** | [**TenantPositionCreateDto**](TenantPositionCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_tenant_position

> <EmptyEnvelope> delete_tenant_position(tenant_id, tenant_position_id, opts)

Delete a tenant position

Delete a tenant position

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PositionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_position_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tenant position
  result = api_instance.delete_tenant_position(tenant_id, tenant_position_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PositionsApi->delete_tenant_position: #{e}"
end
```

#### Using the delete_tenant_position_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tenant_position_with_http_info(tenant_id, tenant_position_id, opts)

```ruby
begin
  # Delete a tenant position
  data, status_code, headers = api_instance.delete_tenant_position_with_http_info(tenant_id, tenant_position_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PositionsApi->delete_tenant_position_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_position_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_position_by_id

> <TenantPositionDtoEnvelope> get_tenant_position_by_id(tenant_id, tenant_position_id, opts)

Retrieve a single tenant position by its ID

Retrieve a single tenant position by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PositionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_position_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single tenant position by its ID
  result = api_instance.get_tenant_position_by_id(tenant_id, tenant_position_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PositionsApi->get_tenant_position_by_id: #{e}"
end
```

#### Using the get_tenant_position_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantPositionDtoEnvelope>, Integer, Hash)> get_tenant_position_by_id_with_http_info(tenant_id, tenant_position_id, opts)

```ruby
begin
  # Retrieve a single tenant position by its ID
  data, status_code, headers = api_instance.get_tenant_position_by_id_with_http_info(tenant_id, tenant_position_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantPositionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PositionsApi->get_tenant_position_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_position_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantPositionDtoEnvelope**](TenantPositionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_positions

> <TenantPositionDtoListEnvelope> get_tenant_positions(tenant_id, opts)

Retrieve a list of tenant positions

Retrieve a list of tenant positions

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PositionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of tenant positions
  result = api_instance.get_tenant_positions(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PositionsApi->get_tenant_positions: #{e}"
end
```

#### Using the get_tenant_positions_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantPositionDtoListEnvelope>, Integer, Hash)> get_tenant_positions_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of tenant positions
  data, status_code, headers = api_instance.get_tenant_positions_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantPositionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PositionsApi->get_tenant_positions_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantPositionDtoListEnvelope**](TenantPositionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_positions_count

> <Int32Envelope> get_tenant_positions_count(tenant_id, opts)

Get the count of tenant positions

Get the count of tenant positions

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PositionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of tenant positions
  result = api_instance.get_tenant_positions_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PositionsApi->get_tenant_positions_count: #{e}"
end
```

#### Using the get_tenant_positions_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tenant_positions_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of tenant positions
  data, status_code, headers = api_instance.get_tenant_positions_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PositionsApi->get_tenant_positions_count_with_http_info: #{e}"
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


## update_tenant_position

> <EmptyEnvelope> update_tenant_position(tenant_id, tenant_position_id, opts)

Update a tenant position

Update a tenant position

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PositionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_position_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_position_update_dto: OpenapiClient::TenantPositionUpdateDto.new # TenantPositionUpdateDto | 
}

begin
  # Update a tenant position
  result = api_instance.update_tenant_position(tenant_id, tenant_position_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PositionsApi->update_tenant_position: #{e}"
end
```

#### Using the update_tenant_position_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tenant_position_with_http_info(tenant_id, tenant_position_id, opts)

```ruby
begin
  # Update a tenant position
  data, status_code, headers = api_instance.update_tenant_position_with_http_info(tenant_id, tenant_position_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PositionsApi->update_tenant_position_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_position_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_position_update_dto** | [**TenantPositionUpdateDto**](TenantPositionUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

