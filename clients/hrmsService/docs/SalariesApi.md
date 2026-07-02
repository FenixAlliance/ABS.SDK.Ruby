# OpenapiClient::SalariesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_salary_async**](SalariesApi.md#create_salary_async) | **POST** /api/v2/HrmsService/Salaries | Create a salary |
| [**delete_salary_async**](SalariesApi.md#delete_salary_async) | **DELETE** /api/v2/HrmsService/Salaries/{salaryId} | Delete a salary |
| [**get_salaries_async**](SalariesApi.md#get_salaries_async) | **GET** /api/v2/HrmsService/Salaries | Get salaries |
| [**get_salaries_count_async**](SalariesApi.md#get_salaries_count_async) | **GET** /api/v2/HrmsService/Salaries/Count | Count salaries |
| [**get_salary_by_id_async**](SalariesApi.md#get_salary_by_id_async) | **GET** /api/v2/HrmsService/Salaries/{salaryId} | Get salary by ID |
| [**patch_salary_async**](SalariesApi.md#patch_salary_async) | **PATCH** /api/v2/HrmsService/Salaries/{salaryId} | Patch a salary |
| [**update_salary_async**](SalariesApi.md#update_salary_async) | **PUT** /api/v2/HrmsService/Salaries/{salaryId} | Update a salary |


## create_salary_async

> <EmptyEnvelope> create_salary_async(tenant_id, opts)

Create a salary

Creates a new salary for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SalariesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  salary_create_dto: OpenapiClient::SalaryCreateDto.new({amount: 3.56, currency_id: 'currency_id_example', employee_profile_id: 'employee_profile_id_example'}) # SalaryCreateDto | 
}

begin
  # Create a salary
  result = api_instance.create_salary_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalariesApi->create_salary_async: #{e}"
end
```

#### Using the create_salary_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_salary_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a salary
  data, status_code, headers = api_instance.create_salary_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalariesApi->create_salary_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **salary_create_dto** | [**SalaryCreateDto**](SalaryCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_salary_async

> <EmptyEnvelope> delete_salary_async(tenant_id, salary_id, opts)

Delete a salary

Deletes a salary for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SalariesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
salary_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a salary
  result = api_instance.delete_salary_async(tenant_id, salary_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalariesApi->delete_salary_async: #{e}"
end
```

#### Using the delete_salary_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_salary_async_with_http_info(tenant_id, salary_id, opts)

```ruby
begin
  # Delete a salary
  data, status_code, headers = api_instance.delete_salary_async_with_http_info(tenant_id, salary_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalariesApi->delete_salary_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **salary_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_salaries_async

> <SalaryDtoListEnvelope> get_salaries_async(tenant_id, opts)

Get salaries

Retrieves salaries for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SalariesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get salaries
  result = api_instance.get_salaries_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalariesApi->get_salaries_async: #{e}"
end
```

#### Using the get_salaries_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SalaryDtoListEnvelope>, Integer, Hash)> get_salaries_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get salaries
  data, status_code, headers = api_instance.get_salaries_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SalaryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalariesApi->get_salaries_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SalaryDtoListEnvelope**](SalaryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_salaries_count_async

> <Int32Envelope> get_salaries_count_async(tenant_id, opts)

Count salaries

Counts salaries for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SalariesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count salaries
  result = api_instance.get_salaries_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalariesApi->get_salaries_count_async: #{e}"
end
```

#### Using the get_salaries_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_salaries_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count salaries
  data, status_code, headers = api_instance.get_salaries_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalariesApi->get_salaries_count_async_with_http_info: #{e}"
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


## get_salary_by_id_async

> <SalaryDtoEnvelope> get_salary_by_id_async(tenant_id, salary_id, opts)

Get salary by ID

Retrieves a specific salary by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SalariesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
salary_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get salary by ID
  result = api_instance.get_salary_by_id_async(tenant_id, salary_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalariesApi->get_salary_by_id_async: #{e}"
end
```

#### Using the get_salary_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SalaryDtoEnvelope>, Integer, Hash)> get_salary_by_id_async_with_http_info(tenant_id, salary_id, opts)

```ruby
begin
  # Get salary by ID
  data, status_code, headers = api_instance.get_salary_by_id_async_with_http_info(tenant_id, salary_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SalaryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalariesApi->get_salary_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **salary_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SalaryDtoEnvelope**](SalaryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_salary_async

> <EmptyEnvelope> patch_salary_async(tenant_id, salary_id, opts)

Patch a salary

Partially updates an existing salary for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SalariesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
salary_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a salary
  result = api_instance.patch_salary_async(tenant_id, salary_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalariesApi->patch_salary_async: #{e}"
end
```

#### Using the patch_salary_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_salary_async_with_http_info(tenant_id, salary_id, opts)

```ruby
begin
  # Patch a salary
  data, status_code, headers = api_instance.patch_salary_async_with_http_info(tenant_id, salary_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalariesApi->patch_salary_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **salary_id** | **String** |  |  |
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


## update_salary_async

> <EmptyEnvelope> update_salary_async(tenant_id, salary_id, opts)

Update a salary

Updates an existing salary for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SalariesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
salary_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  salary_update_dto: OpenapiClient::SalaryUpdateDto.new # SalaryUpdateDto | 
}

begin
  # Update a salary
  result = api_instance.update_salary_async(tenant_id, salary_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalariesApi->update_salary_async: #{e}"
end
```

#### Using the update_salary_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_salary_async_with_http_info(tenant_id, salary_id, opts)

```ruby
begin
  # Update a salary
  data, status_code, headers = api_instance.update_salary_async_with_http_info(tenant_id, salary_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SalariesApi->update_salary_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **salary_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **salary_update_dto** | [**SalaryUpdateDto**](SalaryUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

