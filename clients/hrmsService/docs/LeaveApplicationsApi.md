# OpenapiClient::LeaveApplicationsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_leave_application_async**](LeaveApplicationsApi.md#create_leave_application_async) | **POST** /api/v2/HrmsService/LeaveApplications | Create a leave application |
| [**delete_leave_application_async**](LeaveApplicationsApi.md#delete_leave_application_async) | **DELETE** /api/v2/HrmsService/LeaveApplications/{leaveApplicationId} | Delete a leave application |
| [**get_leave_application_by_id_async**](LeaveApplicationsApi.md#get_leave_application_by_id_async) | **GET** /api/v2/HrmsService/LeaveApplications/{leaveApplicationId} | Get leave application by ID |
| [**get_leave_applications_async**](LeaveApplicationsApi.md#get_leave_applications_async) | **GET** /api/v2/HrmsService/LeaveApplications | Get leave applications |
| [**get_leave_applications_count_async**](LeaveApplicationsApi.md#get_leave_applications_count_async) | **GET** /api/v2/HrmsService/LeaveApplications/Count | Count leave applications |
| [**patch_leave_application_async**](LeaveApplicationsApi.md#patch_leave_application_async) | **PATCH** /api/v2/HrmsService/LeaveApplications/{leaveApplicationId} | Patch a leave application |
| [**update_leave_application_async**](LeaveApplicationsApi.md#update_leave_application_async) | **PUT** /api/v2/HrmsService/LeaveApplications/{leaveApplicationId} | Update a leave application |


## create_leave_application_async

> <EmptyEnvelope> create_leave_application_async(tenant_id, opts)

Create a leave application

Creates a new leave application for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LeaveApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  leave_application_create_dto: OpenapiClient::LeaveApplicationCreateDto.new({leave_type_id: 'leave_type_id_example', employee_profile_id: 'employee_profile_id_example'}) # LeaveApplicationCreateDto | 
}

begin
  # Create a leave application
  result = api_instance.create_leave_application_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveApplicationsApi->create_leave_application_async: #{e}"
end
```

#### Using the create_leave_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_leave_application_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a leave application
  data, status_code, headers = api_instance.create_leave_application_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveApplicationsApi->create_leave_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **leave_application_create_dto** | [**LeaveApplicationCreateDto**](LeaveApplicationCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_leave_application_async

> <EmptyEnvelope> delete_leave_application_async(tenant_id, leave_application_id, opts)

Delete a leave application

Deletes a leave application for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LeaveApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
leave_application_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a leave application
  result = api_instance.delete_leave_application_async(tenant_id, leave_application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveApplicationsApi->delete_leave_application_async: #{e}"
end
```

#### Using the delete_leave_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_leave_application_async_with_http_info(tenant_id, leave_application_id, opts)

```ruby
begin
  # Delete a leave application
  data, status_code, headers = api_instance.delete_leave_application_async_with_http_info(tenant_id, leave_application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveApplicationsApi->delete_leave_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **leave_application_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_leave_application_by_id_async

> <LeaveApplicationDtoEnvelope> get_leave_application_by_id_async(tenant_id, leave_application_id, opts)

Get leave application by ID

Retrieves a specific leave application by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LeaveApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
leave_application_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get leave application by ID
  result = api_instance.get_leave_application_by_id_async(tenant_id, leave_application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveApplicationsApi->get_leave_application_by_id_async: #{e}"
end
```

#### Using the get_leave_application_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LeaveApplicationDtoEnvelope>, Integer, Hash)> get_leave_application_by_id_async_with_http_info(tenant_id, leave_application_id, opts)

```ruby
begin
  # Get leave application by ID
  data, status_code, headers = api_instance.get_leave_application_by_id_async_with_http_info(tenant_id, leave_application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LeaveApplicationDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveApplicationsApi->get_leave_application_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **leave_application_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**LeaveApplicationDtoEnvelope**](LeaveApplicationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_leave_applications_async

> <LeaveApplicationDtoListEnvelope> get_leave_applications_async(tenant_id, opts)

Get leave applications

Retrieves leave applications for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LeaveApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get leave applications
  result = api_instance.get_leave_applications_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveApplicationsApi->get_leave_applications_async: #{e}"
end
```

#### Using the get_leave_applications_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LeaveApplicationDtoListEnvelope>, Integer, Hash)> get_leave_applications_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get leave applications
  data, status_code, headers = api_instance.get_leave_applications_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LeaveApplicationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveApplicationsApi->get_leave_applications_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**LeaveApplicationDtoListEnvelope**](LeaveApplicationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_leave_applications_count_async

> <Int32Envelope> get_leave_applications_count_async(tenant_id, opts)

Count leave applications

Counts leave applications for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LeaveApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count leave applications
  result = api_instance.get_leave_applications_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveApplicationsApi->get_leave_applications_count_async: #{e}"
end
```

#### Using the get_leave_applications_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_leave_applications_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count leave applications
  data, status_code, headers = api_instance.get_leave_applications_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveApplicationsApi->get_leave_applications_count_async_with_http_info: #{e}"
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


## patch_leave_application_async

> <EmptyEnvelope> patch_leave_application_async(tenant_id, leave_application_id, opts)

Patch a leave application

Partially updates an existing leave application for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LeaveApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
leave_application_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a leave application
  result = api_instance.patch_leave_application_async(tenant_id, leave_application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveApplicationsApi->patch_leave_application_async: #{e}"
end
```

#### Using the patch_leave_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_leave_application_async_with_http_info(tenant_id, leave_application_id, opts)

```ruby
begin
  # Patch a leave application
  data, status_code, headers = api_instance.patch_leave_application_async_with_http_info(tenant_id, leave_application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveApplicationsApi->patch_leave_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **leave_application_id** | **String** |  |  |
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


## update_leave_application_async

> <EmptyEnvelope> update_leave_application_async(tenant_id, leave_application_id, opts)

Update a leave application

Updates an existing leave application for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LeaveApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
leave_application_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  leave_application_update_dto: OpenapiClient::LeaveApplicationUpdateDto.new # LeaveApplicationUpdateDto | 
}

begin
  # Update a leave application
  result = api_instance.update_leave_application_async(tenant_id, leave_application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveApplicationsApi->update_leave_application_async: #{e}"
end
```

#### Using the update_leave_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_leave_application_async_with_http_info(tenant_id, leave_application_id, opts)

```ruby
begin
  # Update a leave application
  data, status_code, headers = api_instance.update_leave_application_async_with_http_info(tenant_id, leave_application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveApplicationsApi->update_leave_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **leave_application_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **leave_application_update_dto** | [**LeaveApplicationUpdateDto**](LeaveApplicationUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

