# OpenapiClient::TimeLogApprovalsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**request_project_hours_approval_async**](TimeLogApprovalsApi.md#request_project_hours_approval_async) | **POST** /api/v2/ProjectsService/TimeLogApprovals | Request project hours approval |
| [**update_project_hours_approval_approver_async**](TimeLogApprovalsApi.md#update_project_hours_approval_approver_async) | **PUT** /api/v2/ProjectsService/TimeLogApprovals/{approvalId}/Approver | Update approval approver |
| [**update_project_hours_approval_status_async**](TimeLogApprovalsApi.md#update_project_hours_approval_status_async) | **PUT** /api/v2/ProjectsService/TimeLogApprovals/{approvalId}/Status | Update approval status |


## request_project_hours_approval_async

> request_project_hours_approval_async(tenant_id, opts)

Request project hours approval

Creates a new project hours approval request.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeLogApprovalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  project_hours_approval_create_dto: OpenapiClient::ProjectHoursApprovalCreateDto.new # ProjectHoursApprovalCreateDto | 
}

begin
  # Request project hours approval
  api_instance.request_project_hours_approval_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogApprovalsApi->request_project_hours_approval_async: #{e}"
end
```

#### Using the request_project_hours_approval_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> request_project_hours_approval_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Request project hours approval
  data, status_code, headers = api_instance.request_project_hours_approval_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogApprovalsApi->request_project_hours_approval_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **project_hours_approval_create_dto** | [**ProjectHoursApprovalCreateDto**](ProjectHoursApprovalCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_project_hours_approval_approver_async

> update_project_hours_approval_approver_async(approval_id, tenant_id, opts)

Update approval approver

Updates the approver of an existing project hours approval.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeLogApprovalsApi.new
approval_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  project_hours_approval_approver_update_dto: OpenapiClient::ProjectHoursApprovalApproverUpdateDto.new # ProjectHoursApprovalApproverUpdateDto | 
}

begin
  # Update approval approver
  api_instance.update_project_hours_approval_approver_async(approval_id, tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogApprovalsApi->update_project_hours_approval_approver_async: #{e}"
end
```

#### Using the update_project_hours_approval_approver_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_project_hours_approval_approver_async_with_http_info(approval_id, tenant_id, opts)

```ruby
begin
  # Update approval approver
  data, status_code, headers = api_instance.update_project_hours_approval_approver_async_with_http_info(approval_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogApprovalsApi->update_project_hours_approval_approver_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **approval_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **project_hours_approval_approver_update_dto** | [**ProjectHoursApprovalApproverUpdateDto**](ProjectHoursApprovalApproverUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_project_hours_approval_status_async

> update_project_hours_approval_status_async(tenant_id, approval_id, opts)

Update approval status

Updates the status of an existing project hours approval.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeLogApprovalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
approval_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  project_hours_approval_status_update_dto: OpenapiClient::ProjectHoursApprovalStatusUpdateDto.new # ProjectHoursApprovalStatusUpdateDto | 
}

begin
  # Update approval status
  api_instance.update_project_hours_approval_status_async(tenant_id, approval_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogApprovalsApi->update_project_hours_approval_status_async: #{e}"
end
```

#### Using the update_project_hours_approval_status_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_project_hours_approval_status_async_with_http_info(tenant_id, approval_id, opts)

```ruby
begin
  # Update approval status
  data, status_code, headers = api_instance.update_project_hours_approval_status_async_with_http_info(tenant_id, approval_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeLogApprovalsApi->update_project_hours_approval_status_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **approval_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **project_hours_approval_status_update_dto** | [**ProjectHoursApprovalStatusUpdateDto**](ProjectHoursApprovalStatusUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

