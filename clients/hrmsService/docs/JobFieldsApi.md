# OpenapiClient::JobFieldsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_job_field_async**](JobFieldsApi.md#create_job_field_async) | **POST** /api/v2/HrmsService/JobFields | Create a job field |
| [**delete_job_field_async**](JobFieldsApi.md#delete_job_field_async) | **DELETE** /api/v2/HrmsService/JobFields/{jobFieldId} | Delete a job field |
| [**get_job_field_by_id_async**](JobFieldsApi.md#get_job_field_by_id_async) | **GET** /api/v2/HrmsService/JobFields/{jobFieldId} | Get job field by ID |
| [**get_job_fields_async**](JobFieldsApi.md#get_job_fields_async) | **GET** /api/v2/HrmsService/JobFields | Get job fields |
| [**get_job_fields_count_async**](JobFieldsApi.md#get_job_fields_count_async) | **GET** /api/v2/HrmsService/JobFields/Count | Count job fields |
| [**patch_job_field_async**](JobFieldsApi.md#patch_job_field_async) | **PATCH** /api/v2/HrmsService/JobFields/{jobFieldId} | Patch a job field |
| [**update_job_field_async**](JobFieldsApi.md#update_job_field_async) | **PUT** /api/v2/HrmsService/JobFields/{jobFieldId} | Update a job field |


## create_job_field_async

> <EmptyEnvelope> create_job_field_async(tenant_id, opts)

Create a job field

Creates a new job field (role domain) for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobFieldsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  job_field_create_dto: OpenapiClient::JobFieldCreateDto.new({name: 'name_example'}) # JobFieldCreateDto | 
}

begin
  # Create a job field
  result = api_instance.create_job_field_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobFieldsApi->create_job_field_async: #{e}"
end
```

#### Using the create_job_field_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_job_field_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a job field
  data, status_code, headers = api_instance.create_job_field_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobFieldsApi->create_job_field_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **job_field_create_dto** | [**JobFieldCreateDto**](JobFieldCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_job_field_async

> <EmptyEnvelope> delete_job_field_async(tenant_id, job_field_id, opts)

Delete a job field

Deletes a job field for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobFieldsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_field_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a job field
  result = api_instance.delete_job_field_async(tenant_id, job_field_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobFieldsApi->delete_job_field_async: #{e}"
end
```

#### Using the delete_job_field_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_job_field_async_with_http_info(tenant_id, job_field_id, opts)

```ruby
begin
  # Delete a job field
  data, status_code, headers = api_instance.delete_job_field_async_with_http_info(tenant_id, job_field_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobFieldsApi->delete_job_field_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_field_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_job_field_by_id_async

> <JobFieldDtoEnvelope> get_job_field_by_id_async(tenant_id, job_field_id, opts)

Get job field by ID

Retrieves a specific job field by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobFieldsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_field_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get job field by ID
  result = api_instance.get_job_field_by_id_async(tenant_id, job_field_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobFieldsApi->get_job_field_by_id_async: #{e}"
end
```

#### Using the get_job_field_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JobFieldDtoEnvelope>, Integer, Hash)> get_job_field_by_id_async_with_http_info(tenant_id, job_field_id, opts)

```ruby
begin
  # Get job field by ID
  data, status_code, headers = api_instance.get_job_field_by_id_async_with_http_info(tenant_id, job_field_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JobFieldDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobFieldsApi->get_job_field_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_field_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**JobFieldDtoEnvelope**](JobFieldDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_job_fields_async

> <JobFieldDtoListEnvelope> get_job_fields_async(tenant_id, opts)

Get job fields

Retrieves job field (role domain) taxonomy entries for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobFieldsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  job_field_dto_collection_query_parameters: OpenapiClient::JobFieldDtoCollectionQueryParameters.new # JobFieldDtoCollectionQueryParameters | 
}

begin
  # Get job fields
  result = api_instance.get_job_fields_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobFieldsApi->get_job_fields_async: #{e}"
end
```

#### Using the get_job_fields_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JobFieldDtoListEnvelope>, Integer, Hash)> get_job_fields_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get job fields
  data, status_code, headers = api_instance.get_job_fields_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JobFieldDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobFieldsApi->get_job_fields_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **job_field_dto_collection_query_parameters** | [**JobFieldDtoCollectionQueryParameters**](JobFieldDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**JobFieldDtoListEnvelope**](JobFieldDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_job_fields_count_async

> <Int32Envelope> get_job_fields_count_async(tenant_id, opts)

Count job fields

Counts job field taxonomy entries for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobFieldsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  job_field_dto_collection_query_parameters: OpenapiClient::JobFieldDtoCollectionQueryParameters.new # JobFieldDtoCollectionQueryParameters | 
}

begin
  # Count job fields
  result = api_instance.get_job_fields_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobFieldsApi->get_job_fields_count_async: #{e}"
end
```

#### Using the get_job_fields_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_job_fields_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count job fields
  data, status_code, headers = api_instance.get_job_fields_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobFieldsApi->get_job_fields_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **job_field_dto_collection_query_parameters** | [**JobFieldDtoCollectionQueryParameters**](JobFieldDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_job_field_async

> <EmptyEnvelope> patch_job_field_async(tenant_id, job_field_id, opts)

Patch a job field

Partially updates an existing job field for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobFieldsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_field_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a job field
  result = api_instance.patch_job_field_async(tenant_id, job_field_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobFieldsApi->patch_job_field_async: #{e}"
end
```

#### Using the patch_job_field_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_job_field_async_with_http_info(tenant_id, job_field_id, opts)

```ruby
begin
  # Patch a job field
  data, status_code, headers = api_instance.patch_job_field_async_with_http_info(tenant_id, job_field_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobFieldsApi->patch_job_field_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_field_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_job_field_async

> <EmptyEnvelope> update_job_field_async(tenant_id, job_field_id, opts)

Update a job field

Updates an existing job field for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobFieldsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_field_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  job_field_update_dto: OpenapiClient::JobFieldUpdateDto.new # JobFieldUpdateDto | 
}

begin
  # Update a job field
  result = api_instance.update_job_field_async(tenant_id, job_field_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobFieldsApi->update_job_field_async: #{e}"
end
```

#### Using the update_job_field_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_job_field_async_with_http_info(tenant_id, job_field_id, opts)

```ruby
begin
  # Update a job field
  data, status_code, headers = api_instance.update_job_field_async_with_http_info(tenant_id, job_field_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobFieldsApi->update_job_field_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_field_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **job_field_update_dto** | [**JobFieldUpdateDto**](JobFieldUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

