# OpenapiClient::EmployeeAppraisalSessionsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_employee_appraisal_session_async**](EmployeeAppraisalSessionsApi.md#create_employee_appraisal_session_async) | **POST** /api/v2/HrmsService/EmployeeAppraisalSessions | Create an employee appraisal session |
| [**delete_employee_appraisal_session_async**](EmployeeAppraisalSessionsApi.md#delete_employee_appraisal_session_async) | **DELETE** /api/v2/HrmsService/EmployeeAppraisalSessions/{sessionId} | Delete an employee appraisal session |
| [**get_employee_appraisal_session_by_id_async**](EmployeeAppraisalSessionsApi.md#get_employee_appraisal_session_by_id_async) | **GET** /api/v2/HrmsService/EmployeeAppraisalSessions/{sessionId} | Get employee appraisal session by ID |
| [**get_employee_appraisal_sessions_async**](EmployeeAppraisalSessionsApi.md#get_employee_appraisal_sessions_async) | **GET** /api/v2/HrmsService/EmployeeAppraisalSessions | Get employee appraisal sessions |
| [**get_employee_appraisal_sessions_count_async**](EmployeeAppraisalSessionsApi.md#get_employee_appraisal_sessions_count_async) | **GET** /api/v2/HrmsService/EmployeeAppraisalSessions/Count | Count employee appraisal sessions |
| [**patch_employee_appraisal_session_async**](EmployeeAppraisalSessionsApi.md#patch_employee_appraisal_session_async) | **PATCH** /api/v2/HrmsService/EmployeeAppraisalSessions/{sessionId} | Patch an employee appraisal session |
| [**update_employee_appraisal_session_async**](EmployeeAppraisalSessionsApi.md#update_employee_appraisal_session_async) | **PUT** /api/v2/HrmsService/EmployeeAppraisalSessions/{sessionId} | Update an employee appraisal session |


## create_employee_appraisal_session_async

> <EmptyEnvelope> create_employee_appraisal_session_async(tenant_id, opts)

Create an employee appraisal session

Creates a new employee appraisal session for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeeAppraisalSessionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  employee_appraisal_session_create_dto: OpenapiClient::EmployeeAppraisalSessionCreateDto.new({employee_profile_id: 'employee_profile_id_example', appraisal_workflow_id: 'appraisal_workflow_id_example'}) # EmployeeAppraisalSessionCreateDto | 
}

begin
  # Create an employee appraisal session
  result = api_instance.create_employee_appraisal_session_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeAppraisalSessionsApi->create_employee_appraisal_session_async: #{e}"
end
```

#### Using the create_employee_appraisal_session_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_employee_appraisal_session_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create an employee appraisal session
  data, status_code, headers = api_instance.create_employee_appraisal_session_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeAppraisalSessionsApi->create_employee_appraisal_session_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **employee_appraisal_session_create_dto** | [**EmployeeAppraisalSessionCreateDto**](EmployeeAppraisalSessionCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_employee_appraisal_session_async

> <EmptyEnvelope> delete_employee_appraisal_session_async(tenant_id, session_id, opts)

Delete an employee appraisal session

Deletes an employee appraisal session for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeeAppraisalSessionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
session_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an employee appraisal session
  result = api_instance.delete_employee_appraisal_session_async(tenant_id, session_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeAppraisalSessionsApi->delete_employee_appraisal_session_async: #{e}"
end
```

#### Using the delete_employee_appraisal_session_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_employee_appraisal_session_async_with_http_info(tenant_id, session_id, opts)

```ruby
begin
  # Delete an employee appraisal session
  data, status_code, headers = api_instance.delete_employee_appraisal_session_async_with_http_info(tenant_id, session_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeAppraisalSessionsApi->delete_employee_appraisal_session_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **session_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_employee_appraisal_session_by_id_async

> <EmployeeAppraisalSessionDtoEnvelope> get_employee_appraisal_session_by_id_async(tenant_id, session_id, opts)

Get employee appraisal session by ID

Retrieves a specific employee appraisal session by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeeAppraisalSessionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
session_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get employee appraisal session by ID
  result = api_instance.get_employee_appraisal_session_by_id_async(tenant_id, session_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeAppraisalSessionsApi->get_employee_appraisal_session_by_id_async: #{e}"
end
```

#### Using the get_employee_appraisal_session_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmployeeAppraisalSessionDtoEnvelope>, Integer, Hash)> get_employee_appraisal_session_by_id_async_with_http_info(tenant_id, session_id, opts)

```ruby
begin
  # Get employee appraisal session by ID
  data, status_code, headers = api_instance.get_employee_appraisal_session_by_id_async_with_http_info(tenant_id, session_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmployeeAppraisalSessionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeAppraisalSessionsApi->get_employee_appraisal_session_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **session_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmployeeAppraisalSessionDtoEnvelope**](EmployeeAppraisalSessionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_employee_appraisal_sessions_async

> <EmployeeAppraisalSessionDtoListEnvelope> get_employee_appraisal_sessions_async(tenant_id, opts)

Get employee appraisal sessions

Retrieves employee appraisal sessions for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeeAppraisalSessionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get employee appraisal sessions
  result = api_instance.get_employee_appraisal_sessions_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeAppraisalSessionsApi->get_employee_appraisal_sessions_async: #{e}"
end
```

#### Using the get_employee_appraisal_sessions_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmployeeAppraisalSessionDtoListEnvelope>, Integer, Hash)> get_employee_appraisal_sessions_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get employee appraisal sessions
  data, status_code, headers = api_instance.get_employee_appraisal_sessions_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmployeeAppraisalSessionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeAppraisalSessionsApi->get_employee_appraisal_sessions_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmployeeAppraisalSessionDtoListEnvelope**](EmployeeAppraisalSessionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_employee_appraisal_sessions_count_async

> <Int32Envelope> get_employee_appraisal_sessions_count_async(tenant_id, opts)

Count employee appraisal sessions

Counts employee appraisal sessions for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeeAppraisalSessionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count employee appraisal sessions
  result = api_instance.get_employee_appraisal_sessions_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeAppraisalSessionsApi->get_employee_appraisal_sessions_count_async: #{e}"
end
```

#### Using the get_employee_appraisal_sessions_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_employee_appraisal_sessions_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count employee appraisal sessions
  data, status_code, headers = api_instance.get_employee_appraisal_sessions_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeAppraisalSessionsApi->get_employee_appraisal_sessions_count_async_with_http_info: #{e}"
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


## patch_employee_appraisal_session_async

> <EmptyEnvelope> patch_employee_appraisal_session_async(tenant_id, session_id, opts)

Patch an employee appraisal session

Partially updates an existing employee appraisal session for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeeAppraisalSessionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
session_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch an employee appraisal session
  result = api_instance.patch_employee_appraisal_session_async(tenant_id, session_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeAppraisalSessionsApi->patch_employee_appraisal_session_async: #{e}"
end
```

#### Using the patch_employee_appraisal_session_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_employee_appraisal_session_async_with_http_info(tenant_id, session_id, opts)

```ruby
begin
  # Patch an employee appraisal session
  data, status_code, headers = api_instance.patch_employee_appraisal_session_async_with_http_info(tenant_id, session_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeAppraisalSessionsApi->patch_employee_appraisal_session_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **session_id** | **String** |  |  |
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


## update_employee_appraisal_session_async

> <EmptyEnvelope> update_employee_appraisal_session_async(tenant_id, session_id, opts)

Update an employee appraisal session

Updates an existing employee appraisal session for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeeAppraisalSessionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
session_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  employee_appraisal_session_update_dto: OpenapiClient::EmployeeAppraisalSessionUpdateDto.new # EmployeeAppraisalSessionUpdateDto | 
}

begin
  # Update an employee appraisal session
  result = api_instance.update_employee_appraisal_session_async(tenant_id, session_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeAppraisalSessionsApi->update_employee_appraisal_session_async: #{e}"
end
```

#### Using the update_employee_appraisal_session_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_employee_appraisal_session_async_with_http_info(tenant_id, session_id, opts)

```ruby
begin
  # Update an employee appraisal session
  data, status_code, headers = api_instance.update_employee_appraisal_session_async_with_http_info(tenant_id, session_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeAppraisalSessionsApi->update_employee_appraisal_session_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **session_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **employee_appraisal_session_update_dto** | [**EmployeeAppraisalSessionUpdateDto**](EmployeeAppraisalSessionUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

