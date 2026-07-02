# OpenapiClient::AppraisalStagesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_appraisal_stage_async**](AppraisalStagesApi.md#create_appraisal_stage_async) | **POST** /api/v2/HrmsService/AppraisalStages | Create an appraisal stage |
| [**delete_appraisal_stage_async**](AppraisalStagesApi.md#delete_appraisal_stage_async) | **DELETE** /api/v2/HrmsService/AppraisalStages/{stageId} | Delete an appraisal stage |
| [**get_appraisal_stage_by_id_async**](AppraisalStagesApi.md#get_appraisal_stage_by_id_async) | **GET** /api/v2/HrmsService/AppraisalStages/{stageId} | Get appraisal stage by ID |
| [**get_appraisal_stages_async**](AppraisalStagesApi.md#get_appraisal_stages_async) | **GET** /api/v2/HrmsService/AppraisalStages | Get appraisal stages |
| [**get_appraisal_stages_count_async**](AppraisalStagesApi.md#get_appraisal_stages_count_async) | **GET** /api/v2/HrmsService/AppraisalStages/Count | Count appraisal stages |
| [**update_appraisal_stage_async**](AppraisalStagesApi.md#update_appraisal_stage_async) | **PUT** /api/v2/HrmsService/AppraisalStages/{stageId} | Update an appraisal stage |


## create_appraisal_stage_async

> <EmptyEnvelope> create_appraisal_stage_async(tenant_id, opts)

Create an appraisal stage

Creates a new appraisal stage for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AppraisalStagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  appraisal_stage_create_dto: OpenapiClient::AppraisalStageCreateDto.new({name: 'name_example', appraisal_workflow_id: 'appraisal_workflow_id_example', stage_order: 37}) # AppraisalStageCreateDto | 
}

begin
  # Create an appraisal stage
  result = api_instance.create_appraisal_stage_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalStagesApi->create_appraisal_stage_async: #{e}"
end
```

#### Using the create_appraisal_stage_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_appraisal_stage_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create an appraisal stage
  data, status_code, headers = api_instance.create_appraisal_stage_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalStagesApi->create_appraisal_stage_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **appraisal_stage_create_dto** | [**AppraisalStageCreateDto**](AppraisalStageCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_appraisal_stage_async

> <EmptyEnvelope> delete_appraisal_stage_async(tenant_id, stage_id, opts)

Delete an appraisal stage

Deletes an appraisal stage for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AppraisalStagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
stage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an appraisal stage
  result = api_instance.delete_appraisal_stage_async(tenant_id, stage_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalStagesApi->delete_appraisal_stage_async: #{e}"
end
```

#### Using the delete_appraisal_stage_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_appraisal_stage_async_with_http_info(tenant_id, stage_id, opts)

```ruby
begin
  # Delete an appraisal stage
  data, status_code, headers = api_instance.delete_appraisal_stage_async_with_http_info(tenant_id, stage_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalStagesApi->delete_appraisal_stage_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **stage_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_appraisal_stage_by_id_async

> <AppraisalStageDtoEnvelope> get_appraisal_stage_by_id_async(tenant_id, stage_id, opts)

Get appraisal stage by ID

Retrieves a specific appraisal stage by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AppraisalStagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
stage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get appraisal stage by ID
  result = api_instance.get_appraisal_stage_by_id_async(tenant_id, stage_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalStagesApi->get_appraisal_stage_by_id_async: #{e}"
end
```

#### Using the get_appraisal_stage_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AppraisalStageDtoEnvelope>, Integer, Hash)> get_appraisal_stage_by_id_async_with_http_info(tenant_id, stage_id, opts)

```ruby
begin
  # Get appraisal stage by ID
  data, status_code, headers = api_instance.get_appraisal_stage_by_id_async_with_http_info(tenant_id, stage_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AppraisalStageDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalStagesApi->get_appraisal_stage_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **stage_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**AppraisalStageDtoEnvelope**](AppraisalStageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_appraisal_stages_async

> <AppraisalStageDtoListEnvelope> get_appraisal_stages_async(tenant_id, opts)

Get appraisal stages

Retrieves appraisal stages for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AppraisalStagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get appraisal stages
  result = api_instance.get_appraisal_stages_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalStagesApi->get_appraisal_stages_async: #{e}"
end
```

#### Using the get_appraisal_stages_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AppraisalStageDtoListEnvelope>, Integer, Hash)> get_appraisal_stages_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get appraisal stages
  data, status_code, headers = api_instance.get_appraisal_stages_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AppraisalStageDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalStagesApi->get_appraisal_stages_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**AppraisalStageDtoListEnvelope**](AppraisalStageDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_appraisal_stages_count_async

> <Int32Envelope> get_appraisal_stages_count_async(tenant_id, opts)

Count appraisal stages

Counts appraisal stages for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AppraisalStagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count appraisal stages
  result = api_instance.get_appraisal_stages_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalStagesApi->get_appraisal_stages_count_async: #{e}"
end
```

#### Using the get_appraisal_stages_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_appraisal_stages_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count appraisal stages
  data, status_code, headers = api_instance.get_appraisal_stages_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalStagesApi->get_appraisal_stages_count_async_with_http_info: #{e}"
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


## update_appraisal_stage_async

> <EmptyEnvelope> update_appraisal_stage_async(tenant_id, stage_id, opts)

Update an appraisal stage

Updates an existing appraisal stage for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AppraisalStagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
stage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  appraisal_stage_update_dto: OpenapiClient::AppraisalStageUpdateDto.new # AppraisalStageUpdateDto | 
}

begin
  # Update an appraisal stage
  result = api_instance.update_appraisal_stage_async(tenant_id, stage_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalStagesApi->update_appraisal_stage_async: #{e}"
end
```

#### Using the update_appraisal_stage_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_appraisal_stage_async_with_http_info(tenant_id, stage_id, opts)

```ruby
begin
  # Update an appraisal stage
  data, status_code, headers = api_instance.update_appraisal_stage_async_with_http_info(tenant_id, stage_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AppraisalStagesApi->update_appraisal_stage_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **stage_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **appraisal_stage_update_dto** | [**AppraisalStageUpdateDto**](AppraisalStageUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

