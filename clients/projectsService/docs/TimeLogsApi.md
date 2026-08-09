# OpenapiClient::TimeLogsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_project_period_time_logs_async**](TimeLogsApi.md#count_project_period_time_logs_async) | **GET** /api/v2/ProjectsService/TimeLogs/Count | Get the count of project period time logs |
| [**create_project_time_log_async**](TimeLogsApi.md#create_project_time_log_async) | **POST** /api/v2/ProjectsService/TimeLogs | Create a new project time log |
| [**delete_project_time_log_async**](TimeLogsApi.md#delete_project_time_log_async) | **DELETE** /api/v2/ProjectsService/TimeLogs/{timeLogId} | Delete a project time log |
| [**get_project_period_time_logs_async**](TimeLogsApi.md#get_project_period_time_logs_async) | **GET** /api/v2/ProjectsService/TimeLogs | Retrieve project period time logs |
| [**get_project_time_log_by_id_async**](TimeLogsApi.md#get_project_time_log_by_id_async) | **GET** /api/v2/ProjectsService/TimeLogs/{timeLogId} | Retrieve a project time log by ID |
| [**get_project_time_logs_async**](TimeLogsApi.md#get_project_time_logs_async) | **GET** /api/v2/ProjectsService/TimeLogs/ForProject/{projectId} | Retrieve time logs for a project |
| [**get_project_time_logs_by_responsible_contact_async**](TimeLogsApi.md#get_project_time_logs_by_responsible_contact_async) | **GET** /api/v2/ProjectsService/TimeLogs/ByResponsibleContact | Retrieve time logs by responsible contact |
| [**get_project_time_logs_created_by_contact_async**](TimeLogsApi.md#get_project_time_logs_created_by_contact_async) | **GET** /api/v2/ProjectsService/TimeLogs/CreatedByContact | Retrieve time logs created by a contact |
| [**patch_project_time_log_async**](TimeLogsApi.md#patch_project_time_log_async) | **PATCH** /api/v2/ProjectsService/TimeLogs/{timeLogId} | Patch a project time log |
| [**update_project_time_log_async**](TimeLogsApi.md#update_project_time_log_async) | **PUT** /api/v2/ProjectsService/TimeLogs/{timeLogId} | Update a project time log |


## count_project_period_time_logs_async

> <Int32Envelope> count_project_period_time_logs_async(tenant_id, project_period_id, opts)

Get the count of project period time logs

Returns the total count of time logs for a specific project period with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeLogsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
project_period_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  project_time_log_dto_collection_query_parameters: OpenapiClient::ProjectTimeLogDtoCollectionQueryParameters.new # ProjectTimeLogDtoCollectionQueryParameters | 
}

begin
  # Get the count of project period time logs
  result = api_instance.count_project_period_time_logs_async(tenant_id, project_period_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->count_project_period_time_logs_async: #{e}"
end
```

#### Using the count_project_period_time_logs_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_project_period_time_logs_async_with_http_info(tenant_id, project_period_id, opts)

```ruby
begin
  # Get the count of project period time logs
  data, status_code, headers = api_instance.count_project_period_time_logs_async_with_http_info(tenant_id, project_period_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->count_project_period_time_logs_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **project_period_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **project_time_log_dto_collection_query_parameters** | [**ProjectTimeLogDtoCollectionQueryParameters**](ProjectTimeLogDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_project_time_log_async

> create_project_time_log_async(tenant_id, opts)

Create a new project time log

Creates a new project time log entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeLogsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  project_time_log_create_dto: OpenapiClient::ProjectTimeLogCreateDto.new({project_task_id: 'project_task_id_example', project_period_id: 'project_period_id_example'}) # ProjectTimeLogCreateDto | 
}

begin
  # Create a new project time log
  api_instance.create_project_time_log_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->create_project_time_log_async: #{e}"
end
```

#### Using the create_project_time_log_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_project_time_log_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new project time log
  data, status_code, headers = api_instance.create_project_time_log_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->create_project_time_log_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **project_time_log_create_dto** | [**ProjectTimeLogCreateDto**](ProjectTimeLogCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_project_time_log_async

> delete_project_time_log_async(tenant_id, time_log_id, opts)

Delete a project time log

Deletes a project time log entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeLogsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
time_log_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a project time log
  api_instance.delete_project_time_log_async(tenant_id, time_log_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->delete_project_time_log_async: #{e}"
end
```

#### Using the delete_project_time_log_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_project_time_log_async_with_http_info(tenant_id, time_log_id, opts)

```ruby
begin
  # Delete a project time log
  data, status_code, headers = api_instance.delete_project_time_log_async_with_http_info(tenant_id, time_log_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->delete_project_time_log_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **time_log_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_project_period_time_logs_async

> <ProjectTimeLogDtoListEnvelope> get_project_period_time_logs_async(tenant_id, project_period_id, opts)

Retrieve project period time logs

Retrieves a list of time logs for a specific project period with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeLogsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
project_period_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  project_time_log_dto_collection_query_parameters: OpenapiClient::ProjectTimeLogDtoCollectionQueryParameters.new # ProjectTimeLogDtoCollectionQueryParameters | 
}

begin
  # Retrieve project period time logs
  result = api_instance.get_project_period_time_logs_async(tenant_id, project_period_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->get_project_period_time_logs_async: #{e}"
end
```

#### Using the get_project_period_time_logs_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ProjectTimeLogDtoListEnvelope>, Integer, Hash)> get_project_period_time_logs_async_with_http_info(tenant_id, project_period_id, opts)

```ruby
begin
  # Retrieve project period time logs
  data, status_code, headers = api_instance.get_project_period_time_logs_async_with_http_info(tenant_id, project_period_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ProjectTimeLogDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->get_project_period_time_logs_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **project_period_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **project_time_log_dto_collection_query_parameters** | [**ProjectTimeLogDtoCollectionQueryParameters**](ProjectTimeLogDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ProjectTimeLogDtoListEnvelope**](ProjectTimeLogDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_project_time_log_by_id_async

> <ProjectTimeLogDtoEnvelope> get_project_time_log_by_id_async(time_log_id, tenant_id, opts)

Retrieve a project time log by ID

Retrieves a single project time log by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeLogsApi.new
time_log_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a project time log by ID
  result = api_instance.get_project_time_log_by_id_async(time_log_id, tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->get_project_time_log_by_id_async: #{e}"
end
```

#### Using the get_project_time_log_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ProjectTimeLogDtoEnvelope>, Integer, Hash)> get_project_time_log_by_id_async_with_http_info(time_log_id, tenant_id, opts)

```ruby
begin
  # Retrieve a project time log by ID
  data, status_code, headers = api_instance.get_project_time_log_by_id_async_with_http_info(time_log_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ProjectTimeLogDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->get_project_time_log_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **time_log_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ProjectTimeLogDtoEnvelope**](ProjectTimeLogDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_project_time_logs_async

> <ProjectTimeLogDtoListEnvelope> get_project_time_logs_async(project_id, tenant_id, opts)

Retrieve time logs for a project

Retrieves all time logs associated with the specified project.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeLogsApi.new
project_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve time logs for a project
  result = api_instance.get_project_time_logs_async(project_id, tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->get_project_time_logs_async: #{e}"
end
```

#### Using the get_project_time_logs_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ProjectTimeLogDtoListEnvelope>, Integer, Hash)> get_project_time_logs_async_with_http_info(project_id, tenant_id, opts)

```ruby
begin
  # Retrieve time logs for a project
  data, status_code, headers = api_instance.get_project_time_logs_async_with_http_info(project_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ProjectTimeLogDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->get_project_time_logs_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **project_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ProjectTimeLogDtoListEnvelope**](ProjectTimeLogDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_project_time_logs_by_responsible_contact_async

> <ProjectTimeLogDtoListEnvelope> get_project_time_logs_by_responsible_contact_async(contact_id, tenant_id, opts)

Retrieve time logs by responsible contact

Retrieves time logs where the specified contact is the responsible party.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeLogsApi.new
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve time logs by responsible contact
  result = api_instance.get_project_time_logs_by_responsible_contact_async(contact_id, tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->get_project_time_logs_by_responsible_contact_async: #{e}"
end
```

#### Using the get_project_time_logs_by_responsible_contact_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ProjectTimeLogDtoListEnvelope>, Integer, Hash)> get_project_time_logs_by_responsible_contact_async_with_http_info(contact_id, tenant_id, opts)

```ruby
begin
  # Retrieve time logs by responsible contact
  data, status_code, headers = api_instance.get_project_time_logs_by_responsible_contact_async_with_http_info(contact_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ProjectTimeLogDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->get_project_time_logs_by_responsible_contact_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **contact_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ProjectTimeLogDtoListEnvelope**](ProjectTimeLogDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_project_time_logs_created_by_contact_async

> <ProjectTimeLogDtoListEnvelope> get_project_time_logs_created_by_contact_async(contact_id, tenant_id, opts)

Retrieve time logs created by a contact

Retrieves time logs that were created by the specified contact.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeLogsApi.new
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve time logs created by a contact
  result = api_instance.get_project_time_logs_created_by_contact_async(contact_id, tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->get_project_time_logs_created_by_contact_async: #{e}"
end
```

#### Using the get_project_time_logs_created_by_contact_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ProjectTimeLogDtoListEnvelope>, Integer, Hash)> get_project_time_logs_created_by_contact_async_with_http_info(contact_id, tenant_id, opts)

```ruby
begin
  # Retrieve time logs created by a contact
  data, status_code, headers = api_instance.get_project_time_logs_created_by_contact_async_with_http_info(contact_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ProjectTimeLogDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->get_project_time_logs_created_by_contact_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **contact_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ProjectTimeLogDtoListEnvelope**](ProjectTimeLogDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_project_time_log_async

> patch_project_time_log_async(time_log_id, tenant_id, opts)

Patch a project time log

Partially updates an existing project time log entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeLogsApi.new
time_log_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a project time log
  api_instance.patch_project_time_log_async(time_log_id, tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->patch_project_time_log_async: #{e}"
end
```

#### Using the patch_project_time_log_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> patch_project_time_log_async_with_http_info(time_log_id, tenant_id, opts)

```ruby
begin
  # Patch a project time log
  data, status_code, headers = api_instance.patch_project_time_log_async_with_http_info(time_log_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->patch_project_time_log_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **time_log_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_project_time_log_async

> update_project_time_log_async(time_log_id, tenant_id, opts)

Update a project time log

Updates an existing project time log entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeLogsApi.new
time_log_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  project_time_log_update_dto: OpenapiClient::ProjectTimeLogUpdateDto.new # ProjectTimeLogUpdateDto | 
}

begin
  # Update a project time log
  api_instance.update_project_time_log_async(time_log_id, tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->update_project_time_log_async: #{e}"
end
```

#### Using the update_project_time_log_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_project_time_log_async_with_http_info(time_log_id, tenant_id, opts)

```ruby
begin
  # Update a project time log
  data, status_code, headers = api_instance.update_project_time_log_async_with_http_info(time_log_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogsApi->update_project_time_log_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **time_log_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **project_time_log_update_dto** | [**ProjectTimeLogUpdateDto**](ProjectTimeLogUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

