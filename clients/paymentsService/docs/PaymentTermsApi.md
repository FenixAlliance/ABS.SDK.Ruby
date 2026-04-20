# OpenapiClient::PaymentTermsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_payment_term_async**](PaymentTermsApi.md#create_payment_term_async) | **POST** /api/v2/PaymentsService/PaymentTerms | Creates a new payment term |
| [**delete_payment_term_async**](PaymentTermsApi.md#delete_payment_term_async) | **DELETE** /api/v2/PaymentsService/PaymentTerms/{paymentTermId} | Deletes a payment term |
| [**get_payment_term_details_async**](PaymentTermsApi.md#get_payment_term_details_async) | **GET** /api/v2/PaymentsService/PaymentTerms/{paymentTermId} | Gets a payment term by ID |
| [**get_payment_terms_async**](PaymentTermsApi.md#get_payment_terms_async) | **GET** /api/v2/PaymentsService/PaymentTerms | Retrieves all payment terms |
| [**get_payment_terms_count_async**](PaymentTermsApi.md#get_payment_terms_count_async) | **GET** /api/v2/PaymentsService/PaymentTerms/Count | Counts payment terms |
| [**update_payment_term_async**](PaymentTermsApi.md#update_payment_term_async) | **PUT** /api/v2/PaymentsService/PaymentTerms/{paymentTermId} | Updates a payment term |


## create_payment_term_async

> <EmptyEnvelope> create_payment_term_async(tenant_id, opts)

Creates a new payment term

Creates a new payment term for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentTermsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  payment_term_create_dto: OpenapiClient::PaymentTermCreateDto.new({name: 'name_example'}) # PaymentTermCreateDto | 
}

begin
  # Creates a new payment term
  result = api_instance.create_payment_term_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentTermsApi->create_payment_term_async: #{e}"
end
```

#### Using the create_payment_term_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_payment_term_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new payment term
  data, status_code, headers = api_instance.create_payment_term_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentTermsApi->create_payment_term_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **payment_term_create_dto** | [**PaymentTermCreateDto**](PaymentTermCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_payment_term_async

> <EmptyEnvelope> delete_payment_term_async(tenant_id, payment_term_id, opts)

Deletes a payment term

Deletes the specified payment term.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentTermsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_term_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes a payment term
  result = api_instance.delete_payment_term_async(tenant_id, payment_term_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentTermsApi->delete_payment_term_async: #{e}"
end
```

#### Using the delete_payment_term_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_payment_term_async_with_http_info(tenant_id, payment_term_id, opts)

```ruby
begin
  # Deletes a payment term
  data, status_code, headers = api_instance.delete_payment_term_async_with_http_info(tenant_id, payment_term_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentTermsApi->delete_payment_term_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_term_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payment_term_details_async

> <PaymentTermDtoEnvelope> get_payment_term_details_async(tenant_id, payment_term_id, opts)

Gets a payment term by ID

Retrieves the details of a payment term using its unique ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentTermsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_term_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets a payment term by ID
  result = api_instance.get_payment_term_details_async(tenant_id, payment_term_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentTermsApi->get_payment_term_details_async: #{e}"
end
```

#### Using the get_payment_term_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaymentTermDtoEnvelope>, Integer, Hash)> get_payment_term_details_async_with_http_info(tenant_id, payment_term_id, opts)

```ruby
begin
  # Gets a payment term by ID
  data, status_code, headers = api_instance.get_payment_term_details_async_with_http_info(tenant_id, payment_term_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaymentTermDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentTermsApi->get_payment_term_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_term_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PaymentTermDtoEnvelope**](PaymentTermDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payment_terms_async

> <PaymentTermDtoIReadOnlyListEnvelope> get_payment_terms_async(tenant_id, opts)

Retrieves all payment terms

Gets all payment terms for the current tenant with OData support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentTermsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieves all payment terms
  result = api_instance.get_payment_terms_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentTermsApi->get_payment_terms_async: #{e}"
end
```

#### Using the get_payment_terms_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaymentTermDtoIReadOnlyListEnvelope>, Integer, Hash)> get_payment_terms_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieves all payment terms
  data, status_code, headers = api_instance.get_payment_terms_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaymentTermDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentTermsApi->get_payment_terms_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PaymentTermDtoIReadOnlyListEnvelope**](PaymentTermDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payment_terms_count_async

> <Int32Envelope> get_payment_terms_count_async(tenant_id, opts)

Counts payment terms

Gets the count of payment terms for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentTermsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Counts payment terms
  result = api_instance.get_payment_terms_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentTermsApi->get_payment_terms_count_async: #{e}"
end
```

#### Using the get_payment_terms_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_payment_terms_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Counts payment terms
  data, status_code, headers = api_instance.get_payment_terms_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentTermsApi->get_payment_terms_count_async_with_http_info: #{e}"
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


## update_payment_term_async

> <EmptyEnvelope> update_payment_term_async(tenant_id, payment_term_id, opts)

Updates a payment term

Updates the specified payment term.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentTermsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_term_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  payment_term_update_dto: OpenapiClient::PaymentTermUpdateDto.new # PaymentTermUpdateDto | 
}

begin
  # Updates a payment term
  result = api_instance.update_payment_term_async(tenant_id, payment_term_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentTermsApi->update_payment_term_async: #{e}"
end
```

#### Using the update_payment_term_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_payment_term_async_with_http_info(tenant_id, payment_term_id, opts)

```ruby
begin
  # Updates a payment term
  data, status_code, headers = api_instance.update_payment_term_async_with_http_info(tenant_id, payment_term_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentTermsApi->update_payment_term_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_term_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **payment_term_update_dto** | [**PaymentTermUpdateDto**](PaymentTermUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

