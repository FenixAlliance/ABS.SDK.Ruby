# OpenapiClient::PaymentsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_payment_async**](PaymentsApi.md#create_payment_async) | **POST** /api/v2/PaymentsService/Payments | Creates a new payment |
| [**delete_payment_async**](PaymentsApi.md#delete_payment_async) | **DELETE** /api/v2/PaymentsService/Payments/{paymentId} | Deletes a payment |
| [**get_payment_async**](PaymentsApi.md#get_payment_async) | **GET** /api/v2/PaymentsService/Payments/{paymentId}/Details | Gets a payment by ID (deprecated) |
| [**get_payment_async_v2**](PaymentsApi.md#get_payment_async_v2) | **GET** /api/v2/PaymentsService/Payments/{paymentId} | Gets a payment by ID |
| [**get_payments_async**](PaymentsApi.md#get_payments_async) | **GET** /api/v2/PaymentsService/Payments | Retrieves all payments |
| [**update_payment_async**](PaymentsApi.md#update_payment_async) | **PUT** /api/v2/PaymentsService/Payments/{paymentId} | Updates a payment |


## create_payment_async

> <EmptyEnvelope> create_payment_async(tenant_id, opts)

Creates a new payment

Creates a new payment for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  payment_create_dto: OpenapiClient::PaymentCreateDto.new # PaymentCreateDto | 
}

begin
  # Creates a new payment
  result = api_instance.create_payment_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentsApi->create_payment_async: #{e}"
end
```

#### Using the create_payment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_payment_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new payment
  data, status_code, headers = api_instance.create_payment_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentsApi->create_payment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_create_dto** | [**PaymentCreateDto**](PaymentCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_payment_async

> <EmptyEnvelope> delete_payment_async(tenant_id, payment_id)

Deletes a payment

Deletes the specified payment.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes a payment
  result = api_instance.delete_payment_async(tenant_id, payment_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentsApi->delete_payment_async: #{e}"
end
```

#### Using the delete_payment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_payment_async_with_http_info(tenant_id, payment_id)

```ruby
begin
  # Deletes a payment
  data, status_code, headers = api_instance.delete_payment_async_with_http_info(tenant_id, payment_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentsApi->delete_payment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payment_async

> <PaymentDtoListEnvelope> get_payment_async(tenant_id, payment_id)

Gets a payment by ID (deprecated)

Retrieves a payment using the deprecated /Details route. Use GET {paymentId} instead.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a payment by ID (deprecated)
  result = api_instance.get_payment_async(tenant_id, payment_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentsApi->get_payment_async: #{e}"
end
```

#### Using the get_payment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaymentDtoListEnvelope>, Integer, Hash)> get_payment_async_with_http_info(tenant_id, payment_id)

```ruby
begin
  # Gets a payment by ID (deprecated)
  data, status_code, headers = api_instance.get_payment_async_with_http_info(tenant_id, payment_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaymentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentsApi->get_payment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_id** | **String** |  |  |

### Return type

[**PaymentDtoListEnvelope**](PaymentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payment_async_v2

> <PaymentDtoListEnvelope> get_payment_async_v2(tenant_id, payment_id)

Gets a payment by ID

Retrieves the details of a payment using its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a payment by ID
  result = api_instance.get_payment_async_v2(tenant_id, payment_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentsApi->get_payment_async_v2: #{e}"
end
```

#### Using the get_payment_async_v2_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaymentDtoListEnvelope>, Integer, Hash)> get_payment_async_v2_with_http_info(tenant_id, payment_id)

```ruby
begin
  # Gets a payment by ID
  data, status_code, headers = api_instance.get_payment_async_v2_with_http_info(tenant_id, payment_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaymentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentsApi->get_payment_async_v2_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_id** | **String** |  |  |

### Return type

[**PaymentDtoListEnvelope**](PaymentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payments_async

> <PaymentDtoListEnvelope> get_payments_async(tenant_id)

Retrieves all payments

Gets all payments for the current tenant with OData support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Retrieves all payments
  result = api_instance.get_payments_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentsApi->get_payments_async: #{e}"
end
```

#### Using the get_payments_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaymentDtoListEnvelope>, Integer, Hash)> get_payments_async_with_http_info(tenant_id)

```ruby
begin
  # Retrieves all payments
  data, status_code, headers = api_instance.get_payments_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaymentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentsApi->get_payments_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**PaymentDtoListEnvelope**](PaymentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_payment_async

> <EmptyEnvelope> update_payment_async(tenant_id, payment_id, opts)

Updates a payment

Updates the specified payment.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  payment_update_dto: OpenapiClient::PaymentUpdateDto.new # PaymentUpdateDto | 
}

begin
  # Updates a payment
  result = api_instance.update_payment_async(tenant_id, payment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentsApi->update_payment_async: #{e}"
end
```

#### Using the update_payment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_payment_async_with_http_info(tenant_id, payment_id, opts)

```ruby
begin
  # Updates a payment
  data, status_code, headers = api_instance.update_payment_async_with_http_info(tenant_id, payment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentsApi->update_payment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_id** | **String** |  |  |
| **payment_update_dto** | [**PaymentUpdateDto**](PaymentUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

