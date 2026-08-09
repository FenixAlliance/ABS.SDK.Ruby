# OpenapiClient::DepartmentsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_tenant_department**](DepartmentsApi.md#create_tenant_department) | **POST** /api/v2/TenantsService/Departments | Create a new tenant department |
| [**delete_tenant_department**](DepartmentsApi.md#delete_tenant_department) | **DELETE** /api/v2/TenantsService/Departments/{tenantDepartmentId} | Delete a tenant department |
| [**get_tenant_department_by_id**](DepartmentsApi.md#get_tenant_department_by_id) | **GET** /api/v2/TenantsService/Departments/{tenantDepartmentId} | Retrieve a single tenant department by its ID |
| [**get_tenant_departments**](DepartmentsApi.md#get_tenant_departments) | **GET** /api/v2/TenantsService/Departments | Retrieve a list of tenant departments |
| [**get_tenant_departments_count**](DepartmentsApi.md#get_tenant_departments_count) | **GET** /api/v2/TenantsService/Departments/Count | Get the count of tenant departments |
| [**patch_tenant_department_async**](DepartmentsApi.md#patch_tenant_department_async) | **PATCH** /api/v2/TenantsService/Departments/{tenantDepartmentId} | Patch a tenant department |
| [**update_tenant_department**](DepartmentsApi.md#update_tenant_department) | **PUT** /api/v2/TenantsService/Departments/{tenantDepartmentId} | Update a tenant department |


## create_tenant_department

> <EmptyEnvelope> create_tenant_department(tenant_id, opts)

Create a new tenant department

Create a new tenant department

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DepartmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_department_create_dto: OpenapiClient::TenantDepartmentCreateDto.new # TenantDepartmentCreateDto | 
}

begin
  # Create a new tenant department
  result = api_instance.create_tenant_department(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DepartmentsApi->create_tenant_department: #{e}"
end
```

#### Using the create_tenant_department_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tenant_department_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new tenant department
  data, status_code, headers = api_instance.create_tenant_department_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DepartmentsApi->create_tenant_department_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_department_create_dto** | [**TenantDepartmentCreateDto**](TenantDepartmentCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_tenant_department

> <EmptyEnvelope> delete_tenant_department(tenant_id, tenant_department_id, opts)

Delete a tenant department

Delete a tenant department

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DepartmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_department_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tenant department
  result = api_instance.delete_tenant_department(tenant_id, tenant_department_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DepartmentsApi->delete_tenant_department: #{e}"
end
```

#### Using the delete_tenant_department_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tenant_department_with_http_info(tenant_id, tenant_department_id, opts)

```ruby
begin
  # Delete a tenant department
  data, status_code, headers = api_instance.delete_tenant_department_with_http_info(tenant_id, tenant_department_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DepartmentsApi->delete_tenant_department_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_department_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_department_by_id

> <TenantDepartmentDtoEnvelope> get_tenant_department_by_id(tenant_id, tenant_department_id, opts)

Retrieve a single tenant department by its ID

Retrieve a single tenant department by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DepartmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_department_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single tenant department by its ID
  result = api_instance.get_tenant_department_by_id(tenant_id, tenant_department_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DepartmentsApi->get_tenant_department_by_id: #{e}"
end
```

#### Using the get_tenant_department_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantDepartmentDtoEnvelope>, Integer, Hash)> get_tenant_department_by_id_with_http_info(tenant_id, tenant_department_id, opts)

```ruby
begin
  # Retrieve a single tenant department by its ID
  data, status_code, headers = api_instance.get_tenant_department_by_id_with_http_info(tenant_id, tenant_department_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantDepartmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DepartmentsApi->get_tenant_department_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_department_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantDepartmentDtoEnvelope**](TenantDepartmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_departments

> <TenantDepartmentDtoListEnvelope> get_tenant_departments(tenant_id, opts)

Retrieve a list of tenant departments

Retrieve a list of tenant departments

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DepartmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_department_dto_collection_query_parameters: OpenapiClient::TenantDepartmentDtoCollectionQueryParameters.new # TenantDepartmentDtoCollectionQueryParameters | 
}

begin
  # Retrieve a list of tenant departments
  result = api_instance.get_tenant_departments(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DepartmentsApi->get_tenant_departments: #{e}"
end
```

#### Using the get_tenant_departments_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantDepartmentDtoListEnvelope>, Integer, Hash)> get_tenant_departments_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of tenant departments
  data, status_code, headers = api_instance.get_tenant_departments_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantDepartmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DepartmentsApi->get_tenant_departments_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_department_dto_collection_query_parameters** | [**TenantDepartmentDtoCollectionQueryParameters**](TenantDepartmentDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**TenantDepartmentDtoListEnvelope**](TenantDepartmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_tenant_departments_count

> <Int32Envelope> get_tenant_departments_count(tenant_id, opts)

Get the count of tenant departments

Get the count of tenant departments

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DepartmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_department_dto_collection_query_parameters: OpenapiClient::TenantDepartmentDtoCollectionQueryParameters.new # TenantDepartmentDtoCollectionQueryParameters | 
}

begin
  # Get the count of tenant departments
  result = api_instance.get_tenant_departments_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DepartmentsApi->get_tenant_departments_count: #{e}"
end
```

#### Using the get_tenant_departments_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tenant_departments_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of tenant departments
  data, status_code, headers = api_instance.get_tenant_departments_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DepartmentsApi->get_tenant_departments_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_department_dto_collection_query_parameters** | [**TenantDepartmentDtoCollectionQueryParameters**](TenantDepartmentDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_tenant_department_async

> <EmptyEnvelope> patch_tenant_department_async(tenant_id, tenant_department_id, opts)

Patch a tenant department

Patch a tenant department

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DepartmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_department_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a tenant department
  result = api_instance.patch_tenant_department_async(tenant_id, tenant_department_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DepartmentsApi->patch_tenant_department_async: #{e}"
end
```

#### Using the patch_tenant_department_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_tenant_department_async_with_http_info(tenant_id, tenant_department_id, opts)

```ruby
begin
  # Patch a tenant department
  data, status_code, headers = api_instance.patch_tenant_department_async_with_http_info(tenant_id, tenant_department_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DepartmentsApi->patch_tenant_department_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_department_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_tenant_department

> <EmptyEnvelope> update_tenant_department(tenant_id, tenant_department_id, opts)

Update a tenant department

Update a tenant department

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DepartmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_department_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_department_update_dto: OpenapiClient::TenantDepartmentUpdateDto.new # TenantDepartmentUpdateDto | 
}

begin
  # Update a tenant department
  result = api_instance.update_tenant_department(tenant_id, tenant_department_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DepartmentsApi->update_tenant_department: #{e}"
end
```

#### Using the update_tenant_department_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tenant_department_with_http_info(tenant_id, tenant_department_id, opts)

```ruby
begin
  # Update a tenant department
  data, status_code, headers = api_instance.update_tenant_department_with_http_info(tenant_id, tenant_department_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DepartmentsApi->update_tenant_department_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_department_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_department_update_dto** | [**TenantDepartmentUpdateDto**](TenantDepartmentUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

