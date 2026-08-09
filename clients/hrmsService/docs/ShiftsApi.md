# OpenapiClient::ShiftsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_shift_async**](ShiftsApi.md#create_shift_async) | **POST** /api/v2/HrmsService/Shifts | Create a shift |
| [**delete_shift_async**](ShiftsApi.md#delete_shift_async) | **DELETE** /api/v2/HrmsService/Shifts/{shiftId} | Delete a shift |
| [**get_shift_by_id_async**](ShiftsApi.md#get_shift_by_id_async) | **GET** /api/v2/HrmsService/Shifts/{shiftId} | Get shift by ID |
| [**get_shifts_async**](ShiftsApi.md#get_shifts_async) | **GET** /api/v2/HrmsService/Shifts | Get shifts |
| [**get_shifts_count_async**](ShiftsApi.md#get_shifts_count_async) | **GET** /api/v2/HrmsService/Shifts/Count | Count shifts |
| [**patch_shift_async**](ShiftsApi.md#patch_shift_async) | **PATCH** /api/v2/HrmsService/Shifts/{shiftId} | Patch a shift |
| [**update_shift_async**](ShiftsApi.md#update_shift_async) | **PUT** /api/v2/HrmsService/Shifts/{shiftId} | Update a shift |


## create_shift_async

> <EmptyEnvelope> create_shift_async(tenant_id, opts)

Create a shift

Creates a new shift for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShiftsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shift_create_dto: OpenapiClient::ShiftCreateDto.new({title: 'title_example', start: Time.now, _end: Time.now, employee_profile_id: 'employee_profile_id_example'}) # ShiftCreateDto | 
}

begin
  # Create a shift
  result = api_instance.create_shift_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShiftsApi->create_shift_async: #{e}"
end
```

#### Using the create_shift_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_shift_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a shift
  data, status_code, headers = api_instance.create_shift_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShiftsApi->create_shift_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shift_create_dto** | [**ShiftCreateDto**](ShiftCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_shift_async

> <EmptyEnvelope> delete_shift_async(tenant_id, shift_id, opts)

Delete a shift

Deletes a shift for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShiftsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
shift_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a shift
  result = api_instance.delete_shift_async(tenant_id, shift_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShiftsApi->delete_shift_async: #{e}"
end
```

#### Using the delete_shift_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_shift_async_with_http_info(tenant_id, shift_id, opts)

```ruby
begin
  # Delete a shift
  data, status_code, headers = api_instance.delete_shift_async_with_http_info(tenant_id, shift_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShiftsApi->delete_shift_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **shift_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shift_by_id_async

> <ShiftDtoEnvelope> get_shift_by_id_async(tenant_id, shift_id, opts)

Get shift by ID

Retrieves a specific shift by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShiftsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
shift_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get shift by ID
  result = api_instance.get_shift_by_id_async(tenant_id, shift_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShiftsApi->get_shift_by_id_async: #{e}"
end
```

#### Using the get_shift_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShiftDtoEnvelope>, Integer, Hash)> get_shift_by_id_async_with_http_info(tenant_id, shift_id, opts)

```ruby
begin
  # Get shift by ID
  data, status_code, headers = api_instance.get_shift_by_id_async_with_http_info(tenant_id, shift_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShiftDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShiftsApi->get_shift_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **shift_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShiftDtoEnvelope**](ShiftDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_shifts_async

> <ShiftDtoListEnvelope> get_shifts_async(tenant_id, opts)

Get shifts

Retrieves shifts for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShiftsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shift_dto_collection_query_parameters: OpenapiClient::ShiftDtoCollectionQueryParameters.new # ShiftDtoCollectionQueryParameters | 
}

begin
  # Get shifts
  result = api_instance.get_shifts_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShiftsApi->get_shifts_async: #{e}"
end
```

#### Using the get_shifts_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShiftDtoListEnvelope>, Integer, Hash)> get_shifts_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get shifts
  data, status_code, headers = api_instance.get_shifts_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShiftDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShiftsApi->get_shifts_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shift_dto_collection_query_parameters** | [**ShiftDtoCollectionQueryParameters**](ShiftDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ShiftDtoListEnvelope**](ShiftDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_shifts_count_async

> <Int32Envelope> get_shifts_count_async(tenant_id, opts)

Count shifts

Counts shifts for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShiftsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shift_dto_collection_query_parameters: OpenapiClient::ShiftDtoCollectionQueryParameters.new # ShiftDtoCollectionQueryParameters | 
}

begin
  # Count shifts
  result = api_instance.get_shifts_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShiftsApi->get_shifts_count_async: #{e}"
end
```

#### Using the get_shifts_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_shifts_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count shifts
  data, status_code, headers = api_instance.get_shifts_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShiftsApi->get_shifts_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shift_dto_collection_query_parameters** | [**ShiftDtoCollectionQueryParameters**](ShiftDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_shift_async

> <EmptyEnvelope> patch_shift_async(tenant_id, shift_id, opts)

Patch a shift

Partially updates an existing shift for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShiftsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
shift_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a shift
  result = api_instance.patch_shift_async(tenant_id, shift_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShiftsApi->patch_shift_async: #{e}"
end
```

#### Using the patch_shift_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_shift_async_with_http_info(tenant_id, shift_id, opts)

```ruby
begin
  # Patch a shift
  data, status_code, headers = api_instance.patch_shift_async_with_http_info(tenant_id, shift_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShiftsApi->patch_shift_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **shift_id** | **String** |  |  |
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


## update_shift_async

> <EmptyEnvelope> update_shift_async(tenant_id, shift_id, opts)

Update a shift

Updates an existing shift for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ShiftsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
shift_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  shift_update_dto: OpenapiClient::ShiftUpdateDto.new # ShiftUpdateDto | 
}

begin
  # Update a shift
  result = api_instance.update_shift_async(tenant_id, shift_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShiftsApi->update_shift_async: #{e}"
end
```

#### Using the update_shift_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_shift_async_with_http_info(tenant_id, shift_id, opts)

```ruby
begin
  # Update a shift
  data, status_code, headers = api_instance.update_shift_async_with_http_info(tenant_id, shift_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ShiftsApi->update_shift_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **shift_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **shift_update_dto** | [**ShiftUpdateDto**](ShiftUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

