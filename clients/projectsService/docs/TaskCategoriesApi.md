# OpenapiClient::TaskCategoriesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_tenant_task_categories_async**](TaskCategoriesApi.md#count_tenant_task_categories_async) | **GET** /api/v2/ProjectsService/TaskCategories/Count | Counts task categories |
| [**create_task_category_async**](TaskCategoriesApi.md#create_task_category_async) | **POST** /api/v2/ProjectsService/TaskCategories | Creates a new task category |
| [**delete_task_category_async**](TaskCategoriesApi.md#delete_task_category_async) | **DELETE** /api/v2/ProjectsService/TaskCategories/{taskCategoryId} | Deletes a task category |
| [**get_task_category_by_id_async**](TaskCategoriesApi.md#get_task_category_by_id_async) | **GET** /api/v2/ProjectsService/TaskCategories/{taskCategoryId} | Gets a task category by ID |
| [**get_task_category_task_types_async**](TaskCategoriesApi.md#get_task_category_task_types_async) | **GET** /api/v2/ProjectsService/TaskCategories/{taskCategoryId}/Types | Retrieves task types for a category |
| [**get_tenant_task_categories_async**](TaskCategoriesApi.md#get_tenant_task_categories_async) | **GET** /api/v2/ProjectsService/TaskCategories | Retrieves all task categories |
| [**patch_task_category_async**](TaskCategoriesApi.md#patch_task_category_async) | **PATCH** /api/v2/ProjectsService/TaskCategories/{taskCategoryId} | Patches a task category |
| [**update_task_category_async**](TaskCategoriesApi.md#update_task_category_async) | **PUT** /api/v2/ProjectsService/TaskCategories/{taskCategoryId} | Updates a task category |


## count_tenant_task_categories_async

> <Int32Envelope> count_tenant_task_categories_async(tenant_id, opts)

Counts task categories

Gets the count of task categories for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaskCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  task_category_dto_collection_query_parameters: OpenapiClient::TaskCategoryDtoCollectionQueryParameters.new # TaskCategoryDtoCollectionQueryParameters | 
}

begin
  # Counts task categories
  result = api_instance.count_tenant_task_categories_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskCategoriesApi->count_tenant_task_categories_async: #{e}"
end
```

#### Using the count_tenant_task_categories_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_tenant_task_categories_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Counts task categories
  data, status_code, headers = api_instance.count_tenant_task_categories_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskCategoriesApi->count_tenant_task_categories_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **task_category_dto_collection_query_parameters** | [**TaskCategoryDtoCollectionQueryParameters**](TaskCategoryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_task_category_async

> <TaskCategoryDto> create_task_category_async(tenant_id, opts)

Creates a new task category

Creates a new task category for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaskCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  task_category_create_dto: OpenapiClient::TaskCategoryCreateDto.new # TaskCategoryCreateDto | 
}

begin
  # Creates a new task category
  result = api_instance.create_task_category_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskCategoriesApi->create_task_category_async: #{e}"
end
```

#### Using the create_task_category_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TaskCategoryDto>, Integer, Hash)> create_task_category_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new task category
  data, status_code, headers = api_instance.create_task_category_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TaskCategoryDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskCategoriesApi->create_task_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **task_category_create_dto** | [**TaskCategoryCreateDto**](TaskCategoryCreateDto.md) |  | [optional] |

### Return type

[**TaskCategoryDto**](TaskCategoryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_task_category_async

> <TaskCategoryDto> delete_task_category_async(task_category_id, tenant_id)

Deletes a task category

Deletes the specified task category.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaskCategoriesApi.new
task_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes a task category
  result = api_instance.delete_task_category_async(task_category_id, tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskCategoriesApi->delete_task_category_async: #{e}"
end
```

#### Using the delete_task_category_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TaskCategoryDto>, Integer, Hash)> delete_task_category_async_with_http_info(task_category_id, tenant_id)

```ruby
begin
  # Deletes a task category
  data, status_code, headers = api_instance.delete_task_category_async_with_http_info(task_category_id, tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TaskCategoryDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskCategoriesApi->delete_task_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **task_category_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |

### Return type

[**TaskCategoryDto**](TaskCategoryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_task_category_by_id_async

> <TaskCategoryDto> get_task_category_by_id_async(task_category_id, tenant_id)

Gets a task category by ID

Retrieves the details of a task category using its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaskCategoriesApi.new
task_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a task category by ID
  result = api_instance.get_task_category_by_id_async(task_category_id, tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskCategoriesApi->get_task_category_by_id_async: #{e}"
end
```

#### Using the get_task_category_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TaskCategoryDto>, Integer, Hash)> get_task_category_by_id_async_with_http_info(task_category_id, tenant_id)

```ruby
begin
  # Gets a task category by ID
  data, status_code, headers = api_instance.get_task_category_by_id_async_with_http_info(task_category_id, tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TaskCategoryDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskCategoriesApi->get_task_category_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **task_category_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |

### Return type

[**TaskCategoryDto**](TaskCategoryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_task_category_task_types_async

> <TaskCategoryDto> get_task_category_task_types_async(task_category_id, tenant_id)

Retrieves task types for a category

Gets all task types belonging to the specified task category.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaskCategoriesApi.new
task_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Retrieves task types for a category
  result = api_instance.get_task_category_task_types_async(task_category_id, tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskCategoriesApi->get_task_category_task_types_async: #{e}"
end
```

#### Using the get_task_category_task_types_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TaskCategoryDto>, Integer, Hash)> get_task_category_task_types_async_with_http_info(task_category_id, tenant_id)

```ruby
begin
  # Retrieves task types for a category
  data, status_code, headers = api_instance.get_task_category_task_types_async_with_http_info(task_category_id, tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TaskCategoryDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskCategoriesApi->get_task_category_task_types_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **task_category_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |

### Return type

[**TaskCategoryDto**](TaskCategoryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_task_categories_async

> <TaskCategoryDtoListEnvelope> get_tenant_task_categories_async(tenant_id, opts)

Retrieves all task categories

Gets all task categories for the current tenant with OData support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaskCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  task_category_dto_collection_query_parameters: OpenapiClient::TaskCategoryDtoCollectionQueryParameters.new # TaskCategoryDtoCollectionQueryParameters | 
}

begin
  # Retrieves all task categories
  result = api_instance.get_tenant_task_categories_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskCategoriesApi->get_tenant_task_categories_async: #{e}"
end
```

#### Using the get_tenant_task_categories_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TaskCategoryDtoListEnvelope>, Integer, Hash)> get_tenant_task_categories_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieves all task categories
  data, status_code, headers = api_instance.get_tenant_task_categories_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TaskCategoryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskCategoriesApi->get_tenant_task_categories_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **task_category_dto_collection_query_parameters** | [**TaskCategoryDtoCollectionQueryParameters**](TaskCategoryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**TaskCategoryDtoListEnvelope**](TaskCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_task_category_async

> <EmptyEnvelope> patch_task_category_async(task_category_id, tenant_id, opts)

Patches a task category

Partially updates the specified task category.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaskCategoriesApi.new
task_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patches a task category
  result = api_instance.patch_task_category_async(task_category_id, tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskCategoriesApi->patch_task_category_async: #{e}"
end
```

#### Using the patch_task_category_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_task_category_async_with_http_info(task_category_id, tenant_id, opts)

```ruby
begin
  # Patches a task category
  data, status_code, headers = api_instance.patch_task_category_async_with_http_info(task_category_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskCategoriesApi->patch_task_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **task_category_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_task_category_async

> <TaskCategoryDto> update_task_category_async(task_category_id, tenant_id, opts)

Updates a task category

Updates the specified task category.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaskCategoriesApi.new
task_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  task_category_update_dto: OpenapiClient::TaskCategoryUpdateDto.new # TaskCategoryUpdateDto | 
}

begin
  # Updates a task category
  result = api_instance.update_task_category_async(task_category_id, tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskCategoriesApi->update_task_category_async: #{e}"
end
```

#### Using the update_task_category_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TaskCategoryDto>, Integer, Hash)> update_task_category_async_with_http_info(task_category_id, tenant_id, opts)

```ruby
begin
  # Updates a task category
  data, status_code, headers = api_instance.update_task_category_async_with_http_info(task_category_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TaskCategoryDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaskCategoriesApi->update_task_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **task_category_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **task_category_update_dto** | [**TaskCategoryUpdateDto**](TaskCategoryUpdateDto.md) |  | [optional] |

### Return type

[**TaskCategoryDto**](TaskCategoryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

