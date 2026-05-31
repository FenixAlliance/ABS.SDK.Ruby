# OpenapiClient::JobTitlesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_job_title_async**](JobTitlesApi.md#create_job_title_async) | **POST** /api/v2/HrmsService/JobTitles | Create a job title |
| [**delete_job_title_async**](JobTitlesApi.md#delete_job_title_async) | **DELETE** /api/v2/HrmsService/JobTitles/{jobTitleId} | Delete a job title |
| [**get_job_title_by_id_async**](JobTitlesApi.md#get_job_title_by_id_async) | **GET** /api/v2/HrmsService/JobTitles/{jobTitleId} | Get job title by ID |
| [**get_job_titles_async**](JobTitlesApi.md#get_job_titles_async) | **GET** /api/v2/HrmsService/JobTitles | Get job titles |
| [**get_job_titles_count_async**](JobTitlesApi.md#get_job_titles_count_async) | **GET** /api/v2/HrmsService/JobTitles/Count | Count job titles |
| [**update_job_title_async**](JobTitlesApi.md#update_job_title_async) | **PUT** /api/v2/HrmsService/JobTitles/{jobTitleId} | Update a job title |


## create_job_title_async

> <EmptyEnvelope> create_job_title_async(tenant_id, opts)

Create a job title

Creates a new job title for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobTitlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  job_title_create_dto: OpenapiClient::JobTitleCreateDto.new # JobTitleCreateDto | 
}

begin
  # Create a job title
  result = api_instance.create_job_title_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobTitlesApi->create_job_title_async: #{e}"
end
```

#### Using the create_job_title_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_job_title_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a job title
  data, status_code, headers = api_instance.create_job_title_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobTitlesApi->create_job_title_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **job_title_create_dto** | [**JobTitleCreateDto**](JobTitleCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_job_title_async

> <EmptyEnvelope> delete_job_title_async(tenant_id, job_title_id, opts)

Delete a job title

Deletes a job title for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobTitlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_title_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a job title
  result = api_instance.delete_job_title_async(tenant_id, job_title_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobTitlesApi->delete_job_title_async: #{e}"
end
```

#### Using the delete_job_title_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_job_title_async_with_http_info(tenant_id, job_title_id, opts)

```ruby
begin
  # Delete a job title
  data, status_code, headers = api_instance.delete_job_title_async_with_http_info(tenant_id, job_title_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobTitlesApi->delete_job_title_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_title_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_job_title_by_id_async

> <JobTitleDtoEnvelope> get_job_title_by_id_async(tenant_id, job_title_id, opts)

Get job title by ID

Retrieves a specific job title by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobTitlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_title_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get job title by ID
  result = api_instance.get_job_title_by_id_async(tenant_id, job_title_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobTitlesApi->get_job_title_by_id_async: #{e}"
end
```

#### Using the get_job_title_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JobTitleDtoEnvelope>, Integer, Hash)> get_job_title_by_id_async_with_http_info(tenant_id, job_title_id, opts)

```ruby
begin
  # Get job title by ID
  data, status_code, headers = api_instance.get_job_title_by_id_async_with_http_info(tenant_id, job_title_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JobTitleDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobTitlesApi->get_job_title_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_title_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**JobTitleDtoEnvelope**](JobTitleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_job_titles_async

> <JobTitleDtoListEnvelope> get_job_titles_async(tenant_id, opts)

Get job titles

Retrieves job titles for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobTitlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get job titles
  result = api_instance.get_job_titles_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobTitlesApi->get_job_titles_async: #{e}"
end
```

#### Using the get_job_titles_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JobTitleDtoListEnvelope>, Integer, Hash)> get_job_titles_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get job titles
  data, status_code, headers = api_instance.get_job_titles_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JobTitleDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobTitlesApi->get_job_titles_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**JobTitleDtoListEnvelope**](JobTitleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_job_titles_count_async

> <Int32Envelope> get_job_titles_count_async(tenant_id, opts)

Count job titles

Counts job titles for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobTitlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count job titles
  result = api_instance.get_job_titles_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobTitlesApi->get_job_titles_count_async: #{e}"
end
```

#### Using the get_job_titles_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_job_titles_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count job titles
  data, status_code, headers = api_instance.get_job_titles_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobTitlesApi->get_job_titles_count_async_with_http_info: #{e}"
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


## update_job_title_async

> <EmptyEnvelope> update_job_title_async(tenant_id, job_title_id, opts)

Update a job title

Updates an existing job title for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobTitlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_title_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  job_title_update_dto: OpenapiClient::JobTitleUpdateDto.new # JobTitleUpdateDto | 
}

begin
  # Update a job title
  result = api_instance.update_job_title_async(tenant_id, job_title_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobTitlesApi->update_job_title_async: #{e}"
end
```

#### Using the update_job_title_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_job_title_async_with_http_info(tenant_id, job_title_id, opts)

```ruby
begin
  # Update a job title
  data, status_code, headers = api_instance.update_job_title_async_with_http_info(tenant_id, job_title_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobTitlesApi->update_job_title_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_title_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **job_title_update_dto** | [**JobTitleUpdateDto**](JobTitleUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

