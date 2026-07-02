# OpenapiClient::PaymentModesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_payment_mode_async**](PaymentModesApi.md#create_payment_mode_async) | **POST** /api/v2/PaymentsService/PaymentModes | Creates a new payment mode |
| [**delete_payment_mode_async**](PaymentModesApi.md#delete_payment_mode_async) | **DELETE** /api/v2/PaymentsService/PaymentModes/{paymentModeId} | Deletes a payment mode |
| [**get_payment_mode_details_async**](PaymentModesApi.md#get_payment_mode_details_async) | **GET** /api/v2/PaymentsService/PaymentModes/{paymentModeId} | Gets a payment mode by ID |
| [**get_payment_modes_async**](PaymentModesApi.md#get_payment_modes_async) | **GET** /api/v2/PaymentsService/PaymentModes | Retrieves all payment modes |
| [**get_payment_modes_count_async**](PaymentModesApi.md#get_payment_modes_count_async) | **GET** /api/v2/PaymentsService/PaymentModes/Count | Counts payment modes |
| [**patch_payment_mode_async**](PaymentModesApi.md#patch_payment_mode_async) | **PATCH** /api/v2/PaymentsService/PaymentModes/{paymentModeId} | Patch a payment mode |
| [**update_payment_mode_async**](PaymentModesApi.md#update_payment_mode_async) | **PUT** /api/v2/PaymentsService/PaymentModes/{paymentModeId} | Updates a payment mode |


## create_payment_mode_async

> <EmptyEnvelope> create_payment_mode_async(tenant_id, opts)

Creates a new payment mode

Creates a new payment mode for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentModesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  payment_mode_create_dto: OpenapiClient::PaymentModeCreateDto.new({name: 'name_example'}) # PaymentModeCreateDto | 
}

begin
  # Creates a new payment mode
  result = api_instance.create_payment_mode_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentModesApi->create_payment_mode_async: #{e}"
end
```

#### Using the create_payment_mode_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_payment_mode_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new payment mode
  data, status_code, headers = api_instance.create_payment_mode_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentModesApi->create_payment_mode_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **payment_mode_create_dto** | [**PaymentModeCreateDto**](PaymentModeCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_payment_mode_async

> <EmptyEnvelope> delete_payment_mode_async(tenant_id, payment_mode_id, opts)

Deletes a payment mode

Deletes the specified payment mode.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentModesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_mode_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes a payment mode
  result = api_instance.delete_payment_mode_async(tenant_id, payment_mode_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentModesApi->delete_payment_mode_async: #{e}"
end
```

#### Using the delete_payment_mode_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_payment_mode_async_with_http_info(tenant_id, payment_mode_id, opts)

```ruby
begin
  # Deletes a payment mode
  data, status_code, headers = api_instance.delete_payment_mode_async_with_http_info(tenant_id, payment_mode_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentModesApi->delete_payment_mode_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_mode_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payment_mode_details_async

> <PaymentModeDtoEnvelope> get_payment_mode_details_async(tenant_id, payment_mode_id, opts)

Gets a payment mode by ID

Retrieves the details of a payment mode using its unique ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentModesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_mode_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets a payment mode by ID
  result = api_instance.get_payment_mode_details_async(tenant_id, payment_mode_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentModesApi->get_payment_mode_details_async: #{e}"
end
```

#### Using the get_payment_mode_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaymentModeDtoEnvelope>, Integer, Hash)> get_payment_mode_details_async_with_http_info(tenant_id, payment_mode_id, opts)

```ruby
begin
  # Gets a payment mode by ID
  data, status_code, headers = api_instance.get_payment_mode_details_async_with_http_info(tenant_id, payment_mode_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaymentModeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentModesApi->get_payment_mode_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_mode_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PaymentModeDtoEnvelope**](PaymentModeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payment_modes_async

> <PaymentModeDtoIReadOnlyListEnvelope> get_payment_modes_async(tenant_id, opts)

Retrieves all payment modes

Gets all payment modes for the current tenant with OData support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentModesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieves all payment modes
  result = api_instance.get_payment_modes_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentModesApi->get_payment_modes_async: #{e}"
end
```

#### Using the get_payment_modes_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaymentModeDtoIReadOnlyListEnvelope>, Integer, Hash)> get_payment_modes_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieves all payment modes
  data, status_code, headers = api_instance.get_payment_modes_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaymentModeDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentModesApi->get_payment_modes_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PaymentModeDtoIReadOnlyListEnvelope**](PaymentModeDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payment_modes_count_async

> <Int32Envelope> get_payment_modes_count_async(tenant_id, opts)

Counts payment modes

Gets the count of payment modes for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentModesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Counts payment modes
  result = api_instance.get_payment_modes_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentModesApi->get_payment_modes_count_async: #{e}"
end
```

#### Using the get_payment_modes_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_payment_modes_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Counts payment modes
  data, status_code, headers = api_instance.get_payment_modes_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentModesApi->get_payment_modes_count_async_with_http_info: #{e}"
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


## patch_payment_mode_async

> <EmptyEnvelope> patch_payment_mode_async(tenant_id, payment_mode_id, opts)

Patch a payment mode

Patch a payment mode

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentModesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_mode_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a payment mode
  result = api_instance.patch_payment_mode_async(tenant_id, payment_mode_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentModesApi->patch_payment_mode_async: #{e}"
end
```

#### Using the patch_payment_mode_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_payment_mode_async_with_http_info(tenant_id, payment_mode_id, opts)

```ruby
begin
  # Patch a payment mode
  data, status_code, headers = api_instance.patch_payment_mode_async_with_http_info(tenant_id, payment_mode_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentModesApi->patch_payment_mode_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_mode_id** | **String** |  |  |
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


## update_payment_mode_async

> <EmptyEnvelope> update_payment_mode_async(tenant_id, payment_mode_id, opts)

Updates a payment mode

Updates the specified payment mode.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentModesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_mode_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  payment_mode_update_dto: OpenapiClient::PaymentModeUpdateDto.new # PaymentModeUpdateDto | 
}

begin
  # Updates a payment mode
  result = api_instance.update_payment_mode_async(tenant_id, payment_mode_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentModesApi->update_payment_mode_async: #{e}"
end
```

#### Using the update_payment_mode_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_payment_mode_async_with_http_info(tenant_id, payment_mode_id, opts)

```ruby
begin
  # Updates a payment mode
  data, status_code, headers = api_instance.update_payment_mode_async_with_http_info(tenant_id, payment_mode_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentModesApi->update_payment_mode_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_mode_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **payment_mode_update_dto** | [**PaymentModeUpdateDto**](PaymentModeUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

