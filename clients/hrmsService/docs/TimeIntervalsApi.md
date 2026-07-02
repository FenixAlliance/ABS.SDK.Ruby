# OpenapiClient::TimeIntervalsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_time_interval_async**](TimeIntervalsApi.md#create_time_interval_async) | **POST** /api/v2/HrmsService/TimeIntervals | Create a time interval |
| [**delete_time_interval_async**](TimeIntervalsApi.md#delete_time_interval_async) | **DELETE** /api/v2/HrmsService/TimeIntervals/{timeIntervalId} | Delete a time interval |
| [**get_time_interval_by_id_async**](TimeIntervalsApi.md#get_time_interval_by_id_async) | **GET** /api/v2/HrmsService/TimeIntervals/{timeIntervalId} | Get time interval by ID |
| [**get_time_intervals_async**](TimeIntervalsApi.md#get_time_intervals_async) | **GET** /api/v2/HrmsService/TimeIntervals | Get time intervals |
| [**get_time_intervals_count_async**](TimeIntervalsApi.md#get_time_intervals_count_async) | **GET** /api/v2/HrmsService/TimeIntervals/Count | Count time intervals |
| [**patch_time_interval_async**](TimeIntervalsApi.md#patch_time_interval_async) | **PATCH** /api/v2/HrmsService/TimeIntervals/{timeIntervalId} | Patch a time interval |
| [**update_time_interval_async**](TimeIntervalsApi.md#update_time_interval_async) | **PUT** /api/v2/HrmsService/TimeIntervals/{timeIntervalId} | Update a time interval |


## create_time_interval_async

> <EmptyEnvelope> create_time_interval_async(tenant_id, opts)

Create a time interval

Creates a new time interval for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeIntervalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  time_interval_create_dto: OpenapiClient::TimeIntervalCreateDto.new({title: 'title_example', schedule_id: 'schedule_id_example'}) # TimeIntervalCreateDto | 
}

begin
  # Create a time interval
  result = api_instance.create_time_interval_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeIntervalsApi->create_time_interval_async: #{e}"
end
```

#### Using the create_time_interval_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_time_interval_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a time interval
  data, status_code, headers = api_instance.create_time_interval_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeIntervalsApi->create_time_interval_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **time_interval_create_dto** | [**TimeIntervalCreateDto**](TimeIntervalCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_time_interval_async

> <EmptyEnvelope> delete_time_interval_async(tenant_id, time_interval_id, opts)

Delete a time interval

Deletes a time interval for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeIntervalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
time_interval_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a time interval
  result = api_instance.delete_time_interval_async(tenant_id, time_interval_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeIntervalsApi->delete_time_interval_async: #{e}"
end
```

#### Using the delete_time_interval_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_time_interval_async_with_http_info(tenant_id, time_interval_id, opts)

```ruby
begin
  # Delete a time interval
  data, status_code, headers = api_instance.delete_time_interval_async_with_http_info(tenant_id, time_interval_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeIntervalsApi->delete_time_interval_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **time_interval_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_time_interval_by_id_async

> <TimeIntervalDtoEnvelope> get_time_interval_by_id_async(tenant_id, time_interval_id, opts)

Get time interval by ID

Retrieves a specific time interval by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeIntervalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
time_interval_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get time interval by ID
  result = api_instance.get_time_interval_by_id_async(tenant_id, time_interval_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeIntervalsApi->get_time_interval_by_id_async: #{e}"
end
```

#### Using the get_time_interval_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TimeIntervalDtoEnvelope>, Integer, Hash)> get_time_interval_by_id_async_with_http_info(tenant_id, time_interval_id, opts)

```ruby
begin
  # Get time interval by ID
  data, status_code, headers = api_instance.get_time_interval_by_id_async_with_http_info(tenant_id, time_interval_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TimeIntervalDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeIntervalsApi->get_time_interval_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **time_interval_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TimeIntervalDtoEnvelope**](TimeIntervalDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_time_intervals_async

> <TimeIntervalDtoListEnvelope> get_time_intervals_async(tenant_id, opts)

Get time intervals

Retrieves time intervals for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeIntervalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get time intervals
  result = api_instance.get_time_intervals_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeIntervalsApi->get_time_intervals_async: #{e}"
end
```

#### Using the get_time_intervals_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TimeIntervalDtoListEnvelope>, Integer, Hash)> get_time_intervals_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get time intervals
  data, status_code, headers = api_instance.get_time_intervals_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TimeIntervalDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeIntervalsApi->get_time_intervals_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TimeIntervalDtoListEnvelope**](TimeIntervalDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_time_intervals_count_async

> <Int32Envelope> get_time_intervals_count_async(tenant_id, opts)

Count time intervals

Counts time intervals for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeIntervalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count time intervals
  result = api_instance.get_time_intervals_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeIntervalsApi->get_time_intervals_count_async: #{e}"
end
```

#### Using the get_time_intervals_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_time_intervals_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count time intervals
  data, status_code, headers = api_instance.get_time_intervals_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeIntervalsApi->get_time_intervals_count_async_with_http_info: #{e}"
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


## patch_time_interval_async

> <EmptyEnvelope> patch_time_interval_async(tenant_id, time_interval_id, opts)

Patch a time interval

Partially updates an existing time interval for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeIntervalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
time_interval_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a time interval
  result = api_instance.patch_time_interval_async(tenant_id, time_interval_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeIntervalsApi->patch_time_interval_async: #{e}"
end
```

#### Using the patch_time_interval_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_time_interval_async_with_http_info(tenant_id, time_interval_id, opts)

```ruby
begin
  # Patch a time interval
  data, status_code, headers = api_instance.patch_time_interval_async_with_http_info(tenant_id, time_interval_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeIntervalsApi->patch_time_interval_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **time_interval_id** | **String** |  |  |
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


## update_time_interval_async

> <EmptyEnvelope> update_time_interval_async(tenant_id, time_interval_id, opts)

Update a time interval

Updates an existing time interval for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimeIntervalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
time_interval_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  time_interval_update_dto: OpenapiClient::TimeIntervalUpdateDto.new # TimeIntervalUpdateDto | 
}

begin
  # Update a time interval
  result = api_instance.update_time_interval_async(tenant_id, time_interval_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeIntervalsApi->update_time_interval_async: #{e}"
end
```

#### Using the update_time_interval_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_time_interval_async_with_http_info(tenant_id, time_interval_id, opts)

```ruby
begin
  # Update a time interval
  data, status_code, headers = api_instance.update_time_interval_async_with_http_info(tenant_id, time_interval_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimeIntervalsApi->update_time_interval_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **time_interval_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **time_interval_update_dto** | [**TimeIntervalUpdateDto**](TimeIntervalUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

