# OpenapiClient::LeaveTypesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_leave_type_async**](LeaveTypesApi.md#create_leave_type_async) | **POST** /api/v2/HrmsService/LeaveTypes | Create a leave type |
| [**delete_leave_type_async**](LeaveTypesApi.md#delete_leave_type_async) | **DELETE** /api/v2/HrmsService/LeaveTypes/{leaveTypeId} | Delete a leave type |
| [**get_leave_type_by_id_async**](LeaveTypesApi.md#get_leave_type_by_id_async) | **GET** /api/v2/HrmsService/LeaveTypes/{leaveTypeId} | Get leave type by ID |
| [**get_leave_types_async**](LeaveTypesApi.md#get_leave_types_async) | **GET** /api/v2/HrmsService/LeaveTypes | Get leave types |
| [**get_leave_types_count_async**](LeaveTypesApi.md#get_leave_types_count_async) | **GET** /api/v2/HrmsService/LeaveTypes/Count | Count leave types |
| [**update_leave_type_async**](LeaveTypesApi.md#update_leave_type_async) | **PUT** /api/v2/HrmsService/LeaveTypes/{leaveTypeId} | Update a leave type |


## create_leave_type_async

> <EmptyEnvelope> create_leave_type_async(tenant_id, opts)

Create a leave type

Creates a new leave type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LeaveTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  leave_type_create_dto: OpenapiClient::LeaveTypeCreateDto.new({title: 'title_example'}) # LeaveTypeCreateDto | 
}

begin
  # Create a leave type
  result = api_instance.create_leave_type_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveTypesApi->create_leave_type_async: #{e}"
end
```

#### Using the create_leave_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_leave_type_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a leave type
  data, status_code, headers = api_instance.create_leave_type_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveTypesApi->create_leave_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **leave_type_create_dto** | [**LeaveTypeCreateDto**](LeaveTypeCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_leave_type_async

> <EmptyEnvelope> delete_leave_type_async(tenant_id, leave_type_id, opts)

Delete a leave type

Deletes a leave type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LeaveTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
leave_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a leave type
  result = api_instance.delete_leave_type_async(tenant_id, leave_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveTypesApi->delete_leave_type_async: #{e}"
end
```

#### Using the delete_leave_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_leave_type_async_with_http_info(tenant_id, leave_type_id, opts)

```ruby
begin
  # Delete a leave type
  data, status_code, headers = api_instance.delete_leave_type_async_with_http_info(tenant_id, leave_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveTypesApi->delete_leave_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **leave_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_leave_type_by_id_async

> <LeaveTypeDtoEnvelope> get_leave_type_by_id_async(tenant_id, leave_type_id, opts)

Get leave type by ID

Retrieves a specific leave type by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LeaveTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
leave_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get leave type by ID
  result = api_instance.get_leave_type_by_id_async(tenant_id, leave_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveTypesApi->get_leave_type_by_id_async: #{e}"
end
```

#### Using the get_leave_type_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LeaveTypeDtoEnvelope>, Integer, Hash)> get_leave_type_by_id_async_with_http_info(tenant_id, leave_type_id, opts)

```ruby
begin
  # Get leave type by ID
  data, status_code, headers = api_instance.get_leave_type_by_id_async_with_http_info(tenant_id, leave_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LeaveTypeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveTypesApi->get_leave_type_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **leave_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**LeaveTypeDtoEnvelope**](LeaveTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_leave_types_async

> <LeaveTypeDtoListEnvelope> get_leave_types_async(tenant_id, opts)

Get leave types

Retrieves leave types for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LeaveTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get leave types
  result = api_instance.get_leave_types_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveTypesApi->get_leave_types_async: #{e}"
end
```

#### Using the get_leave_types_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LeaveTypeDtoListEnvelope>, Integer, Hash)> get_leave_types_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get leave types
  data, status_code, headers = api_instance.get_leave_types_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LeaveTypeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveTypesApi->get_leave_types_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**LeaveTypeDtoListEnvelope**](LeaveTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_leave_types_count_async

> <Int32Envelope> get_leave_types_count_async(tenant_id, opts)

Count leave types

Counts leave types for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LeaveTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count leave types
  result = api_instance.get_leave_types_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveTypesApi->get_leave_types_count_async: #{e}"
end
```

#### Using the get_leave_types_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_leave_types_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count leave types
  data, status_code, headers = api_instance.get_leave_types_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveTypesApi->get_leave_types_count_async_with_http_info: #{e}"
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


## update_leave_type_async

> <EmptyEnvelope> update_leave_type_async(tenant_id, leave_type_id, opts)

Update a leave type

Updates an existing leave type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LeaveTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
leave_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  leave_type_update_dto: OpenapiClient::LeaveTypeUpdateDto.new # LeaveTypeUpdateDto | 
}

begin
  # Update a leave type
  result = api_instance.update_leave_type_async(tenant_id, leave_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveTypesApi->update_leave_type_async: #{e}"
end
```

#### Using the update_leave_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_leave_type_async_with_http_info(tenant_id, leave_type_id, opts)

```ruby
begin
  # Update a leave type
  data, status_code, headers = api_instance.update_leave_type_async_with_http_info(tenant_id, leave_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LeaveTypesApi->update_leave_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **leave_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **leave_type_update_dto** | [**LeaveTypeUpdateDto**](LeaveTypeUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

