# OpenapiClient::SchedulesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_schedule_async**](SchedulesApi.md#create_schedule_async) | **POST** /api/v2/HrmsService/Schedules | Create a schedule |
| [**delete_schedule_async**](SchedulesApi.md#delete_schedule_async) | **DELETE** /api/v2/HrmsService/Schedules/{scheduleId} | Delete a schedule |
| [**get_schedule_by_id_async**](SchedulesApi.md#get_schedule_by_id_async) | **GET** /api/v2/HrmsService/Schedules/{scheduleId} | Get schedule by ID |
| [**get_schedules_async**](SchedulesApi.md#get_schedules_async) | **GET** /api/v2/HrmsService/Schedules | Get schedules |
| [**get_schedules_count_async**](SchedulesApi.md#get_schedules_count_async) | **GET** /api/v2/HrmsService/Schedules/Count | Count schedules |
| [**patch_schedule_async**](SchedulesApi.md#patch_schedule_async) | **PATCH** /api/v2/HrmsService/Schedules/{scheduleId} | Patch a schedule |
| [**update_schedule_async**](SchedulesApi.md#update_schedule_async) | **PUT** /api/v2/HrmsService/Schedules/{scheduleId} | Update a schedule |


## create_schedule_async

> <EmptyEnvelope> create_schedule_async(tenant_id, opts)

Create a schedule

Creates a new schedule for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SchedulesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  schedule_create_dto: OpenapiClient::ScheduleCreateDto.new({name: 'name_example'}) # ScheduleCreateDto | 
}

begin
  # Create a schedule
  result = api_instance.create_schedule_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SchedulesApi->create_schedule_async: #{e}"
end
```

#### Using the create_schedule_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_schedule_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a schedule
  data, status_code, headers = api_instance.create_schedule_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SchedulesApi->create_schedule_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **schedule_create_dto** | [**ScheduleCreateDto**](ScheduleCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_schedule_async

> <EmptyEnvelope> delete_schedule_async(tenant_id, schedule_id, opts)

Delete a schedule

Deletes a schedule for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SchedulesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
schedule_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a schedule
  result = api_instance.delete_schedule_async(tenant_id, schedule_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SchedulesApi->delete_schedule_async: #{e}"
end
```

#### Using the delete_schedule_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_schedule_async_with_http_info(tenant_id, schedule_id, opts)

```ruby
begin
  # Delete a schedule
  data, status_code, headers = api_instance.delete_schedule_async_with_http_info(tenant_id, schedule_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SchedulesApi->delete_schedule_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **schedule_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_schedule_by_id_async

> <ScheduleDtoEnvelope> get_schedule_by_id_async(tenant_id, schedule_id, opts)

Get schedule by ID

Retrieves a specific schedule by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SchedulesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
schedule_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get schedule by ID
  result = api_instance.get_schedule_by_id_async(tenant_id, schedule_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SchedulesApi->get_schedule_by_id_async: #{e}"
end
```

#### Using the get_schedule_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ScheduleDtoEnvelope>, Integer, Hash)> get_schedule_by_id_async_with_http_info(tenant_id, schedule_id, opts)

```ruby
begin
  # Get schedule by ID
  data, status_code, headers = api_instance.get_schedule_by_id_async_with_http_info(tenant_id, schedule_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ScheduleDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SchedulesApi->get_schedule_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **schedule_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ScheduleDtoEnvelope**](ScheduleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_schedules_async

> <ScheduleDtoListEnvelope> get_schedules_async(tenant_id, opts)

Get schedules

Retrieves schedules for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SchedulesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get schedules
  result = api_instance.get_schedules_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SchedulesApi->get_schedules_async: #{e}"
end
```

#### Using the get_schedules_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ScheduleDtoListEnvelope>, Integer, Hash)> get_schedules_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get schedules
  data, status_code, headers = api_instance.get_schedules_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ScheduleDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SchedulesApi->get_schedules_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ScheduleDtoListEnvelope**](ScheduleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_schedules_count_async

> <Int32Envelope> get_schedules_count_async(tenant_id, opts)

Count schedules

Counts schedules for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SchedulesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count schedules
  result = api_instance.get_schedules_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SchedulesApi->get_schedules_count_async: #{e}"
end
```

#### Using the get_schedules_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_schedules_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count schedules
  data, status_code, headers = api_instance.get_schedules_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SchedulesApi->get_schedules_count_async_with_http_info: #{e}"
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


## patch_schedule_async

> <EmptyEnvelope> patch_schedule_async(tenant_id, schedule_id, opts)

Patch a schedule

Partially updates an existing schedule for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SchedulesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
schedule_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a schedule
  result = api_instance.patch_schedule_async(tenant_id, schedule_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SchedulesApi->patch_schedule_async: #{e}"
end
```

#### Using the patch_schedule_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_schedule_async_with_http_info(tenant_id, schedule_id, opts)

```ruby
begin
  # Patch a schedule
  data, status_code, headers = api_instance.patch_schedule_async_with_http_info(tenant_id, schedule_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SchedulesApi->patch_schedule_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **schedule_id** | **String** |  |  |
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


## update_schedule_async

> <EmptyEnvelope> update_schedule_async(tenant_id, schedule_id, opts)

Update a schedule

Updates an existing schedule for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SchedulesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
schedule_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  schedule_update_dto: OpenapiClient::ScheduleUpdateDto.new # ScheduleUpdateDto | 
}

begin
  # Update a schedule
  result = api_instance.update_schedule_async(tenant_id, schedule_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SchedulesApi->update_schedule_async: #{e}"
end
```

#### Using the update_schedule_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_schedule_async_with_http_info(tenant_id, schedule_id, opts)

```ruby
begin
  # Update a schedule
  data, status_code, headers = api_instance.update_schedule_async_with_http_info(tenant_id, schedule_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SchedulesApi->update_schedule_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **schedule_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **schedule_update_dto** | [**ScheduleUpdateDto**](ScheduleUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

