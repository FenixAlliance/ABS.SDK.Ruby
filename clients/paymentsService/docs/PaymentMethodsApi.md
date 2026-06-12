# OpenapiClient::PaymentMethodsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_payment_method_async**](PaymentMethodsApi.md#create_payment_method_async) | **POST** /api/v2/PaymentsService/PaymentMethods | Creates a new payment method |
| [**delete_payment_method_async**](PaymentMethodsApi.md#delete_payment_method_async) | **DELETE** /api/v2/PaymentsService/PaymentMethods/{paymentMethodId} | Deletes a payment method |
| [**get_payment_method_details_async**](PaymentMethodsApi.md#get_payment_method_details_async) | **GET** /api/v2/PaymentsService/PaymentMethods/{paymentMethodId} | Gets a payment method by ID |
| [**get_payment_methods_async**](PaymentMethodsApi.md#get_payment_methods_async) | **GET** /api/v2/PaymentsService/PaymentMethods | Retrieves all payment methods |
| [**get_payment_methods_count_async**](PaymentMethodsApi.md#get_payment_methods_count_async) | **GET** /api/v2/PaymentsService/PaymentMethods/Count | Counts payment methods |
| [**patch_payment_method_async**](PaymentMethodsApi.md#patch_payment_method_async) | **PATCH** /api/v2/PaymentsService/PaymentMethods/{paymentMethodId} | Patch a payment method |
| [**update_payment_method_async**](PaymentMethodsApi.md#update_payment_method_async) | **PUT** /api/v2/PaymentsService/PaymentMethods/{paymentMethodId} | Updates a payment method |


## create_payment_method_async

> <EmptyEnvelope> create_payment_method_async(tenant_id, opts)

Creates a new payment method

Creates a new payment method for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentMethodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  payment_method_create_dto: OpenapiClient::PaymentMethodCreateDto.new({name: 'name_example'}) # PaymentMethodCreateDto | 
}

begin
  # Creates a new payment method
  result = api_instance.create_payment_method_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentMethodsApi->create_payment_method_async: #{e}"
end
```

#### Using the create_payment_method_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_payment_method_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new payment method
  data, status_code, headers = api_instance.create_payment_method_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentMethodsApi->create_payment_method_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **payment_method_create_dto** | [**PaymentMethodCreateDto**](PaymentMethodCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_payment_method_async

> <EmptyEnvelope> delete_payment_method_async(tenant_id, payment_method_id, opts)

Deletes a payment method

Deletes the specified payment method.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentMethodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_method_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes a payment method
  result = api_instance.delete_payment_method_async(tenant_id, payment_method_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentMethodsApi->delete_payment_method_async: #{e}"
end
```

#### Using the delete_payment_method_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_payment_method_async_with_http_info(tenant_id, payment_method_id, opts)

```ruby
begin
  # Deletes a payment method
  data, status_code, headers = api_instance.delete_payment_method_async_with_http_info(tenant_id, payment_method_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentMethodsApi->delete_payment_method_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_method_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payment_method_details_async

> <PaymentMethodDtoEnvelope> get_payment_method_details_async(tenant_id, payment_method_id, opts)

Gets a payment method by ID

Retrieves the details of a payment method using its unique ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentMethodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_method_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets a payment method by ID
  result = api_instance.get_payment_method_details_async(tenant_id, payment_method_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentMethodsApi->get_payment_method_details_async: #{e}"
end
```

#### Using the get_payment_method_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaymentMethodDtoEnvelope>, Integer, Hash)> get_payment_method_details_async_with_http_info(tenant_id, payment_method_id, opts)

```ruby
begin
  # Gets a payment method by ID
  data, status_code, headers = api_instance.get_payment_method_details_async_with_http_info(tenant_id, payment_method_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaymentMethodDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentMethodsApi->get_payment_method_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_method_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PaymentMethodDtoEnvelope**](PaymentMethodDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payment_methods_async

> <PaymentMethodDtoIReadOnlyListEnvelope> get_payment_methods_async(tenant_id, opts)

Retrieves all payment methods

Gets all payment methods for the current tenant with OData support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentMethodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieves all payment methods
  result = api_instance.get_payment_methods_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentMethodsApi->get_payment_methods_async: #{e}"
end
```

#### Using the get_payment_methods_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaymentMethodDtoIReadOnlyListEnvelope>, Integer, Hash)> get_payment_methods_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieves all payment methods
  data, status_code, headers = api_instance.get_payment_methods_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaymentMethodDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentMethodsApi->get_payment_methods_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PaymentMethodDtoIReadOnlyListEnvelope**](PaymentMethodDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payment_methods_count_async

> <Int32Envelope> get_payment_methods_count_async(tenant_id, opts)

Counts payment methods

Gets the count of payment methods for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentMethodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Counts payment methods
  result = api_instance.get_payment_methods_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentMethodsApi->get_payment_methods_count_async: #{e}"
end
```

#### Using the get_payment_methods_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_payment_methods_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Counts payment methods
  data, status_code, headers = api_instance.get_payment_methods_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentMethodsApi->get_payment_methods_count_async_with_http_info: #{e}"
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


## patch_payment_method_async

> <EmptyEnvelope> patch_payment_method_async(tenant_id, payment_method_id, opts)

Patch a payment method

Patch a payment method

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentMethodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_method_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a payment method
  result = api_instance.patch_payment_method_async(tenant_id, payment_method_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentMethodsApi->patch_payment_method_async: #{e}"
end
```

#### Using the patch_payment_method_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_payment_method_async_with_http_info(tenant_id, payment_method_id, opts)

```ruby
begin
  # Patch a payment method
  data, status_code, headers = api_instance.patch_payment_method_async_with_http_info(tenant_id, payment_method_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentMethodsApi->patch_payment_method_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_method_id** | **String** |  |  |
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


## update_payment_method_async

> <EmptyEnvelope> update_payment_method_async(tenant_id, payment_method_id, opts)

Updates a payment method

Updates the specified payment method.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentMethodsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_method_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  payment_method_update_dto: OpenapiClient::PaymentMethodUpdateDto.new # PaymentMethodUpdateDto | 
}

begin
  # Updates a payment method
  result = api_instance.update_payment_method_async(tenant_id, payment_method_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentMethodsApi->update_payment_method_async: #{e}"
end
```

#### Using the update_payment_method_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_payment_method_async_with_http_info(tenant_id, payment_method_id, opts)

```ruby
begin
  # Updates a payment method
  data, status_code, headers = api_instance.update_payment_method_async_with_http_info(tenant_id, payment_method_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentMethodsApi->update_payment_method_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_method_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **payment_method_update_dto** | [**PaymentMethodUpdateDto**](PaymentMethodUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

