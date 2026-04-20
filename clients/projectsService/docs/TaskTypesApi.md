# OpenapiClient::TaskTypesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_task_type_async**](TaskTypesApi.md#create_task_type_async) | **POST** /api/v2/ProjectsService/TaskTypes | Creates a new task type |
| [**delete_task_type_async**](TaskTypesApi.md#delete_task_type_async) | **DELETE** /api/v2/ProjectsService/TaskTypes/{taskTypeId} | Deletes a task type |
| [**get_task_type_by_id_async**](TaskTypesApi.md#get_task_type_by_id_async) | **GET** /api/v2/ProjectsService/TaskTypes/{taskTypeId} | Gets a task type by ID |
| [**update_task_type_async**](TaskTypesApi.md#update_task_type_async) | **PUT** /api/v2/ProjectsService/TaskTypes/{taskTypeId} | Updates a task type |


## create_task_type_async

> <TaskTypeDto> create_task_type_async(tenant_id, opts)

Creates a new task type

Creates a new task type for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaskTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  task_type_create_dto: OpenapiClient::TaskTypeCreateDto.new # TaskTypeCreateDto | 
}

begin
  # Creates a new task type
  result = api_instance.create_task_type_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskTypesApi->create_task_type_async: #{e}"
end
```

#### Using the create_task_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TaskTypeDto>, Integer, Hash)> create_task_type_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new task type
  data, status_code, headers = api_instance.create_task_type_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TaskTypeDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskTypesApi->create_task_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **task_type_create_dto** | [**TaskTypeCreateDto**](TaskTypeCreateDto.md) |  | [optional] |

### Return type

[**TaskTypeDto**](TaskTypeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_task_type_async

> <TaskTypeDto> delete_task_type_async(task_type_id, tenant_id)

Deletes a task type

Deletes the specified task type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaskTypesApi.new
task_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes a task type
  result = api_instance.delete_task_type_async(task_type_id, tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskTypesApi->delete_task_type_async: #{e}"
end
```

#### Using the delete_task_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TaskTypeDto>, Integer, Hash)> delete_task_type_async_with_http_info(task_type_id, tenant_id)

```ruby
begin
  # Deletes a task type
  data, status_code, headers = api_instance.delete_task_type_async_with_http_info(task_type_id, tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TaskTypeDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskTypesApi->delete_task_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **task_type_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |

### Return type

[**TaskTypeDto**](TaskTypeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_task_type_by_id_async

> <TaskTypeDto> get_task_type_by_id_async(task_type_id, tenant_id)

Gets a task type by ID

Retrieves the details of a task type using its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaskTypesApi.new
task_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a task type by ID
  result = api_instance.get_task_type_by_id_async(task_type_id, tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskTypesApi->get_task_type_by_id_async: #{e}"
end
```

#### Using the get_task_type_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TaskTypeDto>, Integer, Hash)> get_task_type_by_id_async_with_http_info(task_type_id, tenant_id)

```ruby
begin
  # Gets a task type by ID
  data, status_code, headers = api_instance.get_task_type_by_id_async_with_http_info(task_type_id, tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TaskTypeDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskTypesApi->get_task_type_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **task_type_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |

### Return type

[**TaskTypeDto**](TaskTypeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_task_type_async

> <TaskTypeDto> update_task_type_async(task_type_id, tenant_id, opts)

Updates a task type

Updates the specified task type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaskTypesApi.new
task_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  task_type_update_dto: OpenapiClient::TaskTypeUpdateDto.new # TaskTypeUpdateDto | 
}

begin
  # Updates a task type
  result = api_instance.update_task_type_async(task_type_id, tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskTypesApi->update_task_type_async: #{e}"
end
```

#### Using the update_task_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TaskTypeDto>, Integer, Hash)> update_task_type_async_with_http_info(task_type_id, tenant_id, opts)

```ruby
begin
  # Updates a task type
  data, status_code, headers = api_instance.update_task_type_async_with_http_info(task_type_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TaskTypeDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskTypesApi->update_task_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **task_type_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **task_type_update_dto** | [**TaskTypeUpdateDto**](TaskTypeUpdateDto.md) |  | [optional] |

### Return type

[**TaskTypeDto**](TaskTypeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

