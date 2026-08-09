# OpenapiClient::JobApplicantsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_job_applicant_async**](JobApplicantsApi.md#create_job_applicant_async) | **POST** /api/v2/HrmsService/JobApplicants | Create a job applicant |
| [**delete_job_applicant_async**](JobApplicantsApi.md#delete_job_applicant_async) | **DELETE** /api/v2/HrmsService/JobApplicants/{jobApplicantId} | Delete a job applicant |
| [**get_job_applicant_by_id_async**](JobApplicantsApi.md#get_job_applicant_by_id_async) | **GET** /api/v2/HrmsService/JobApplicants/{jobApplicantId} | Get job applicant by ID |
| [**get_job_applicants_async**](JobApplicantsApi.md#get_job_applicants_async) | **GET** /api/v2/HrmsService/JobApplicants | Get job applicants |
| [**get_job_applicants_count_async**](JobApplicantsApi.md#get_job_applicants_count_async) | **GET** /api/v2/HrmsService/JobApplicants/Count | Count job applicants |
| [**patch_job_applicant_async**](JobApplicantsApi.md#patch_job_applicant_async) | **PATCH** /api/v2/HrmsService/JobApplicants/{jobApplicantId} | Patch a job applicant |
| [**update_job_applicant_async**](JobApplicantsApi.md#update_job_applicant_async) | **PUT** /api/v2/HrmsService/JobApplicants/{jobApplicantId} | Update a job applicant |


## create_job_applicant_async

> <EmptyEnvelope> create_job_applicant_async(tenant_id, opts)

Create a job applicant

Creates a new job applicant (candidate) profile for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobApplicantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  job_applicant_profile_create_dto: OpenapiClient::JobApplicantProfileCreateDto.new # JobApplicantProfileCreateDto | 
}

begin
  # Create a job applicant
  result = api_instance.create_job_applicant_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicantsApi->create_job_applicant_async: #{e}"
end
```

#### Using the create_job_applicant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_job_applicant_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a job applicant
  data, status_code, headers = api_instance.create_job_applicant_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicantsApi->create_job_applicant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **job_applicant_profile_create_dto** | [**JobApplicantProfileCreateDto**](JobApplicantProfileCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_job_applicant_async

> <EmptyEnvelope> delete_job_applicant_async(tenant_id, job_applicant_id, opts)

Delete a job applicant

Deletes a job applicant (candidate) profile for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobApplicantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_applicant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a job applicant
  result = api_instance.delete_job_applicant_async(tenant_id, job_applicant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicantsApi->delete_job_applicant_async: #{e}"
end
```

#### Using the delete_job_applicant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_job_applicant_async_with_http_info(tenant_id, job_applicant_id, opts)

```ruby
begin
  # Delete a job applicant
  data, status_code, headers = api_instance.delete_job_applicant_async_with_http_info(tenant_id, job_applicant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicantsApi->delete_job_applicant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_applicant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_job_applicant_by_id_async

> <JobApplicantProfileDtoEnvelope> get_job_applicant_by_id_async(tenant_id, job_applicant_id, opts)

Get job applicant by ID

Retrieves a specific job applicant (candidate) profile by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobApplicantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_applicant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get job applicant by ID
  result = api_instance.get_job_applicant_by_id_async(tenant_id, job_applicant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicantsApi->get_job_applicant_by_id_async: #{e}"
end
```

#### Using the get_job_applicant_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JobApplicantProfileDtoEnvelope>, Integer, Hash)> get_job_applicant_by_id_async_with_http_info(tenant_id, job_applicant_id, opts)

```ruby
begin
  # Get job applicant by ID
  data, status_code, headers = api_instance.get_job_applicant_by_id_async_with_http_info(tenant_id, job_applicant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JobApplicantProfileDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicantsApi->get_job_applicant_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_applicant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**JobApplicantProfileDtoEnvelope**](JobApplicantProfileDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_job_applicants_async

> <JobApplicantProfileDtoListEnvelope> get_job_applicants_async(tenant_id, opts)

Get job applicants

Retrieves job applicant (candidate) profiles for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobApplicantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  job_applicant_profile_dto_collection_query_parameters: OpenapiClient::JobApplicantProfileDtoCollectionQueryParameters.new # JobApplicantProfileDtoCollectionQueryParameters | 
}

begin
  # Get job applicants
  result = api_instance.get_job_applicants_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicantsApi->get_job_applicants_async: #{e}"
end
```

#### Using the get_job_applicants_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JobApplicantProfileDtoListEnvelope>, Integer, Hash)> get_job_applicants_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get job applicants
  data, status_code, headers = api_instance.get_job_applicants_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JobApplicantProfileDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicantsApi->get_job_applicants_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **job_applicant_profile_dto_collection_query_parameters** | [**JobApplicantProfileDtoCollectionQueryParameters**](JobApplicantProfileDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**JobApplicantProfileDtoListEnvelope**](JobApplicantProfileDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_job_applicants_count_async

> <Int32Envelope> get_job_applicants_count_async(tenant_id, opts)

Count job applicants

Counts job applicant profiles for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobApplicantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  job_applicant_profile_dto_collection_query_parameters: OpenapiClient::JobApplicantProfileDtoCollectionQueryParameters.new # JobApplicantProfileDtoCollectionQueryParameters | 
}

begin
  # Count job applicants
  result = api_instance.get_job_applicants_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicantsApi->get_job_applicants_count_async: #{e}"
end
```

#### Using the get_job_applicants_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_job_applicants_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count job applicants
  data, status_code, headers = api_instance.get_job_applicants_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicantsApi->get_job_applicants_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **job_applicant_profile_dto_collection_query_parameters** | [**JobApplicantProfileDtoCollectionQueryParameters**](JobApplicantProfileDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_job_applicant_async

> <EmptyEnvelope> patch_job_applicant_async(tenant_id, job_applicant_id, opts)

Patch a job applicant

Partially updates an existing job applicant (candidate) profile for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobApplicantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_applicant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a job applicant
  result = api_instance.patch_job_applicant_async(tenant_id, job_applicant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicantsApi->patch_job_applicant_async: #{e}"
end
```

#### Using the patch_job_applicant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_job_applicant_async_with_http_info(tenant_id, job_applicant_id, opts)

```ruby
begin
  # Patch a job applicant
  data, status_code, headers = api_instance.patch_job_applicant_async_with_http_info(tenant_id, job_applicant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicantsApi->patch_job_applicant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_applicant_id** | **String** |  |  |
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


## update_job_applicant_async

> <EmptyEnvelope> update_job_applicant_async(tenant_id, job_applicant_id, opts)

Update a job applicant

Updates an existing job applicant (candidate) profile for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobApplicantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_applicant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  job_applicant_profile_update_dto: OpenapiClient::JobApplicantProfileUpdateDto.new # JobApplicantProfileUpdateDto | 
}

begin
  # Update a job applicant
  result = api_instance.update_job_applicant_async(tenant_id, job_applicant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicantsApi->update_job_applicant_async: #{e}"
end
```

#### Using the update_job_applicant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_job_applicant_async_with_http_info(tenant_id, job_applicant_id, opts)

```ruby
begin
  # Update a job applicant
  data, status_code, headers = api_instance.update_job_applicant_async_with_http_info(tenant_id, job_applicant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicantsApi->update_job_applicant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_applicant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **job_applicant_profile_update_dto** | [**JobApplicantProfileUpdateDto**](JobApplicantProfileUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

