# OpenapiClient::UnitGroupsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_unit_async**](UnitGroupsApi.md#create_unit_async) | **POST** /api/v2/TenantsService/UnitGroups/{unitGroupId}/Units | Create a unit within a unit group |
| [**create_unit_group_async**](UnitGroupsApi.md#create_unit_group_async) | **POST** /api/v2/TenantsService/UnitGroups | Create a new unit group |
| [**delete_unit_async**](UnitGroupsApi.md#delete_unit_async) | **DELETE** /api/v2/TenantsService/UnitGroups/{unitGroupId}/Units/{unitId} | Delete a unit from a unit group |
| [**delete_unit_group_async**](UnitGroupsApi.md#delete_unit_group_async) | **DELETE** /api/v2/TenantsService/UnitGroups/{unitGroupId} | Delete a unit group |
| [**get_unit_async**](UnitGroupsApi.md#get_unit_async) | **GET** /api/v2/TenantsService/UnitGroups/{unitGroupId}/Units/{unitId} | Retrieve a unit by ID within a unit group |
| [**get_unit_group_async**](UnitGroupsApi.md#get_unit_group_async) | **GET** /api/v2/TenantsService/UnitGroups/{unitGroupId} | Retrieve a unit group by ID |
| [**get_unit_groups_async**](UnitGroupsApi.md#get_unit_groups_async) | **GET** /api/v2/TenantsService/UnitGroups | Retrieve a list of unit groups |
| [**get_unit_groups_count_async**](UnitGroupsApi.md#get_unit_groups_count_async) | **GET** /api/v2/TenantsService/UnitGroups/Count | Get the count of unit groups |
| [**get_units_async**](UnitGroupsApi.md#get_units_async) | **GET** /api/v2/TenantsService/UnitGroups/{unitGroupId}/Units | Retrieve units for a unit group |
| [**get_units_count_async**](UnitGroupsApi.md#get_units_count_async) | **GET** /api/v2/TenantsService/UnitGroups/{unitGroupId}/Units/Count | Get the count of units in a unit group |
| [**patch_unit_async**](UnitGroupsApi.md#patch_unit_async) | **PATCH** /api/v2/TenantsService/UnitGroups/{unitGroupId}/Units/{unitId} | Patch a unit within a unit group |
| [**patch_unit_group_async**](UnitGroupsApi.md#patch_unit_group_async) | **PATCH** /api/v2/TenantsService/UnitGroups/{unitGroupId} | Patch a unit group |
| [**update_unit_async**](UnitGroupsApi.md#update_unit_async) | **PUT** /api/v2/TenantsService/UnitGroups/{unitGroupId}/Units/{unitId} | Update a unit within a unit group |
| [**update_unit_group_async**](UnitGroupsApi.md#update_unit_group_async) | **PUT** /api/v2/TenantsService/UnitGroups/{unitGroupId} | Update a unit group |


## create_unit_async

> <EmptyEnvelope> create_unit_async(tenant_id, unit_group_id, opts)

Create a unit within a unit group

Creates a new unit within a specific unit group.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
unit_group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  unit_create_dto: OpenapiClient::UnitCreateDto.new({name: 'name_example'}) # UnitCreateDto | 
}

begin
  # Create a unit within a unit group
  result = api_instance.create_unit_async(tenant_id, unit_group_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->create_unit_async: #{e}"
end
```

#### Using the create_unit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_unit_async_with_http_info(tenant_id, unit_group_id, opts)

```ruby
begin
  # Create a unit within a unit group
  data, status_code, headers = api_instance.create_unit_async_with_http_info(tenant_id, unit_group_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->create_unit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **unit_group_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **unit_create_dto** | [**UnitCreateDto**](UnitCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_unit_group_async

> <EmptyEnvelope> create_unit_group_async(tenant_id, opts)

Create a new unit group

Creates a new unit group for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  unit_group_create_dto: OpenapiClient::UnitGroupCreateDto.new({name: 'name_example'}) # UnitGroupCreateDto | 
}

begin
  # Create a new unit group
  result = api_instance.create_unit_group_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->create_unit_group_async: #{e}"
end
```

#### Using the create_unit_group_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_unit_group_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new unit group
  data, status_code, headers = api_instance.create_unit_group_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->create_unit_group_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **unit_group_create_dto** | [**UnitGroupCreateDto**](UnitGroupCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_unit_async

> <EmptyEnvelope> delete_unit_async(tenant_id, unit_group_id, unit_id, opts)

Delete a unit from a unit group

Deletes a unit from a specific unit group.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
unit_group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
unit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a unit from a unit group
  result = api_instance.delete_unit_async(tenant_id, unit_group_id, unit_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->delete_unit_async: #{e}"
end
```

#### Using the delete_unit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_unit_async_with_http_info(tenant_id, unit_group_id, unit_id, opts)

```ruby
begin
  # Delete a unit from a unit group
  data, status_code, headers = api_instance.delete_unit_async_with_http_info(tenant_id, unit_group_id, unit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->delete_unit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **unit_group_id** | **String** |  |  |
| **unit_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_unit_group_async

> <EmptyEnvelope> delete_unit_group_async(tenant_id, unit_group_id, opts)

Delete a unit group

Deletes a unit group by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
unit_group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a unit group
  result = api_instance.delete_unit_group_async(tenant_id, unit_group_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->delete_unit_group_async: #{e}"
end
```

#### Using the delete_unit_group_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_unit_group_async_with_http_info(tenant_id, unit_group_id, opts)

```ruby
begin
  # Delete a unit group
  data, status_code, headers = api_instance.delete_unit_group_async_with_http_info(tenant_id, unit_group_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->delete_unit_group_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **unit_group_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_unit_async

> <UnitDtoEnvelope> get_unit_async(tenant_id, unit_group_id, unit_id, opts)

Retrieve a unit by ID within a unit group

Retrieves a single unit by its unique identifier within a specific unit group.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
unit_group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
unit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a unit by ID within a unit group
  result = api_instance.get_unit_async(tenant_id, unit_group_id, unit_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->get_unit_async: #{e}"
end
```

#### Using the get_unit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<UnitDtoEnvelope>, Integer, Hash)> get_unit_async_with_http_info(tenant_id, unit_group_id, unit_id, opts)

```ruby
begin
  # Retrieve a unit by ID within a unit group
  data, status_code, headers = api_instance.get_unit_async_with_http_info(tenant_id, unit_group_id, unit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <UnitDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->get_unit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **unit_group_id** | **String** |  |  |
| **unit_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**UnitDtoEnvelope**](UnitDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_unit_group_async

> <UnitGroupDtoEnvelope> get_unit_group_async(tenant_id, unit_group_id, opts)

Retrieve a unit group by ID

Retrieves a single unit group by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
unit_group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a unit group by ID
  result = api_instance.get_unit_group_async(tenant_id, unit_group_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->get_unit_group_async: #{e}"
end
```

#### Using the get_unit_group_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<UnitGroupDtoEnvelope>, Integer, Hash)> get_unit_group_async_with_http_info(tenant_id, unit_group_id, opts)

```ruby
begin
  # Retrieve a unit group by ID
  data, status_code, headers = api_instance.get_unit_group_async_with_http_info(tenant_id, unit_group_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <UnitGroupDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->get_unit_group_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **unit_group_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**UnitGroupDtoEnvelope**](UnitGroupDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_unit_groups_async

> <UnitGroupDtoListEnvelope> get_unit_groups_async(tenant_id, opts)

Retrieve a list of unit groups

Retrieves a list of unit groups for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of unit groups
  result = api_instance.get_unit_groups_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->get_unit_groups_async: #{e}"
end
```

#### Using the get_unit_groups_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<UnitGroupDtoListEnvelope>, Integer, Hash)> get_unit_groups_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of unit groups
  data, status_code, headers = api_instance.get_unit_groups_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <UnitGroupDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->get_unit_groups_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**UnitGroupDtoListEnvelope**](UnitGroupDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_unit_groups_count_async

> <Int32Envelope> get_unit_groups_count_async(tenant_id, opts)

Get the count of unit groups

Returns the total count of unit groups for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of unit groups
  result = api_instance.get_unit_groups_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->get_unit_groups_count_async: #{e}"
end
```

#### Using the get_unit_groups_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_unit_groups_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of unit groups
  data, status_code, headers = api_instance.get_unit_groups_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->get_unit_groups_count_async_with_http_info: #{e}"
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


## get_units_async

> <UnitDtoListEnvelope> get_units_async(tenant_id, unit_group_id, opts)

Retrieve units for a unit group

Retrieves a list of units belonging to a specific unit group.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
unit_group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve units for a unit group
  result = api_instance.get_units_async(tenant_id, unit_group_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->get_units_async: #{e}"
end
```

#### Using the get_units_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<UnitDtoListEnvelope>, Integer, Hash)> get_units_async_with_http_info(tenant_id, unit_group_id, opts)

```ruby
begin
  # Retrieve units for a unit group
  data, status_code, headers = api_instance.get_units_async_with_http_info(tenant_id, unit_group_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <UnitDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->get_units_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **unit_group_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**UnitDtoListEnvelope**](UnitDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_units_count_async

> <Int32Envelope> get_units_count_async(tenant_id, unit_group_id, opts)

Get the count of units in a unit group

Returns the total count of units in a specific unit group.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
unit_group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of units in a unit group
  result = api_instance.get_units_count_async(tenant_id, unit_group_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->get_units_count_async: #{e}"
end
```

#### Using the get_units_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_units_count_async_with_http_info(tenant_id, unit_group_id, opts)

```ruby
begin
  # Get the count of units in a unit group
  data, status_code, headers = api_instance.get_units_count_async_with_http_info(tenant_id, unit_group_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->get_units_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **unit_group_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_unit_async

> <EmptyEnvelope> patch_unit_async(tenant_id, unit_group_id, unit_id, opts)

Patch a unit within a unit group

Partially updates an existing unit within a specific unit group.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
unit_group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
unit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a unit within a unit group
  result = api_instance.patch_unit_async(tenant_id, unit_group_id, unit_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->patch_unit_async: #{e}"
end
```

#### Using the patch_unit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_unit_async_with_http_info(tenant_id, unit_group_id, unit_id, opts)

```ruby
begin
  # Patch a unit within a unit group
  data, status_code, headers = api_instance.patch_unit_async_with_http_info(tenant_id, unit_group_id, unit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->patch_unit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **unit_group_id** | **String** |  |  |
| **unit_id** | **String** |  |  |
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


## patch_unit_group_async

> <EmptyEnvelope> patch_unit_group_async(tenant_id, unit_group_id, opts)

Patch a unit group

Partially updates an existing unit group by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
unit_group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a unit group
  result = api_instance.patch_unit_group_async(tenant_id, unit_group_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->patch_unit_group_async: #{e}"
end
```

#### Using the patch_unit_group_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_unit_group_async_with_http_info(tenant_id, unit_group_id, opts)

```ruby
begin
  # Patch a unit group
  data, status_code, headers = api_instance.patch_unit_group_async_with_http_info(tenant_id, unit_group_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->patch_unit_group_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **unit_group_id** | **String** |  |  |
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


## update_unit_async

> <EmptyEnvelope> update_unit_async(tenant_id, unit_group_id, unit_id, opts)

Update a unit within a unit group

Updates an existing unit within a specific unit group.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
unit_group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
unit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  unit_update_dto: OpenapiClient::UnitUpdateDto.new # UnitUpdateDto | 
}

begin
  # Update a unit within a unit group
  result = api_instance.update_unit_async(tenant_id, unit_group_id, unit_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->update_unit_async: #{e}"
end
```

#### Using the update_unit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_unit_async_with_http_info(tenant_id, unit_group_id, unit_id, opts)

```ruby
begin
  # Update a unit within a unit group
  data, status_code, headers = api_instance.update_unit_async_with_http_info(tenant_id, unit_group_id, unit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->update_unit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **unit_group_id** | **String** |  |  |
| **unit_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **unit_update_dto** | [**UnitUpdateDto**](UnitUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_unit_group_async

> <EmptyEnvelope> update_unit_group_async(tenant_id, unit_group_id, opts)

Update a unit group

Updates an existing unit group by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UnitGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
unit_group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  unit_group_update_dto: OpenapiClient::UnitGroupUpdateDto.new # UnitGroupUpdateDto | 
}

begin
  # Update a unit group
  result = api_instance.update_unit_group_async(tenant_id, unit_group_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->update_unit_group_async: #{e}"
end
```

#### Using the update_unit_group_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_unit_group_async_with_http_info(tenant_id, unit_group_id, opts)

```ruby
begin
  # Update a unit group
  data, status_code, headers = api_instance.update_unit_group_async_with_http_info(tenant_id, unit_group_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UnitGroupsApi->update_unit_group_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **unit_group_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **unit_group_update_dto** | [**UnitGroupUpdateDto**](UnitGroupUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

