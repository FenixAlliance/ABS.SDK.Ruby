# OpenapiClient::TerritoriesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_tenant_territory**](TerritoriesApi.md#create_tenant_territory) | **POST** /api/v2/TenantsService/Territories | Create a new tenant territory |
| [**delete_tenant_territory**](TerritoriesApi.md#delete_tenant_territory) | **DELETE** /api/v2/TenantsService/Territories/{tenantTerritoryId} | Delete a tenant territory |
| [**get_tenant_territories**](TerritoriesApi.md#get_tenant_territories) | **GET** /api/v2/TenantsService/Territories | Retrieve a list of tenant territories |
| [**get_tenant_territories_count**](TerritoriesApi.md#get_tenant_territories_count) | **GET** /api/v2/TenantsService/Territories/Count | Get the count of tenant territories |
| [**get_tenant_territory_by_id**](TerritoriesApi.md#get_tenant_territory_by_id) | **GET** /api/v2/TenantsService/Territories/{tenantTerritoryId} | Retrieve a single tenant territory by its ID |
| [**patch_tenant_territory**](TerritoriesApi.md#patch_tenant_territory) | **PATCH** /api/v2/TenantsService/Territories/{tenantTerritoryId} | Patch a tenant territory |
| [**update_tenant_territory**](TerritoriesApi.md#update_tenant_territory) | **PUT** /api/v2/TenantsService/Territories/{tenantTerritoryId} | Update a tenant territory |


## create_tenant_territory

> <EmptyEnvelope> create_tenant_territory(tenant_id, opts)

Create a new tenant territory

Create a new tenant territory

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TerritoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_territory_create_dto: OpenapiClient::TenantTerritoryCreateDto.new # TenantTerritoryCreateDto | 
}

begin
  # Create a new tenant territory
  result = api_instance.create_tenant_territory(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TerritoriesApi->create_tenant_territory: #{e}"
end
```

#### Using the create_tenant_territory_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tenant_territory_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new tenant territory
  data, status_code, headers = api_instance.create_tenant_territory_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TerritoriesApi->create_tenant_territory_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_territory_create_dto** | [**TenantTerritoryCreateDto**](TenantTerritoryCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_tenant_territory

> <EmptyEnvelope> delete_tenant_territory(tenant_id, tenant_territory_id, opts)

Delete a tenant territory

Delete a tenant territory

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TerritoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_territory_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tenant territory
  result = api_instance.delete_tenant_territory(tenant_id, tenant_territory_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TerritoriesApi->delete_tenant_territory: #{e}"
end
```

#### Using the delete_tenant_territory_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tenant_territory_with_http_info(tenant_id, tenant_territory_id, opts)

```ruby
begin
  # Delete a tenant territory
  data, status_code, headers = api_instance.delete_tenant_territory_with_http_info(tenant_id, tenant_territory_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TerritoriesApi->delete_tenant_territory_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_territory_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_territories

> <TenantTerritoryDtoListEnvelope> get_tenant_territories(tenant_id, opts)

Retrieve a list of tenant territories

Retrieve a list of tenant territories

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TerritoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of tenant territories
  result = api_instance.get_tenant_territories(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TerritoriesApi->get_tenant_territories: #{e}"
end
```

#### Using the get_tenant_territories_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantTerritoryDtoListEnvelope>, Integer, Hash)> get_tenant_territories_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of tenant territories
  data, status_code, headers = api_instance.get_tenant_territories_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantTerritoryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TerritoriesApi->get_tenant_territories_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantTerritoryDtoListEnvelope**](TenantTerritoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_territories_count

> <Int32Envelope> get_tenant_territories_count(tenant_id, opts)

Get the count of tenant territories

Get the count of tenant territories

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TerritoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of tenant territories
  result = api_instance.get_tenant_territories_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TerritoriesApi->get_tenant_territories_count: #{e}"
end
```

#### Using the get_tenant_territories_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tenant_territories_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of tenant territories
  data, status_code, headers = api_instance.get_tenant_territories_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TerritoriesApi->get_tenant_territories_count_with_http_info: #{e}"
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


## get_tenant_territory_by_id

> <TenantTerritoryDtoEnvelope> get_tenant_territory_by_id(tenant_id, tenant_territory_id, opts)

Retrieve a single tenant territory by its ID

Retrieve a single tenant territory by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TerritoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_territory_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single tenant territory by its ID
  result = api_instance.get_tenant_territory_by_id(tenant_id, tenant_territory_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TerritoriesApi->get_tenant_territory_by_id: #{e}"
end
```

#### Using the get_tenant_territory_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantTerritoryDtoEnvelope>, Integer, Hash)> get_tenant_territory_by_id_with_http_info(tenant_id, tenant_territory_id, opts)

```ruby
begin
  # Retrieve a single tenant territory by its ID
  data, status_code, headers = api_instance.get_tenant_territory_by_id_with_http_info(tenant_id, tenant_territory_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantTerritoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TerritoriesApi->get_tenant_territory_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_territory_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantTerritoryDtoEnvelope**](TenantTerritoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_tenant_territory

> <EmptyEnvelope> patch_tenant_territory(tenant_id, tenant_territory_id, opts)

Patch a tenant territory

Patch a tenant territory

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TerritoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_territory_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a tenant territory
  result = api_instance.patch_tenant_territory(tenant_id, tenant_territory_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TerritoriesApi->patch_tenant_territory: #{e}"
end
```

#### Using the patch_tenant_territory_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_tenant_territory_with_http_info(tenant_id, tenant_territory_id, opts)

```ruby
begin
  # Patch a tenant territory
  data, status_code, headers = api_instance.patch_tenant_territory_with_http_info(tenant_id, tenant_territory_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TerritoriesApi->patch_tenant_territory_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_territory_id** | **String** |  |  |
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


## update_tenant_territory

> <EmptyEnvelope> update_tenant_territory(tenant_id, tenant_territory_id, opts)

Update a tenant territory

Update a tenant territory

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TerritoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_territory_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_territory_update_dto: OpenapiClient::TenantTerritoryUpdateDto.new # TenantTerritoryUpdateDto | 
}

begin
  # Update a tenant territory
  result = api_instance.update_tenant_territory(tenant_id, tenant_territory_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TerritoriesApi->update_tenant_territory: #{e}"
end
```

#### Using the update_tenant_territory_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tenant_territory_with_http_info(tenant_id, tenant_territory_id, opts)

```ruby
begin
  # Update a tenant territory
  data, status_code, headers = api_instance.update_tenant_territory_with_http_info(tenant_id, tenant_territory_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TerritoriesApi->update_tenant_territory_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_territory_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_territory_update_dto** | [**TenantTerritoryUpdateDto**](TenantTerritoryUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

