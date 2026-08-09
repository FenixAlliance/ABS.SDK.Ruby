# OpenapiClient::AppraisalWorkflowsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_appraisal_workflow_async**](AppraisalWorkflowsApi.md#create_appraisal_workflow_async) | **POST** /api/v2/HrmsService/AppraisalWorkflows | Create an appraisal workflow |
| [**delete_appraisal_workflow_async**](AppraisalWorkflowsApi.md#delete_appraisal_workflow_async) | **DELETE** /api/v2/HrmsService/AppraisalWorkflows/{workflowId} | Delete an appraisal workflow |
| [**get_appraisal_workflow_by_id_async**](AppraisalWorkflowsApi.md#get_appraisal_workflow_by_id_async) | **GET** /api/v2/HrmsService/AppraisalWorkflows/{workflowId} | Get appraisal workflow by ID |
| [**get_appraisal_workflows_async**](AppraisalWorkflowsApi.md#get_appraisal_workflows_async) | **GET** /api/v2/HrmsService/AppraisalWorkflows | Get appraisal workflows |
| [**get_appraisal_workflows_count_async**](AppraisalWorkflowsApi.md#get_appraisal_workflows_count_async) | **GET** /api/v2/HrmsService/AppraisalWorkflows/Count | Count appraisal workflows |
| [**update_appraisal_workflow_async**](AppraisalWorkflowsApi.md#update_appraisal_workflow_async) | **PUT** /api/v2/HrmsService/AppraisalWorkflows/{workflowId} | Update an appraisal workflow |


## create_appraisal_workflow_async

> <EmptyEnvelope> create_appraisal_workflow_async(tenant_id, opts)

Create an appraisal workflow

Creates a new appraisal workflow for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AppraisalWorkflowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  appraisal_workflow_create_dto: OpenapiClient::AppraisalWorkflowCreateDto.new({name: 'name_example'}) # AppraisalWorkflowCreateDto | 
}

begin
  # Create an appraisal workflow
  result = api_instance.create_appraisal_workflow_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalWorkflowsApi->create_appraisal_workflow_async: #{e}"
end
```

#### Using the create_appraisal_workflow_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_appraisal_workflow_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create an appraisal workflow
  data, status_code, headers = api_instance.create_appraisal_workflow_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalWorkflowsApi->create_appraisal_workflow_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **appraisal_workflow_create_dto** | [**AppraisalWorkflowCreateDto**](AppraisalWorkflowCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_appraisal_workflow_async

> <EmptyEnvelope> delete_appraisal_workflow_async(tenant_id, workflow_id, opts)

Delete an appraisal workflow

Deletes an appraisal workflow for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AppraisalWorkflowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
workflow_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an appraisal workflow
  result = api_instance.delete_appraisal_workflow_async(tenant_id, workflow_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalWorkflowsApi->delete_appraisal_workflow_async: #{e}"
end
```

#### Using the delete_appraisal_workflow_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_appraisal_workflow_async_with_http_info(tenant_id, workflow_id, opts)

```ruby
begin
  # Delete an appraisal workflow
  data, status_code, headers = api_instance.delete_appraisal_workflow_async_with_http_info(tenant_id, workflow_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalWorkflowsApi->delete_appraisal_workflow_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **workflow_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_appraisal_workflow_by_id_async

> <AppraisalWorkflowDtoEnvelope> get_appraisal_workflow_by_id_async(tenant_id, workflow_id, opts)

Get appraisal workflow by ID

Retrieves a specific appraisal workflow by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AppraisalWorkflowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
workflow_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get appraisal workflow by ID
  result = api_instance.get_appraisal_workflow_by_id_async(tenant_id, workflow_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalWorkflowsApi->get_appraisal_workflow_by_id_async: #{e}"
end
```

#### Using the get_appraisal_workflow_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AppraisalWorkflowDtoEnvelope>, Integer, Hash)> get_appraisal_workflow_by_id_async_with_http_info(tenant_id, workflow_id, opts)

```ruby
begin
  # Get appraisal workflow by ID
  data, status_code, headers = api_instance.get_appraisal_workflow_by_id_async_with_http_info(tenant_id, workflow_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AppraisalWorkflowDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalWorkflowsApi->get_appraisal_workflow_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **workflow_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**AppraisalWorkflowDtoEnvelope**](AppraisalWorkflowDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_appraisal_workflows_async

> <AppraisalWorkflowDtoListEnvelope> get_appraisal_workflows_async(tenant_id, opts)

Get appraisal workflows

Retrieves appraisal workflows for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AppraisalWorkflowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  appraisal_workflow_dto_collection_query_parameters: OpenapiClient::AppraisalWorkflowDtoCollectionQueryParameters.new # AppraisalWorkflowDtoCollectionQueryParameters | 
}

begin
  # Get appraisal workflows
  result = api_instance.get_appraisal_workflows_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalWorkflowsApi->get_appraisal_workflows_async: #{e}"
end
```

#### Using the get_appraisal_workflows_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AppraisalWorkflowDtoListEnvelope>, Integer, Hash)> get_appraisal_workflows_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get appraisal workflows
  data, status_code, headers = api_instance.get_appraisal_workflows_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AppraisalWorkflowDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalWorkflowsApi->get_appraisal_workflows_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **appraisal_workflow_dto_collection_query_parameters** | [**AppraisalWorkflowDtoCollectionQueryParameters**](AppraisalWorkflowDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AppraisalWorkflowDtoListEnvelope**](AppraisalWorkflowDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_appraisal_workflows_count_async

> <Int32Envelope> get_appraisal_workflows_count_async(tenant_id, opts)

Count appraisal workflows

Counts appraisal workflows for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AppraisalWorkflowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  appraisal_workflow_dto_collection_query_parameters: OpenapiClient::AppraisalWorkflowDtoCollectionQueryParameters.new # AppraisalWorkflowDtoCollectionQueryParameters | 
}

begin
  # Count appraisal workflows
  result = api_instance.get_appraisal_workflows_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalWorkflowsApi->get_appraisal_workflows_count_async: #{e}"
end
```

#### Using the get_appraisal_workflows_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_appraisal_workflows_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count appraisal workflows
  data, status_code, headers = api_instance.get_appraisal_workflows_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalWorkflowsApi->get_appraisal_workflows_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **appraisal_workflow_dto_collection_query_parameters** | [**AppraisalWorkflowDtoCollectionQueryParameters**](AppraisalWorkflowDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_appraisal_workflow_async

> <EmptyEnvelope> update_appraisal_workflow_async(tenant_id, workflow_id, opts)

Update an appraisal workflow

Updates an existing appraisal workflow for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AppraisalWorkflowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
workflow_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  appraisal_workflow_update_dto: OpenapiClient::AppraisalWorkflowUpdateDto.new # AppraisalWorkflowUpdateDto | 
}

begin
  # Update an appraisal workflow
  result = api_instance.update_appraisal_workflow_async(tenant_id, workflow_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalWorkflowsApi->update_appraisal_workflow_async: #{e}"
end
```

#### Using the update_appraisal_workflow_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_appraisal_workflow_async_with_http_info(tenant_id, workflow_id, opts)

```ruby
begin
  # Update an appraisal workflow
  data, status_code, headers = api_instance.update_appraisal_workflow_async_with_http_info(tenant_id, workflow_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalWorkflowsApi->update_appraisal_workflow_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **workflow_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **appraisal_workflow_update_dto** | [**AppraisalWorkflowUpdateDto**](AppraisalWorkflowUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

