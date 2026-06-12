# OpenapiClient::EmployeesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_employee_async**](EmployeesApi.md#create_employee_async) | **POST** /api/v2/HrmsService/Employees | Create an employee |
| [**delete_employee_async**](EmployeesApi.md#delete_employee_async) | **DELETE** /api/v2/HrmsService/Employees/{employeeId} | Delete an employee |
| [**get_employee_by_id_async**](EmployeesApi.md#get_employee_by_id_async) | **GET** /api/v2/HrmsService/Employees/{employeeId} | Get employee by ID |
| [**get_employees_async**](EmployeesApi.md#get_employees_async) | **GET** /api/v2/HrmsService/Employees | Get employees |
| [**get_employees_count_async**](EmployeesApi.md#get_employees_count_async) | **GET** /api/v2/HrmsService/Employees/Count | Count employees |
| [**patch_employee_async**](EmployeesApi.md#patch_employee_async) | **PATCH** /api/v2/HrmsService/Employees/{employeeId} | Patch an employee |
| [**update_employee_async**](EmployeesApi.md#update_employee_async) | **PUT** /api/v2/HrmsService/Employees/{employeeId} | Update an employee |


## create_employee_async

> <EmptyEnvelope> create_employee_async(tenant_id, opts)

Create an employee

Creates a new employee for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  employee_profile_create_dto: OpenapiClient::EmployeeProfileCreateDto.new # EmployeeProfileCreateDto | 
}

begin
  # Create an employee
  result = api_instance.create_employee_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeesApi->create_employee_async: #{e}"
end
```

#### Using the create_employee_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_employee_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create an employee
  data, status_code, headers = api_instance.create_employee_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeesApi->create_employee_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **employee_profile_create_dto** | [**EmployeeProfileCreateDto**](EmployeeProfileCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_employee_async

> <EmptyEnvelope> delete_employee_async(tenant_id, employee_id, opts)

Delete an employee

Deletes an employee for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
employee_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an employee
  result = api_instance.delete_employee_async(tenant_id, employee_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeesApi->delete_employee_async: #{e}"
end
```

#### Using the delete_employee_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_employee_async_with_http_info(tenant_id, employee_id, opts)

```ruby
begin
  # Delete an employee
  data, status_code, headers = api_instance.delete_employee_async_with_http_info(tenant_id, employee_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeesApi->delete_employee_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **employee_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_employee_by_id_async

> <EmployeeProfileDtoEnvelope> get_employee_by_id_async(tenant_id, employee_id, opts)

Get employee by ID

Retrieves a specific employee by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
employee_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get employee by ID
  result = api_instance.get_employee_by_id_async(tenant_id, employee_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeesApi->get_employee_by_id_async: #{e}"
end
```

#### Using the get_employee_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmployeeProfileDtoEnvelope>, Integer, Hash)> get_employee_by_id_async_with_http_info(tenant_id, employee_id, opts)

```ruby
begin
  # Get employee by ID
  data, status_code, headers = api_instance.get_employee_by_id_async_with_http_info(tenant_id, employee_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmployeeProfileDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeesApi->get_employee_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **employee_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmployeeProfileDtoEnvelope**](EmployeeProfileDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_employees_async

> <EmployeeProfileDtoListEnvelope> get_employees_async(tenant_id, opts)

Get employees

Retrieves employees for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get employees
  result = api_instance.get_employees_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeesApi->get_employees_async: #{e}"
end
```

#### Using the get_employees_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmployeeProfileDtoListEnvelope>, Integer, Hash)> get_employees_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get employees
  data, status_code, headers = api_instance.get_employees_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmployeeProfileDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeesApi->get_employees_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmployeeProfileDtoListEnvelope**](EmployeeProfileDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_employees_count_async

> <Int32Envelope> get_employees_count_async(tenant_id, opts)

Count employees

Counts employees for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count employees
  result = api_instance.get_employees_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeesApi->get_employees_count_async: #{e}"
end
```

#### Using the get_employees_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_employees_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count employees
  data, status_code, headers = api_instance.get_employees_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeesApi->get_employees_count_async_with_http_info: #{e}"
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


## patch_employee_async

> <EmptyEnvelope> patch_employee_async(tenant_id, employee_id, opts)

Patch an employee

Partially updates an existing employee for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
employee_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch an employee
  result = api_instance.patch_employee_async(tenant_id, employee_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeesApi->patch_employee_async: #{e}"
end
```

#### Using the patch_employee_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_employee_async_with_http_info(tenant_id, employee_id, opts)

```ruby
begin
  # Patch an employee
  data, status_code, headers = api_instance.patch_employee_async_with_http_info(tenant_id, employee_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeesApi->patch_employee_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **employee_id** | **String** |  |  |
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


## update_employee_async

> <EmptyEnvelope> update_employee_async(tenant_id, employee_id, opts)

Update an employee

Updates an existing employee for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
employee_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  employee_profile_update_dto: OpenapiClient::EmployeeProfileUpdateDto.new # EmployeeProfileUpdateDto | 
}

begin
  # Update an employee
  result = api_instance.update_employee_async(tenant_id, employee_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeesApi->update_employee_async: #{e}"
end
```

#### Using the update_employee_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_employee_async_with_http_info(tenant_id, employee_id, opts)

```ruby
begin
  # Update an employee
  data, status_code, headers = api_instance.update_employee_async_with_http_info(tenant_id, employee_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeesApi->update_employee_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **employee_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **employee_profile_update_dto** | [**EmployeeProfileUpdateDto**](EmployeeProfileUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

