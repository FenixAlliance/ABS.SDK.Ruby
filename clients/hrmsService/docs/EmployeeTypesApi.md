# OpenapiClient::EmployeeTypesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_employee_type_async**](EmployeeTypesApi.md#create_employee_type_async) | **POST** /api/v2/HrmsService/EmployeeTypes | Create an employee type |
| [**delete_employee_type_async**](EmployeeTypesApi.md#delete_employee_type_async) | **DELETE** /api/v2/HrmsService/EmployeeTypes/{employeeTypeId} | Delete an employee type |
| [**get_employee_type_by_id_async**](EmployeeTypesApi.md#get_employee_type_by_id_async) | **GET** /api/v2/HrmsService/EmployeeTypes/{employeeTypeId} | Get employee type by ID |
| [**get_employee_types_async**](EmployeeTypesApi.md#get_employee_types_async) | **GET** /api/v2/HrmsService/EmployeeTypes | Get employee types |
| [**get_employee_types_count_async**](EmployeeTypesApi.md#get_employee_types_count_async) | **GET** /api/v2/HrmsService/EmployeeTypes/Count | Count employee types |
| [**update_employee_type_async**](EmployeeTypesApi.md#update_employee_type_async) | **PUT** /api/v2/HrmsService/EmployeeTypes/{employeeTypeId} | Update an employee type |


## create_employee_type_async

> <EmptyEnvelope> create_employee_type_async(tenant_id, opts)

Create an employee type

Creates a new employee type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeeTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  employee_type_create_dto: OpenapiClient::EmployeeTypeCreateDto.new # EmployeeTypeCreateDto | 
}

begin
  # Create an employee type
  result = api_instance.create_employee_type_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeTypesApi->create_employee_type_async: #{e}"
end
```

#### Using the create_employee_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_employee_type_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create an employee type
  data, status_code, headers = api_instance.create_employee_type_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeTypesApi->create_employee_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **employee_type_create_dto** | [**EmployeeTypeCreateDto**](EmployeeTypeCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_employee_type_async

> <EmptyEnvelope> delete_employee_type_async(tenant_id, employee_type_id, opts)

Delete an employee type

Deletes an employee type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeeTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
employee_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an employee type
  result = api_instance.delete_employee_type_async(tenant_id, employee_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeTypesApi->delete_employee_type_async: #{e}"
end
```

#### Using the delete_employee_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_employee_type_async_with_http_info(tenant_id, employee_type_id, opts)

```ruby
begin
  # Delete an employee type
  data, status_code, headers = api_instance.delete_employee_type_async_with_http_info(tenant_id, employee_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeTypesApi->delete_employee_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **employee_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_employee_type_by_id_async

> <EmployeeTypeDtoEnvelope> get_employee_type_by_id_async(tenant_id, employee_type_id, opts)

Get employee type by ID

Retrieves a specific employee type by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeeTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
employee_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get employee type by ID
  result = api_instance.get_employee_type_by_id_async(tenant_id, employee_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeTypesApi->get_employee_type_by_id_async: #{e}"
end
```

#### Using the get_employee_type_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmployeeTypeDtoEnvelope>, Integer, Hash)> get_employee_type_by_id_async_with_http_info(tenant_id, employee_type_id, opts)

```ruby
begin
  # Get employee type by ID
  data, status_code, headers = api_instance.get_employee_type_by_id_async_with_http_info(tenant_id, employee_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmployeeTypeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeTypesApi->get_employee_type_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **employee_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmployeeTypeDtoEnvelope**](EmployeeTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_employee_types_async

> <EmployeeTypeDtoListEnvelope> get_employee_types_async(tenant_id, opts)

Get employee types

Retrieves employee types for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeeTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get employee types
  result = api_instance.get_employee_types_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeTypesApi->get_employee_types_async: #{e}"
end
```

#### Using the get_employee_types_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmployeeTypeDtoListEnvelope>, Integer, Hash)> get_employee_types_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get employee types
  data, status_code, headers = api_instance.get_employee_types_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmployeeTypeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeTypesApi->get_employee_types_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmployeeTypeDtoListEnvelope**](EmployeeTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_employee_types_count_async

> <Int32Envelope> get_employee_types_count_async(tenant_id, opts)

Count employee types

Counts employee types for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeeTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count employee types
  result = api_instance.get_employee_types_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeTypesApi->get_employee_types_count_async: #{e}"
end
```

#### Using the get_employee_types_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_employee_types_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count employee types
  data, status_code, headers = api_instance.get_employee_types_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeTypesApi->get_employee_types_count_async_with_http_info: #{e}"
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


## update_employee_type_async

> <EmptyEnvelope> update_employee_type_async(tenant_id, employee_type_id, opts)

Update an employee type

Updates an existing employee type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeeTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
employee_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  employee_type_update_dto: OpenapiClient::EmployeeTypeUpdateDto.new # EmployeeTypeUpdateDto | 
}

begin
  # Update an employee type
  result = api_instance.update_employee_type_async(tenant_id, employee_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeTypesApi->update_employee_type_async: #{e}"
end
```

#### Using the update_employee_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_employee_type_async_with_http_info(tenant_id, employee_type_id, opts)

```ruby
begin
  # Update an employee type
  data, status_code, headers = api_instance.update_employee_type_async_with_http_info(tenant_id, employee_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeTypesApi->update_employee_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **employee_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **employee_type_update_dto** | [**EmployeeTypeUpdateDto**](EmployeeTypeUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

