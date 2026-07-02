# OpenapiClient::PayrollsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_payroll_async**](PayrollsApi.md#create_payroll_async) | **POST** /api/v2/HrmsService/Payrolls | Create a payroll |
| [**delete_payroll_async**](PayrollsApi.md#delete_payroll_async) | **DELETE** /api/v2/HrmsService/Payrolls/{payrollId} | Delete a payroll |
| [**get_payroll_by_id_async**](PayrollsApi.md#get_payroll_by_id_async) | **GET** /api/v2/HrmsService/Payrolls/{payrollId} | Get payroll by ID |
| [**get_payrolls_async**](PayrollsApi.md#get_payrolls_async) | **GET** /api/v2/HrmsService/Payrolls | Get payrolls |
| [**get_payrolls_count_async**](PayrollsApi.md#get_payrolls_count_async) | **GET** /api/v2/HrmsService/Payrolls/Count | Count payrolls |
| [**patch_payroll_async**](PayrollsApi.md#patch_payroll_async) | **PATCH** /api/v2/HrmsService/Payrolls/{payrollId} | Patch a payroll |
| [**update_payroll_async**](PayrollsApi.md#update_payroll_async) | **PUT** /api/v2/HrmsService/Payrolls/{payrollId} | Update a payroll |


## create_payroll_async

> <EmptyEnvelope> create_payroll_async(tenant_id, opts)

Create a payroll

Creates a new payroll for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PayrollsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  payroll_create_dto: OpenapiClient::PayrollCreateDto.new({payroll_period_id: 'payroll_period_id_example'}) # PayrollCreateDto | 
}

begin
  # Create a payroll
  result = api_instance.create_payroll_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollsApi->create_payroll_async: #{e}"
end
```

#### Using the create_payroll_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_payroll_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a payroll
  data, status_code, headers = api_instance.create_payroll_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollsApi->create_payroll_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **payroll_create_dto** | [**PayrollCreateDto**](PayrollCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_payroll_async

> <EmptyEnvelope> delete_payroll_async(tenant_id, payroll_id, opts)

Delete a payroll

Deletes a payroll for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PayrollsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payroll_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a payroll
  result = api_instance.delete_payroll_async(tenant_id, payroll_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollsApi->delete_payroll_async: #{e}"
end
```

#### Using the delete_payroll_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_payroll_async_with_http_info(tenant_id, payroll_id, opts)

```ruby
begin
  # Delete a payroll
  data, status_code, headers = api_instance.delete_payroll_async_with_http_info(tenant_id, payroll_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollsApi->delete_payroll_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payroll_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payroll_by_id_async

> <PayrollDtoEnvelope> get_payroll_by_id_async(tenant_id, payroll_id, opts)

Get payroll by ID

Retrieves a specific payroll by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PayrollsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payroll_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get payroll by ID
  result = api_instance.get_payroll_by_id_async(tenant_id, payroll_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollsApi->get_payroll_by_id_async: #{e}"
end
```

#### Using the get_payroll_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PayrollDtoEnvelope>, Integer, Hash)> get_payroll_by_id_async_with_http_info(tenant_id, payroll_id, opts)

```ruby
begin
  # Get payroll by ID
  data, status_code, headers = api_instance.get_payroll_by_id_async_with_http_info(tenant_id, payroll_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PayrollDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollsApi->get_payroll_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payroll_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PayrollDtoEnvelope**](PayrollDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payrolls_async

> <PayrollDtoListEnvelope> get_payrolls_async(tenant_id, opts)

Get payrolls

Retrieves payrolls for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PayrollsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get payrolls
  result = api_instance.get_payrolls_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollsApi->get_payrolls_async: #{e}"
end
```

#### Using the get_payrolls_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PayrollDtoListEnvelope>, Integer, Hash)> get_payrolls_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get payrolls
  data, status_code, headers = api_instance.get_payrolls_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PayrollDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollsApi->get_payrolls_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PayrollDtoListEnvelope**](PayrollDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payrolls_count_async

> <Int32Envelope> get_payrolls_count_async(tenant_id, opts)

Count payrolls

Counts payrolls for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PayrollsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count payrolls
  result = api_instance.get_payrolls_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollsApi->get_payrolls_count_async: #{e}"
end
```

#### Using the get_payrolls_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_payrolls_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count payrolls
  data, status_code, headers = api_instance.get_payrolls_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollsApi->get_payrolls_count_async_with_http_info: #{e}"
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


## patch_payroll_async

> <EmptyEnvelope> patch_payroll_async(tenant_id, payroll_id, opts)

Patch a payroll

Partially updates an existing payroll for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PayrollsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payroll_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a payroll
  result = api_instance.patch_payroll_async(tenant_id, payroll_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollsApi->patch_payroll_async: #{e}"
end
```

#### Using the patch_payroll_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_payroll_async_with_http_info(tenant_id, payroll_id, opts)

```ruby
begin
  # Patch a payroll
  data, status_code, headers = api_instance.patch_payroll_async_with_http_info(tenant_id, payroll_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollsApi->patch_payroll_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payroll_id** | **String** |  |  |
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


## update_payroll_async

> <EmptyEnvelope> update_payroll_async(tenant_id, payroll_id, opts)

Update a payroll

Updates an existing payroll for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PayrollsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payroll_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  payroll_update_dto: OpenapiClient::PayrollUpdateDto.new # PayrollUpdateDto | 
}

begin
  # Update a payroll
  result = api_instance.update_payroll_async(tenant_id, payroll_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollsApi->update_payroll_async: #{e}"
end
```

#### Using the update_payroll_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_payroll_async_with_http_info(tenant_id, payroll_id, opts)

```ruby
begin
  # Update a payroll
  data, status_code, headers = api_instance.update_payroll_async_with_http_info(tenant_id, payroll_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PayrollsApi->update_payroll_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payroll_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **payroll_update_dto** | [**PayrollUpdateDto**](PayrollUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

