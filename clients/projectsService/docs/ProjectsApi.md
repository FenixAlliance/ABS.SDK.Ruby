# OpenapiClient::ProjectsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_project_async**](ProjectsApi.md#create_project_async) | **POST** /api/v2/ProjectsService/Projects | Creates a new project |
| [**create_project_period_async**](ProjectsApi.md#create_project_period_async) | **POST** /api/v2/ProjectsService/Projects/{projectId}/Periods | Creates a project period |
| [**create_project_task_async**](ProjectsApi.md#create_project_task_async) | **POST** /api/v2/ProjectsService/Projects/{projectId}/Tasks | Creates a project task |
| [**delete_project_async**](ProjectsApi.md#delete_project_async) | **DELETE** /api/v2/ProjectsService/Projects/{projectId} | Deletes a project |
| [**delete_project_period_async**](ProjectsApi.md#delete_project_period_async) | **DELETE** /api/v2/ProjectsService/Projects/{projectId}/Periods/{projectPeriodId} | Deletes a project period |
| [**delete_project_task_async**](ProjectsApi.md#delete_project_task_async) | **DELETE** /api/v2/ProjectsService/Projects/{projectId}/Tasks/{projectTaskId} | Deletes a project task |
| [**get_project_by_id_async**](ProjectsApi.md#get_project_by_id_async) | **GET** /api/v2/ProjectsService/Projects/{projectId} | Gets a project by ID |
| [**get_project_periods_async**](ProjectsApi.md#get_project_periods_async) | **GET** /api/v2/ProjectsService/Projects/{projectId}/Periods | Retrieves project periods |
| [**get_project_task_categories_async**](ProjectsApi.md#get_project_task_categories_async) | **GET** /api/v2/ProjectsService/Projects/{projectId}/TaskCategories | Retrieves project task categories |
| [**get_project_task_categories_count_async**](ProjectsApi.md#get_project_task_categories_count_async) | **GET** /api/v2/ProjectsService/Projects/{projectId}/TaskCategories/Count | Counts project task categories |
| [**get_project_tasks_async**](ProjectsApi.md#get_project_tasks_async) | **GET** /api/v2/ProjectsService/Projects/{projectId}/Tasks | Retrieves project tasks |
| [**get_project_tasks_count_async**](ProjectsApi.md#get_project_tasks_count_async) | **GET** /api/v2/ProjectsService/Projects/{projectId}/Tasks/Count | Counts project tasks |
| [**get_project_time_logs_async**](ProjectsApi.md#get_project_time_logs_async) | **GET** /api/v2/ProjectsService/Projects/{projectId}/TimeLogs | Retrieves project time logs |
| [**get_project_time_logs_count_async**](ProjectsApi.md#get_project_time_logs_count_async) | **GET** /api/v2/ProjectsService/Projects/{projectId}/TimeLogs/Count | Counts project time logs |
| [**get_projects_by_tenant_id_async**](ProjectsApi.md#get_projects_by_tenant_id_async) | **GET** /api/v2/ProjectsService/Projects | Retrieves all projects |
| [**get_projects_count_by_tenant_id_async**](ProjectsApi.md#get_projects_count_by_tenant_id_async) | **GET** /api/v2/ProjectsService/Projects/Count | Counts projects |
| [**update_project_async**](ProjectsApi.md#update_project_async) | **PUT** /api/v2/ProjectsService/Projects/{projectId} | Updates a project |
| [**update_project_period_async**](ProjectsApi.md#update_project_period_async) | **PUT** /api/v2/ProjectsService/Projects/{projectId}/Periods/{projectPeriodId} | Updates a project period |
| [**update_project_task_async**](ProjectsApi.md#update_project_task_async) | **PUT** /api/v2/ProjectsService/Projects/{projectId}/Tasks/{projectTaskId} | Updates a project task |


## create_project_async

> <EmptyEnvelope> create_project_async(tenant_id, opts)

Creates a new project

Creates a new project for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  project_create_dto: OpenapiClient::ProjectCreateDto.new # ProjectCreateDto | 
}

begin
  # Creates a new project
  result = api_instance.create_project_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->create_project_async: #{e}"
end
```

#### Using the create_project_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_project_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new project
  data, status_code, headers = api_instance.create_project_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->create_project_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **project_create_dto** | [**ProjectCreateDto**](ProjectCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_project_period_async

> <EmptyEnvelope> create_project_period_async(project_id, tenant_id, opts)

Creates a project period

Creates a new period for the specified project.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectsApi.new
project_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  project_period_create_dto: OpenapiClient::ProjectPeriodCreateDto.new # ProjectPeriodCreateDto | 
}

begin
  # Creates a project period
  result = api_instance.create_project_period_async(project_id, tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->create_project_period_async: #{e}"
end
```

#### Using the create_project_period_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_project_period_async_with_http_info(project_id, tenant_id, opts)

```ruby
begin
  # Creates a project period
  data, status_code, headers = api_instance.create_project_period_async_with_http_info(project_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->create_project_period_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **project_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **project_period_create_dto** | [**ProjectPeriodCreateDto**](ProjectPeriodCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_project_task_async

> <EmptyEnvelope> create_project_task_async(project_id, tenant_id, opts)

Creates a project task

Creates a new task for the specified project.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectsApi.new
project_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  project_task_create_dto: OpenapiClient::ProjectTaskCreateDto.new # ProjectTaskCreateDto | 
}

begin
  # Creates a project task
  result = api_instance.create_project_task_async(project_id, tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->create_project_task_async: #{e}"
end
```

#### Using the create_project_task_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_project_task_async_with_http_info(project_id, tenant_id, opts)

```ruby
begin
  # Creates a project task
  data, status_code, headers = api_instance.create_project_task_async_with_http_info(project_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->create_project_task_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **project_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **project_task_create_dto** | [**ProjectTaskCreateDto**](ProjectTaskCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_project_async

> <EmptyEnvelope> delete_project_async(project_id, tenant_id)

Deletes a project

Deletes the specified project.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectsApi.new
project_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes a project
  result = api_instance.delete_project_async(project_id, tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->delete_project_async: #{e}"
end
```

#### Using the delete_project_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_project_async_with_http_info(project_id, tenant_id)

```ruby
begin
  # Deletes a project
  data, status_code, headers = api_instance.delete_project_async_with_http_info(project_id, tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->delete_project_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **project_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_project_period_async

> <EmptyEnvelope> delete_project_period_async(project_id, project_period_id, tenant_id)

Deletes a project period

Deletes the specified period from a project.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectsApi.new
project_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
project_period_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes a project period
  result = api_instance.delete_project_period_async(project_id, project_period_id, tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->delete_project_period_async: #{e}"
end
```

#### Using the delete_project_period_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_project_period_async_with_http_info(project_id, project_period_id, tenant_id)

```ruby
begin
  # Deletes a project period
  data, status_code, headers = api_instance.delete_project_period_async_with_http_info(project_id, project_period_id, tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->delete_project_period_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **project_id** | **String** |  |  |
| **project_period_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_project_task_async

> <EmptyEnvelope> delete_project_task_async(tenant_id, project_id, project_task_id)

Deletes a project task

Deletes the specified task from a project.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
project_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
project_task_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes a project task
  result = api_instance.delete_project_task_async(tenant_id, project_id, project_task_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->delete_project_task_async: #{e}"
end
```

#### Using the delete_project_task_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_project_task_async_with_http_info(tenant_id, project_id, project_task_id)

```ruby
begin
  # Deletes a project task
  data, status_code, headers = api_instance.delete_project_task_async_with_http_info(tenant_id, project_id, project_task_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->delete_project_task_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **project_id** | **String** |  |  |
| **project_task_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_project_by_id_async

> <ProjectDtoEnvelope> get_project_by_id_async(project_id, tenant_id)

Gets a project by ID

Retrieves the details of a project using its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectsApi.new
project_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a project by ID
  result = api_instance.get_project_by_id_async(project_id, tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_project_by_id_async: #{e}"
end
```

#### Using the get_project_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ProjectDtoEnvelope>, Integer, Hash)> get_project_by_id_async_with_http_info(project_id, tenant_id)

```ruby
begin
  # Gets a project by ID
  data, status_code, headers = api_instance.get_project_by_id_async_with_http_info(project_id, tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ProjectDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_project_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **project_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |

### Return type

[**ProjectDtoEnvelope**](ProjectDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_project_periods_async

> <ProjectPeriodDtoListEnvelope> get_project_periods_async(project_id, tenant_id)

Retrieves project periods

Gets all periods for a specific project.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectsApi.new
project_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Retrieves project periods
  result = api_instance.get_project_periods_async(project_id, tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_project_periods_async: #{e}"
end
```

#### Using the get_project_periods_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ProjectPeriodDtoListEnvelope>, Integer, Hash)> get_project_periods_async_with_http_info(project_id, tenant_id)

```ruby
begin
  # Retrieves project periods
  data, status_code, headers = api_instance.get_project_periods_async_with_http_info(project_id, tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ProjectPeriodDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_project_periods_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **project_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |

### Return type

[**ProjectPeriodDtoListEnvelope**](ProjectPeriodDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_project_task_categories_async

> <TaskCategoryDtoListEnvelope> get_project_task_categories_async(project_id, tenant_id)

Retrieves project task categories

Gets all task categories for a specific project with OData support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectsApi.new
project_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Retrieves project task categories
  result = api_instance.get_project_task_categories_async(project_id, tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_project_task_categories_async: #{e}"
end
```

#### Using the get_project_task_categories_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TaskCategoryDtoListEnvelope>, Integer, Hash)> get_project_task_categories_async_with_http_info(project_id, tenant_id)

```ruby
begin
  # Retrieves project task categories
  data, status_code, headers = api_instance.get_project_task_categories_async_with_http_info(project_id, tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TaskCategoryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_project_task_categories_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **project_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |

### Return type

[**TaskCategoryDtoListEnvelope**](TaskCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_project_task_categories_count_async

> <Int32Envelope> get_project_task_categories_count_async(project_id, tenant_id)

Counts project task categories

Gets the count of task categories for a specific project.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectsApi.new
project_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Counts project task categories
  result = api_instance.get_project_task_categories_count_async(project_id, tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_project_task_categories_count_async: #{e}"
end
```

#### Using the get_project_task_categories_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_project_task_categories_count_async_with_http_info(project_id, tenant_id)

```ruby
begin
  # Counts project task categories
  data, status_code, headers = api_instance.get_project_task_categories_count_async_with_http_info(project_id, tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_project_task_categories_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **project_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_project_tasks_async

> <ProjectTaskDtoListEnvelope> get_project_tasks_async(project_id, tenant_id)

Retrieves project tasks

Gets all tasks for a specific project with OData support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectsApi.new
project_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Retrieves project tasks
  result = api_instance.get_project_tasks_async(project_id, tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_project_tasks_async: #{e}"
end
```

#### Using the get_project_tasks_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ProjectTaskDtoListEnvelope>, Integer, Hash)> get_project_tasks_async_with_http_info(project_id, tenant_id)

```ruby
begin
  # Retrieves project tasks
  data, status_code, headers = api_instance.get_project_tasks_async_with_http_info(project_id, tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ProjectTaskDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_project_tasks_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **project_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |

### Return type

[**ProjectTaskDtoListEnvelope**](ProjectTaskDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_project_tasks_count_async

> <Int32Envelope> get_project_tasks_count_async(project_id, tenant_id)

Counts project tasks

Gets the count of tasks for a specific project.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectsApi.new
project_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Counts project tasks
  result = api_instance.get_project_tasks_count_async(project_id, tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_project_tasks_count_async: #{e}"
end
```

#### Using the get_project_tasks_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_project_tasks_count_async_with_http_info(project_id, tenant_id)

```ruby
begin
  # Counts project tasks
  data, status_code, headers = api_instance.get_project_tasks_count_async_with_http_info(project_id, tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_project_tasks_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **project_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_project_time_logs_async

> <ProjectTimeLogDtoListEnvelope> get_project_time_logs_async(project_id, tenant_id)

Retrieves project time logs

Gets all time log entries for a specific project with OData support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectsApi.new
project_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Retrieves project time logs
  result = api_instance.get_project_time_logs_async(project_id, tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_project_time_logs_async: #{e}"
end
```

#### Using the get_project_time_logs_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ProjectTimeLogDtoListEnvelope>, Integer, Hash)> get_project_time_logs_async_with_http_info(project_id, tenant_id)

```ruby
begin
  # Retrieves project time logs
  data, status_code, headers = api_instance.get_project_time_logs_async_with_http_info(project_id, tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ProjectTimeLogDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_project_time_logs_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **project_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |

### Return type

[**ProjectTimeLogDtoListEnvelope**](ProjectTimeLogDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_project_time_logs_count_async

> <Int32Envelope> get_project_time_logs_count_async(project_id, tenant_id)

Counts project time logs

Gets the count of time log entries for a specific project.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectsApi.new
project_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Counts project time logs
  result = api_instance.get_project_time_logs_count_async(project_id, tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_project_time_logs_count_async: #{e}"
end
```

#### Using the get_project_time_logs_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_project_time_logs_count_async_with_http_info(project_id, tenant_id)

```ruby
begin
  # Counts project time logs
  data, status_code, headers = api_instance.get_project_time_logs_count_async_with_http_info(project_id, tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_project_time_logs_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **project_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_projects_by_tenant_id_async

> <ProjectDtoListEnvelope> get_projects_by_tenant_id_async(tenant_id)

Retrieves all projects

Gets all projects for the current tenant with OData support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Retrieves all projects
  result = api_instance.get_projects_by_tenant_id_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_projects_by_tenant_id_async: #{e}"
end
```

#### Using the get_projects_by_tenant_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ProjectDtoListEnvelope>, Integer, Hash)> get_projects_by_tenant_id_async_with_http_info(tenant_id)

```ruby
begin
  # Retrieves all projects
  data, status_code, headers = api_instance.get_projects_by_tenant_id_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ProjectDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_projects_by_tenant_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**ProjectDtoListEnvelope**](ProjectDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_projects_count_by_tenant_id_async

> <Int32Envelope> get_projects_count_by_tenant_id_async(tenant_id)

Counts projects

Gets the count of projects for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Counts projects
  result = api_instance.get_projects_count_by_tenant_id_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_projects_count_by_tenant_id_async: #{e}"
end
```

#### Using the get_projects_count_by_tenant_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_projects_count_by_tenant_id_async_with_http_info(tenant_id)

```ruby
begin
  # Counts projects
  data, status_code, headers = api_instance.get_projects_count_by_tenant_id_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->get_projects_count_by_tenant_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_project_async

> <EmptyEnvelope> update_project_async(project_id, tenant_id, opts)

Updates a project

Updates the specified project.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectsApi.new
project_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  project_update_dto: OpenapiClient::ProjectUpdateDto.new # ProjectUpdateDto | 
}

begin
  # Updates a project
  result = api_instance.update_project_async(project_id, tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->update_project_async: #{e}"
end
```

#### Using the update_project_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_project_async_with_http_info(project_id, tenant_id, opts)

```ruby
begin
  # Updates a project
  data, status_code, headers = api_instance.update_project_async_with_http_info(project_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->update_project_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **project_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **project_update_dto** | [**ProjectUpdateDto**](ProjectUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_project_period_async

> <EmptyEnvelope> update_project_period_async(project_id, project_period_id, tenant_id, opts)

Updates a project period

Updates the specified period for a project.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectsApi.new
project_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
project_period_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  project_period_update_dto: OpenapiClient::ProjectPeriodUpdateDto.new # ProjectPeriodUpdateDto | 
}

begin
  # Updates a project period
  result = api_instance.update_project_period_async(project_id, project_period_id, tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->update_project_period_async: #{e}"
end
```

#### Using the update_project_period_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_project_period_async_with_http_info(project_id, project_period_id, tenant_id, opts)

```ruby
begin
  # Updates a project period
  data, status_code, headers = api_instance.update_project_period_async_with_http_info(project_id, project_period_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->update_project_period_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **project_id** | **String** |  |  |
| **project_period_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **project_period_update_dto** | [**ProjectPeriodUpdateDto**](ProjectPeriodUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_project_task_async

> <EmptyEnvelope> update_project_task_async(project_id, project_task_id, tenant_id, opts)

Updates a project task

Updates the specified task in a project.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProjectsApi.new
project_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
project_task_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  project_task_update_dto: OpenapiClient::ProjectTaskUpdateDto.new # ProjectTaskUpdateDto | 
}

begin
  # Updates a project task
  result = api_instance.update_project_task_async(project_id, project_task_id, tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->update_project_task_async: #{e}"
end
```

#### Using the update_project_task_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_project_task_async_with_http_info(project_id, project_task_id, tenant_id, opts)

```ruby
begin
  # Updates a project task
  data, status_code, headers = api_instance.update_project_task_async_with_http_info(project_id, project_task_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProjectsApi->update_project_task_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **project_id** | **String** |  |  |
| **project_task_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **project_task_update_dto** | [**ProjectTaskUpdateDto**](ProjectTaskUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

