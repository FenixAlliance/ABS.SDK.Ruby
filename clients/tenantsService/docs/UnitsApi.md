# OpenapiClient::UnitsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_tenant_unit**](UnitsApi.md#create_tenant_unit) | **POST** /api/v2/TenantsService/Units | Create a new tenant unit |
| [**delete_tenant_unit**](UnitsApi.md#delete_tenant_unit) | **DELETE** /api/v2/TenantsService/Units/{tenantUnitId} | Delete a tenant unit |
| [**get_tenant_unit_by_id**](UnitsApi.md#get_tenant_unit_by_id) | **GET** /api/v2/TenantsService/Units/{tenantUnitId} | Retrieve a single tenant unit by its ID |
| [**get_tenant_units**](UnitsApi.md#get_tenant_units) | **GET** /api/v2/TenantsService/Units | Retrieve a list of tenant units |
| [**get_tenant_units_count**](UnitsApi.md#get_tenant_units_count) | **GET** /api/v2/TenantsService/Units/Count | Get the count of tenant units |
| [**update_tenant_unit**](UnitsApi.md#update_tenant_unit) | **PUT** /api/v2/TenantsService/Units/{tenantUnitId} | Update a tenant unit |


## create_tenant_unit

> <EmptyEnvelope> create_tenant_unit(tenant_id, opts)

Create a new tenant unit

Create a new tenant unit

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_unit_create_dto: OpenapiClient::TenantUnitCreateDto.new # TenantUnitCreateDto | 
}

begin
  # Create a new tenant unit
  result = api_instance.create_tenant_unit(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitsApi->create_tenant_unit: #{e}"
end
```

#### Using the create_tenant_unit_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tenant_unit_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new tenant unit
  data, status_code, headers = api_instance.create_tenant_unit_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitsApi->create_tenant_unit_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_unit_create_dto** | [**TenantUnitCreateDto**](TenantUnitCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_tenant_unit

> <EmptyEnvelope> delete_tenant_unit(tenant_id, tenant_unit_id, opts)

Delete a tenant unit

Delete a tenant unit

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_unit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tenant unit
  result = api_instance.delete_tenant_unit(tenant_id, tenant_unit_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitsApi->delete_tenant_unit: #{e}"
end
```

#### Using the delete_tenant_unit_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tenant_unit_with_http_info(tenant_id, tenant_unit_id, opts)

```ruby
begin
  # Delete a tenant unit
  data, status_code, headers = api_instance.delete_tenant_unit_with_http_info(tenant_id, tenant_unit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitsApi->delete_tenant_unit_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_unit_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_unit_by_id

> <TenantUnitDtoEnvelope> get_tenant_unit_by_id(tenant_id, tenant_unit_id, opts)

Retrieve a single tenant unit by its ID

Retrieve a single tenant unit by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_unit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single tenant unit by its ID
  result = api_instance.get_tenant_unit_by_id(tenant_id, tenant_unit_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitsApi->get_tenant_unit_by_id: #{e}"
end
```

#### Using the get_tenant_unit_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantUnitDtoEnvelope>, Integer, Hash)> get_tenant_unit_by_id_with_http_info(tenant_id, tenant_unit_id, opts)

```ruby
begin
  # Retrieve a single tenant unit by its ID
  data, status_code, headers = api_instance.get_tenant_unit_by_id_with_http_info(tenant_id, tenant_unit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantUnitDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitsApi->get_tenant_unit_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_unit_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantUnitDtoEnvelope**](TenantUnitDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_units

> <TenantUnitDtoListEnvelope> get_tenant_units(tenant_id, opts)

Retrieve a list of tenant units

Retrieve a list of tenant units

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of tenant units
  result = api_instance.get_tenant_units(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitsApi->get_tenant_units: #{e}"
end
```

#### Using the get_tenant_units_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantUnitDtoListEnvelope>, Integer, Hash)> get_tenant_units_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of tenant units
  data, status_code, headers = api_instance.get_tenant_units_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantUnitDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitsApi->get_tenant_units_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantUnitDtoListEnvelope**](TenantUnitDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_units_count

> <Int32Envelope> get_tenant_units_count(tenant_id, opts)

Get the count of tenant units

Get the count of tenant units

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of tenant units
  result = api_instance.get_tenant_units_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitsApi->get_tenant_units_count: #{e}"
end
```

#### Using the get_tenant_units_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tenant_units_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of tenant units
  data, status_code, headers = api_instance.get_tenant_units_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitsApi->get_tenant_units_count_with_http_info: #{e}"
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


## update_tenant_unit

> <EmptyEnvelope> update_tenant_unit(tenant_id, tenant_unit_id, opts)

Update a tenant unit

Update a tenant unit

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_unit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_unit_update_dto: OpenapiClient::TenantUnitUpdateDto.new # TenantUnitUpdateDto | 
}

begin
  # Update a tenant unit
  result = api_instance.update_tenant_unit(tenant_id, tenant_unit_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitsApi->update_tenant_unit: #{e}"
end
```

#### Using the update_tenant_unit_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tenant_unit_with_http_info(tenant_id, tenant_unit_id, opts)

```ruby
begin
  # Update a tenant unit
  data, status_code, headers = api_instance.update_tenant_unit_with_http_info(tenant_id, tenant_unit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitsApi->update_tenant_unit_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_unit_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_unit_update_dto** | [**TenantUnitUpdateDto**](TenantUnitUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

