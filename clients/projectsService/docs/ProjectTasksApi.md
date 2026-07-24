# OpenapiClient::ProjectTasksApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_project_task_async**](ProjectTasksApi.md#create_project_task_async) | **POST** /api/v2/ProjectsService/ProjectTasks | Create a project task |
| [**delete_project_task_async**](ProjectTasksApi.md#delete_project_task_async) | **DELETE** /api/v2/ProjectsService/ProjectTasks/{projectTaskId} | Delete a project task |
| [**get_project_task_by_id_async**](ProjectTasksApi.md#get_project_task_by_id_async) | **GET** /api/v2/ProjectsService/ProjectTasks/{projectTaskId} | Get project task by ID |
| [**get_project_tasks_async**](ProjectTasksApi.md#get_project_tasks_async) | **GET** /api/v2/ProjectsService/ProjectTasks | Get all project tasks |
| [**get_project_tasks_count_async**](ProjectTasksApi.md#get_project_tasks_count_async) | **GET** /api/v2/ProjectsService/ProjectTasks/Count | Get project tasks count |
| [**patch_project_task_async**](ProjectTasksApi.md#patch_project_task_async) | **PATCH** /api/v2/ProjectsService/ProjectTasks/{projectTaskId} | Patch a project task |
| [**update_project_task_async**](ProjectTasksApi.md#update_project_task_async) | **PUT** /api/v2/ProjectsService/ProjectTasks/{projectTaskId} | Update a project task |


## create_project_task_async

> <EmptyEnvelope> create_project_task_async(tenant_id, opts)

Create a project task

Creates a new project task.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectTasksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  project_task_create_dto: OpenapiClient::ProjectTaskCreateDto.new # ProjectTaskCreateDto | 
}

begin
  # Create a project task
  result = api_instance.create_project_task_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectTasksApi->create_project_task_async: #{e}"
end
```

#### Using the create_project_task_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_project_task_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a project task
  data, status_code, headers = api_instance.create_project_task_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectTasksApi->create_project_task_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **project_task_create_dto** | [**ProjectTaskCreateDto**](ProjectTaskCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_project_task_async

> <EmptyEnvelope> delete_project_task_async(tenant_id, project_task_id, opts)

Delete a project task

Deletes a project task.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectTasksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
project_task_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a project task
  result = api_instance.delete_project_task_async(tenant_id, project_task_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectTasksApi->delete_project_task_async: #{e}"
end
```

#### Using the delete_project_task_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_project_task_async_with_http_info(tenant_id, project_task_id, opts)

```ruby
begin
  # Delete a project task
  data, status_code, headers = api_instance.delete_project_task_async_with_http_info(tenant_id, project_task_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectTasksApi->delete_project_task_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **project_task_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_project_task_by_id_async

> <ProjectTaskDtoEnvelope> get_project_task_by_id_async(tenant_id, project_task_id, opts)

Get project task by ID

Retrieves a specific project task.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectTasksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
project_task_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get project task by ID
  result = api_instance.get_project_task_by_id_async(tenant_id, project_task_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectTasksApi->get_project_task_by_id_async: #{e}"
end
```

#### Using the get_project_task_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ProjectTaskDtoEnvelope>, Integer, Hash)> get_project_task_by_id_async_with_http_info(tenant_id, project_task_id, opts)

```ruby
begin
  # Get project task by ID
  data, status_code, headers = api_instance.get_project_task_by_id_async_with_http_info(tenant_id, project_task_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ProjectTaskDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectTasksApi->get_project_task_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **project_task_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ProjectTaskDtoEnvelope**](ProjectTaskDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_project_tasks_async

> <ProjectTaskDtoListEnvelope> get_project_tasks_async(tenant_id, opts)

Get all project tasks

Retrieves all project tasks for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectTasksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all project tasks
  result = api_instance.get_project_tasks_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectTasksApi->get_project_tasks_async: #{e}"
end
```

#### Using the get_project_tasks_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ProjectTaskDtoListEnvelope>, Integer, Hash)> get_project_tasks_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all project tasks
  data, status_code, headers = api_instance.get_project_tasks_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ProjectTaskDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectTasksApi->get_project_tasks_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ProjectTaskDtoListEnvelope**](ProjectTaskDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_project_tasks_count_async

> <Int32Envelope> get_project_tasks_count_async(tenant_id, opts)

Get project tasks count

Returns the count of project tasks for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectTasksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get project tasks count
  result = api_instance.get_project_tasks_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectTasksApi->get_project_tasks_count_async: #{e}"
end
```

#### Using the get_project_tasks_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_project_tasks_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get project tasks count
  data, status_code, headers = api_instance.get_project_tasks_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectTasksApi->get_project_tasks_count_async_with_http_info: #{e}"
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


## patch_project_task_async

> <EmptyEnvelope> patch_project_task_async(tenant_id, project_task_id, opts)

Patch a project task

Partially updates an existing project task.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectTasksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
project_task_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a project task
  result = api_instance.patch_project_task_async(tenant_id, project_task_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectTasksApi->patch_project_task_async: #{e}"
end
```

#### Using the patch_project_task_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_project_task_async_with_http_info(tenant_id, project_task_id, opts)

```ruby
begin
  # Patch a project task
  data, status_code, headers = api_instance.patch_project_task_async_with_http_info(tenant_id, project_task_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectTasksApi->patch_project_task_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **project_task_id** | **String** |  |  |
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


## update_project_task_async

> <EmptyEnvelope> update_project_task_async(tenant_id, project_task_id, opts)

Update a project task

Updates an existing project task.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectTasksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
project_task_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  project_task_update_dto: OpenapiClient::ProjectTaskUpdateDto.new # ProjectTaskUpdateDto | 
}

begin
  # Update a project task
  result = api_instance.update_project_task_async(tenant_id, project_task_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectTasksApi->update_project_task_async: #{e}"
end
```

#### Using the update_project_task_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_project_task_async_with_http_info(tenant_id, project_task_id, opts)

```ruby
begin
  # Update a project task
  data, status_code, headers = api_instance.update_project_task_async_with_http_info(tenant_id, project_task_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectTasksApi->update_project_task_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **project_task_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **project_task_update_dto** | [**ProjectTaskUpdateDto**](ProjectTaskUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

