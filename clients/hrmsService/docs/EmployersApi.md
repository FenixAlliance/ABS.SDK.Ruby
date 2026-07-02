# OpenapiClient::EmployersApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_employer_async**](EmployersApi.md#create_employer_async) | **POST** /api/v2/HrmsService/Employers | Create an employer |
| [**delete_employer_async**](EmployersApi.md#delete_employer_async) | **DELETE** /api/v2/HrmsService/Employers/{employerId} | Delete an employer |
| [**get_employer_by_id_async**](EmployersApi.md#get_employer_by_id_async) | **GET** /api/v2/HrmsService/Employers/{employerId} | Get employer by ID |
| [**get_employers_async**](EmployersApi.md#get_employers_async) | **GET** /api/v2/HrmsService/Employers | Get employers |
| [**get_employers_count_async**](EmployersApi.md#get_employers_count_async) | **GET** /api/v2/HrmsService/Employers/Count | Count employers |
| [**patch_employer_async**](EmployersApi.md#patch_employer_async) | **PATCH** /api/v2/HrmsService/Employers/{employerId} | Patch an employer |
| [**update_employer_async**](EmployersApi.md#update_employer_async) | **PUT** /api/v2/HrmsService/Employers/{employerId} | Update an employer |


## create_employer_async

> <EmptyEnvelope> create_employer_async(tenant_id, opts)

Create an employer

Creates a new employer for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  employer_profile_create_dto: OpenapiClient::EmployerProfileCreateDto.new # EmployerProfileCreateDto | 
}

begin
  # Create an employer
  result = api_instance.create_employer_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployersApi->create_employer_async: #{e}"
end
```

#### Using the create_employer_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_employer_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create an employer
  data, status_code, headers = api_instance.create_employer_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployersApi->create_employer_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **employer_profile_create_dto** | [**EmployerProfileCreateDto**](EmployerProfileCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_employer_async

> <EmptyEnvelope> delete_employer_async(tenant_id, employer_id, opts)

Delete an employer

Deletes an employer for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
employer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an employer
  result = api_instance.delete_employer_async(tenant_id, employer_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployersApi->delete_employer_async: #{e}"
end
```

#### Using the delete_employer_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_employer_async_with_http_info(tenant_id, employer_id, opts)

```ruby
begin
  # Delete an employer
  data, status_code, headers = api_instance.delete_employer_async_with_http_info(tenant_id, employer_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployersApi->delete_employer_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **employer_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_employer_by_id_async

> <EmployerProfileDtoEnvelope> get_employer_by_id_async(tenant_id, employer_id, opts)

Get employer by ID

Retrieves a specific employer by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
employer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get employer by ID
  result = api_instance.get_employer_by_id_async(tenant_id, employer_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployersApi->get_employer_by_id_async: #{e}"
end
```

#### Using the get_employer_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmployerProfileDtoEnvelope>, Integer, Hash)> get_employer_by_id_async_with_http_info(tenant_id, employer_id, opts)

```ruby
begin
  # Get employer by ID
  data, status_code, headers = api_instance.get_employer_by_id_async_with_http_info(tenant_id, employer_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmployerProfileDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployersApi->get_employer_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **employer_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmployerProfileDtoEnvelope**](EmployerProfileDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_employers_async

> <EmployerProfileDtoListEnvelope> get_employers_async(tenant_id, opts)

Get employers

Retrieves employers for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get employers
  result = api_instance.get_employers_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployersApi->get_employers_async: #{e}"
end
```

#### Using the get_employers_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmployerProfileDtoListEnvelope>, Integer, Hash)> get_employers_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get employers
  data, status_code, headers = api_instance.get_employers_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmployerProfileDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployersApi->get_employers_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmployerProfileDtoListEnvelope**](EmployerProfileDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_employers_count_async

> <Int32Envelope> get_employers_count_async(tenant_id, opts)

Count employers

Counts employers for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count employers
  result = api_instance.get_employers_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployersApi->get_employers_count_async: #{e}"
end
```

#### Using the get_employers_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_employers_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count employers
  data, status_code, headers = api_instance.get_employers_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployersApi->get_employers_count_async_with_http_info: #{e}"
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


## patch_employer_async

> <EmptyEnvelope> patch_employer_async(tenant_id, employer_id, opts)

Patch an employer

Partially updates an existing employer for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
employer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch an employer
  result = api_instance.patch_employer_async(tenant_id, employer_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployersApi->patch_employer_async: #{e}"
end
```

#### Using the patch_employer_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_employer_async_with_http_info(tenant_id, employer_id, opts)

```ruby
begin
  # Patch an employer
  data, status_code, headers = api_instance.patch_employer_async_with_http_info(tenant_id, employer_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployersApi->patch_employer_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **employer_id** | **String** |  |  |
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


## update_employer_async

> <EmptyEnvelope> update_employer_async(tenant_id, employer_id, opts)

Update an employer

Updates an existing employer for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
employer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  employer_profile_update_dto: OpenapiClient::EmployerProfileUpdateDto.new # EmployerProfileUpdateDto | 
}

begin
  # Update an employer
  result = api_instance.update_employer_async(tenant_id, employer_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployersApi->update_employer_async: #{e}"
end
```

#### Using the update_employer_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_employer_async_with_http_info(tenant_id, employer_id, opts)

```ruby
begin
  # Update an employer
  data, status_code, headers = api_instance.update_employer_async_with_http_info(tenant_id, employer_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployersApi->update_employer_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **employer_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **employer_profile_update_dto** | [**EmployerProfileUpdateDto**](EmployerProfileUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

