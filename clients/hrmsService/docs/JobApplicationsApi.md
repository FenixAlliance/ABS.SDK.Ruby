# OpenapiClient::JobApplicationsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**change_job_application_status_async**](JobApplicationsApi.md#change_job_application_status_async) | **POST** /api/v2/HrmsService/JobApplications/{jobApplicationId}/Status | Change job application status |
| [**create_job_application_async**](JobApplicationsApi.md#create_job_application_async) | **POST** /api/v2/HrmsService/JobApplications | Create a job application |
| [**delete_job_application_async**](JobApplicationsApi.md#delete_job_application_async) | **DELETE** /api/v2/HrmsService/JobApplications/{jobApplicationId} | Delete a job application |
| [**get_job_application_by_id_async**](JobApplicationsApi.md#get_job_application_by_id_async) | **GET** /api/v2/HrmsService/JobApplications/{jobApplicationId} | Get job application by ID |
| [**get_job_applications_async**](JobApplicationsApi.md#get_job_applications_async) | **GET** /api/v2/HrmsService/JobApplications | Get job applications |
| [**get_job_applications_count_async**](JobApplicationsApi.md#get_job_applications_count_async) | **GET** /api/v2/HrmsService/JobApplications/Count | Count job applications |
| [**patch_job_application_async**](JobApplicationsApi.md#patch_job_application_async) | **PATCH** /api/v2/HrmsService/JobApplications/{jobApplicationId} | Patch a job application |
| [**update_job_application_async**](JobApplicationsApi.md#update_job_application_async) | **PUT** /api/v2/HrmsService/JobApplications/{jobApplicationId} | Update a job application |


## change_job_application_status_async

> <EmptyEnvelope> change_job_application_status_async(tenant_id, job_application_id, status, opts)

Change job application status

Transitions the application to a new funnel status (e.g. UnderReview, Interviewing, Offered, Hired, Rejected). Raises JobApplicationStatusChanged; terminal statuses are immutable.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_application_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
status = 'Submitted' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Change job application status
  result = api_instance.change_job_application_status_async(tenant_id, job_application_id, status, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicationsApi->change_job_application_status_async: #{e}"
end
```

#### Using the change_job_application_status_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> change_job_application_status_async_with_http_info(tenant_id, job_application_id, status, opts)

```ruby
begin
  # Change job application status
  data, status_code, headers = api_instance.change_job_application_status_async_with_http_info(tenant_id, job_application_id, status, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicationsApi->change_job_application_status_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_application_id** | **String** |  |  |
| **status** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_job_application_async

> <EmptyEnvelope> create_job_application_async(tenant_id, opts)

Create a job application

Records a candidate's application against one of the tenant's job offers. The targeted job offer must belong to the tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  job_offer_application_create_dto: OpenapiClient::JobOfferApplicationCreateDto.new # JobOfferApplicationCreateDto | 
}

begin
  # Create a job application
  result = api_instance.create_job_application_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicationsApi->create_job_application_async: #{e}"
end
```

#### Using the create_job_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_job_application_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a job application
  data, status_code, headers = api_instance.create_job_application_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicationsApi->create_job_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **job_offer_application_create_dto** | [**JobOfferApplicationCreateDto**](JobOfferApplicationCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_job_application_async

> <EmptyEnvelope> delete_job_application_async(tenant_id, job_application_id, opts)

Delete a job application

Removes an application submitted against one of the tenant's job offers.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_application_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a job application
  result = api_instance.delete_job_application_async(tenant_id, job_application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicationsApi->delete_job_application_async: #{e}"
end
```

#### Using the delete_job_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_job_application_async_with_http_info(tenant_id, job_application_id, opts)

```ruby
begin
  # Delete a job application
  data, status_code, headers = api_instance.delete_job_application_async_with_http_info(tenant_id, job_application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicationsApi->delete_job_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_application_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_job_application_by_id_async

> <JobOfferApplicationDtoEnvelope> get_job_application_by_id_async(tenant_id, job_application_id, opts)

Get job application by ID

Retrieves a specific application submitted against one of the tenant's job offers.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_application_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get job application by ID
  result = api_instance.get_job_application_by_id_async(tenant_id, job_application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicationsApi->get_job_application_by_id_async: #{e}"
end
```

#### Using the get_job_application_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JobOfferApplicationDtoEnvelope>, Integer, Hash)> get_job_application_by_id_async_with_http_info(tenant_id, job_application_id, opts)

```ruby
begin
  # Get job application by ID
  data, status_code, headers = api_instance.get_job_application_by_id_async_with_http_info(tenant_id, job_application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JobOfferApplicationDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicationsApi->get_job_application_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_application_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**JobOfferApplicationDtoEnvelope**](JobOfferApplicationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_job_applications_async

> <JobOfferApplicationDtoListEnvelope> get_job_applications_async(tenant_id, opts)

Get job applications

Retrieves applications submitted against the tenant's job offers. Filter with `$filter=JobOfferId eq '...'` or `JobApplicantProfileId eq '...'`.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get job applications
  result = api_instance.get_job_applications_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicationsApi->get_job_applications_async: #{e}"
end
```

#### Using the get_job_applications_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JobOfferApplicationDtoListEnvelope>, Integer, Hash)> get_job_applications_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get job applications
  data, status_code, headers = api_instance.get_job_applications_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JobOfferApplicationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicationsApi->get_job_applications_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**JobOfferApplicationDtoListEnvelope**](JobOfferApplicationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_job_applications_count_async

> <Int32Envelope> get_job_applications_count_async(tenant_id, opts)

Count job applications

Counts applications submitted against the tenant's job offers.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count job applications
  result = api_instance.get_job_applications_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicationsApi->get_job_applications_count_async: #{e}"
end
```

#### Using the get_job_applications_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_job_applications_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count job applications
  data, status_code, headers = api_instance.get_job_applications_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicationsApi->get_job_applications_count_async_with_http_info: #{e}"
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


## patch_job_application_async

> <EmptyEnvelope> patch_job_application_async(tenant_id, job_application_id, opts)

Patch a job application

Partially updates an existing application submitted against one of the tenant's job offers.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_application_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a job application
  result = api_instance.patch_job_application_async(tenant_id, job_application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicationsApi->patch_job_application_async: #{e}"
end
```

#### Using the patch_job_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_job_application_async_with_http_info(tenant_id, job_application_id, opts)

```ruby
begin
  # Patch a job application
  data, status_code, headers = api_instance.patch_job_application_async_with_http_info(tenant_id, job_application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicationsApi->patch_job_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_application_id** | **String** |  |  |
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


## update_job_application_async

> <EmptyEnvelope> update_job_application_async(tenant_id, job_application_id, opts)

Update a job application

Updates an existing application submitted against one of the tenant's job offers.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_application_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  job_offer_application_update_dto: OpenapiClient::JobOfferApplicationUpdateDto.new # JobOfferApplicationUpdateDto | 
}

begin
  # Update a job application
  result = api_instance.update_job_application_async(tenant_id, job_application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicationsApi->update_job_application_async: #{e}"
end
```

#### Using the update_job_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_job_application_async_with_http_info(tenant_id, job_application_id, opts)

```ruby
begin
  # Update a job application
  data, status_code, headers = api_instance.update_job_application_async_with_http_info(tenant_id, job_application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobApplicationsApi->update_job_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_application_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **job_offer_application_update_dto** | [**JobOfferApplicationUpdateDto**](JobOfferApplicationUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

