# OpenapiClient::TeamsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_tenant_team**](TeamsApi.md#create_tenant_team) | **POST** /api/v2/TenantsService/Teams | Create a new tenant team |
| [**delete_tenant_team**](TeamsApi.md#delete_tenant_team) | **DELETE** /api/v2/TenantsService/Teams/{tenantTeamId} | Delete a tenant team |
| [**get_tenant_team_by_id**](TeamsApi.md#get_tenant_team_by_id) | **GET** /api/v2/TenantsService/Teams/{tenantTeamId} | Retrieve a single tenant team by its ID |
| [**get_tenant_teams**](TeamsApi.md#get_tenant_teams) | **GET** /api/v2/TenantsService/Teams | Retrieve a list of tenant teams |
| [**get_tenant_teams_count**](TeamsApi.md#get_tenant_teams_count) | **GET** /api/v2/TenantsService/Teams/Count | Get the count of tenant teams |
| [**update_tenant_team**](TeamsApi.md#update_tenant_team) | **PUT** /api/v2/TenantsService/Teams/{tenantTeamId} | Update a tenant team |


## create_tenant_team

> <EmptyEnvelope> create_tenant_team(tenant_id, opts)

Create a new tenant team

Create a new tenant team

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_team_create_dto: OpenapiClient::TenantTeamCreateDto.new({business_id: 'business_id_example'}) # TenantTeamCreateDto | 
}

begin
  # Create a new tenant team
  result = api_instance.create_tenant_team(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->create_tenant_team: #{e}"
end
```

#### Using the create_tenant_team_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tenant_team_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new tenant team
  data, status_code, headers = api_instance.create_tenant_team_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->create_tenant_team_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_team_create_dto** | [**TenantTeamCreateDto**](TenantTeamCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_tenant_team

> <EmptyEnvelope> delete_tenant_team(tenant_id, tenant_team_id, opts)

Delete a tenant team

Delete a tenant team

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_team_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tenant team
  result = api_instance.delete_tenant_team(tenant_id, tenant_team_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->delete_tenant_team: #{e}"
end
```

#### Using the delete_tenant_team_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tenant_team_with_http_info(tenant_id, tenant_team_id, opts)

```ruby
begin
  # Delete a tenant team
  data, status_code, headers = api_instance.delete_tenant_team_with_http_info(tenant_id, tenant_team_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->delete_tenant_team_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_team_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_team_by_id

> <TenantTeamDtoEnvelope> get_tenant_team_by_id(tenant_id, tenant_team_id, opts)

Retrieve a single tenant team by its ID

Retrieve a single tenant team by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_team_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single tenant team by its ID
  result = api_instance.get_tenant_team_by_id(tenant_id, tenant_team_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->get_tenant_team_by_id: #{e}"
end
```

#### Using the get_tenant_team_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantTeamDtoEnvelope>, Integer, Hash)> get_tenant_team_by_id_with_http_info(tenant_id, tenant_team_id, opts)

```ruby
begin
  # Retrieve a single tenant team by its ID
  data, status_code, headers = api_instance.get_tenant_team_by_id_with_http_info(tenant_id, tenant_team_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantTeamDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->get_tenant_team_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_team_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantTeamDtoEnvelope**](TenantTeamDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_teams

> <TenantTeamDtoListEnvelope> get_tenant_teams(tenant_id, opts)

Retrieve a list of tenant teams

Retrieve a list of tenant teams

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of tenant teams
  result = api_instance.get_tenant_teams(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->get_tenant_teams: #{e}"
end
```

#### Using the get_tenant_teams_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantTeamDtoListEnvelope>, Integer, Hash)> get_tenant_teams_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of tenant teams
  data, status_code, headers = api_instance.get_tenant_teams_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantTeamDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->get_tenant_teams_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantTeamDtoListEnvelope**](TenantTeamDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_teams_count

> <Int32Envelope> get_tenant_teams_count(tenant_id, opts)

Get the count of tenant teams

Get the count of tenant teams

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of tenant teams
  result = api_instance.get_tenant_teams_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->get_tenant_teams_count: #{e}"
end
```

#### Using the get_tenant_teams_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tenant_teams_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of tenant teams
  data, status_code, headers = api_instance.get_tenant_teams_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->get_tenant_teams_count_with_http_info: #{e}"
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


## update_tenant_team

> <EmptyEnvelope> update_tenant_team(tenant_id, tenant_team_id, opts)

Update a tenant team

Update a tenant team

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_team_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_team_update_dto: OpenapiClient::TenantTeamUpdateDto.new # TenantTeamUpdateDto | 
}

begin
  # Update a tenant team
  result = api_instance.update_tenant_team(tenant_id, tenant_team_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->update_tenant_team: #{e}"
end
```

#### Using the update_tenant_team_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tenant_team_with_http_info(tenant_id, tenant_team_id, opts)

```ruby
begin
  # Update a tenant team
  data, status_code, headers = api_instance.update_tenant_team_with_http_info(tenant_id, tenant_team_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->update_tenant_team_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_team_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_team_update_dto** | [**TenantTeamUpdateDto**](TenantTeamUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

