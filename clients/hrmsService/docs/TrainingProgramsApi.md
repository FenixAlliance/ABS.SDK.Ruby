# OpenapiClient::TrainingProgramsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_training_program_async**](TrainingProgramsApi.md#create_training_program_async) | **POST** /api/v2/HrmsService/TrainingPrograms | Create a training program |
| [**delete_training_program_async**](TrainingProgramsApi.md#delete_training_program_async) | **DELETE** /api/v2/HrmsService/TrainingPrograms/{programId} | Delete a training program |
| [**get_training_program_by_id_async**](TrainingProgramsApi.md#get_training_program_by_id_async) | **GET** /api/v2/HrmsService/TrainingPrograms/{programId} | Get training program by ID |
| [**get_training_programs_async**](TrainingProgramsApi.md#get_training_programs_async) | **GET** /api/v2/HrmsService/TrainingPrograms | Get training programs |
| [**get_training_programs_count_async**](TrainingProgramsApi.md#get_training_programs_count_async) | **GET** /api/v2/HrmsService/TrainingPrograms/Count | Count training programs |
| [**update_training_program_async**](TrainingProgramsApi.md#update_training_program_async) | **PUT** /api/v2/HrmsService/TrainingPrograms/{programId} | Update a training program |


## create_training_program_async

> <EmptyEnvelope> create_training_program_async(tenant_id, opts)

Create a training program

Creates a new training program for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrainingProgramsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  training_program_create_dto: OpenapiClient::TrainingProgramCreateDto.new({title: 'title_example'}) # TrainingProgramCreateDto | 
}

begin
  # Create a training program
  result = api_instance.create_training_program_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramsApi->create_training_program_async: #{e}"
end
```

#### Using the create_training_program_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_training_program_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a training program
  data, status_code, headers = api_instance.create_training_program_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramsApi->create_training_program_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **training_program_create_dto** | [**TrainingProgramCreateDto**](TrainingProgramCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_training_program_async

> <EmptyEnvelope> delete_training_program_async(tenant_id, program_id, opts)

Delete a training program

Deletes a training program for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrainingProgramsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
program_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a training program
  result = api_instance.delete_training_program_async(tenant_id, program_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramsApi->delete_training_program_async: #{e}"
end
```

#### Using the delete_training_program_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_training_program_async_with_http_info(tenant_id, program_id, opts)

```ruby
begin
  # Delete a training program
  data, status_code, headers = api_instance.delete_training_program_async_with_http_info(tenant_id, program_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramsApi->delete_training_program_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **program_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_training_program_by_id_async

> <TrainingProgramDtoEnvelope> get_training_program_by_id_async(tenant_id, program_id, opts)

Get training program by ID

Retrieves a specific training program by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrainingProgramsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
program_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get training program by ID
  result = api_instance.get_training_program_by_id_async(tenant_id, program_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramsApi->get_training_program_by_id_async: #{e}"
end
```

#### Using the get_training_program_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TrainingProgramDtoEnvelope>, Integer, Hash)> get_training_program_by_id_async_with_http_info(tenant_id, program_id, opts)

```ruby
begin
  # Get training program by ID
  data, status_code, headers = api_instance.get_training_program_by_id_async_with_http_info(tenant_id, program_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TrainingProgramDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramsApi->get_training_program_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **program_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TrainingProgramDtoEnvelope**](TrainingProgramDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_training_programs_async

> <TrainingProgramDtoListEnvelope> get_training_programs_async(tenant_id, opts)

Get training programs

Retrieves training programs for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrainingProgramsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get training programs
  result = api_instance.get_training_programs_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramsApi->get_training_programs_async: #{e}"
end
```

#### Using the get_training_programs_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TrainingProgramDtoListEnvelope>, Integer, Hash)> get_training_programs_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get training programs
  data, status_code, headers = api_instance.get_training_programs_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TrainingProgramDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramsApi->get_training_programs_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TrainingProgramDtoListEnvelope**](TrainingProgramDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_training_programs_count_async

> <Int32Envelope> get_training_programs_count_async(tenant_id, opts)

Count training programs

Counts training programs for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrainingProgramsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count training programs
  result = api_instance.get_training_programs_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramsApi->get_training_programs_count_async: #{e}"
end
```

#### Using the get_training_programs_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_training_programs_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count training programs
  data, status_code, headers = api_instance.get_training_programs_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramsApi->get_training_programs_count_async_with_http_info: #{e}"
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


## update_training_program_async

> <EmptyEnvelope> update_training_program_async(tenant_id, program_id, opts)

Update a training program

Updates an existing training program for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrainingProgramsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
program_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  training_program_update_dto: OpenapiClient::TrainingProgramUpdateDto.new # TrainingProgramUpdateDto | 
}

begin
  # Update a training program
  result = api_instance.update_training_program_async(tenant_id, program_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramsApi->update_training_program_async: #{e}"
end
```

#### Using the update_training_program_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_training_program_async_with_http_info(tenant_id, program_id, opts)

```ruby
begin
  # Update a training program
  data, status_code, headers = api_instance.update_training_program_async_with_http_info(tenant_id, program_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramsApi->update_training_program_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **program_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **training_program_update_dto** | [**TrainingProgramUpdateDto**](TrainingProgramUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

