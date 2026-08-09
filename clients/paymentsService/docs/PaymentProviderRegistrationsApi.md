# OpenapiClient::PaymentProviderRegistrationsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_async**](PaymentProviderRegistrationsApi.md#create_async) | **POST** /api/v2/PaymentsService/PaymentProviderRegistrations | Provisions a provider webhook registration |
| [**get_async**](PaymentProviderRegistrationsApi.md#get_async) | **GET** /api/v2/PaymentsService/PaymentProviderRegistrations | Lists the tenant&#39;s provider registrations |
| [**get_count_async**](PaymentProviderRegistrationsApi.md#get_count_async) | **GET** /api/v2/PaymentsService/PaymentProviderRegistrations/Count | Counts the tenant&#39;s provider registrations |
| [**rotate_key_async**](PaymentProviderRegistrationsApi.md#rotate_key_async) | **POST** /api/v2/PaymentsService/PaymentProviderRegistrations/{registrationId}/RotateKey | Rotates a registration&#39;s webhook key |


## create_async

> <ProviderWebhookRegistrationCreatedDtoEnvelope> create_async(tenant_id, opts)

Provisions a provider webhook registration

Stores the BYO signing secret in the tenant options store, creates + activates the registration, and reveals the one-time plaintext webhook key plus its fully-composed inbound URL.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentProviderRegistrationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  create_provider_webhook_registration_request: OpenapiClient::CreateProviderWebhookRegistrationRequest.new # CreateProviderWebhookRegistrationRequest | 
}

begin
  # Provisions a provider webhook registration
  result = api_instance.create_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentProviderRegistrationsApi->create_async: #{e}"
end
```

#### Using the create_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ProviderWebhookRegistrationCreatedDtoEnvelope>, Integer, Hash)> create_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Provisions a provider webhook registration
  data, status_code, headers = api_instance.create_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ProviderWebhookRegistrationCreatedDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentProviderRegistrationsApi->create_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **create_provider_webhook_registration_request** | [**CreateProviderWebhookRegistrationRequest**](CreateProviderWebhookRegistrationRequest.md) |  | [optional] |

### Return type

[**ProviderWebhookRegistrationCreatedDtoEnvelope**](ProviderWebhookRegistrationCreatedDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_async

> <PaymentProviderRegistrationDtoListEnvelope> get_async(tenant_id, opts)

Lists the tenant's provider registrations

Gets all provider registrations for the current tenant with OData support (no secret is ever returned).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentProviderRegistrationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  payment_provider_registration_dto_collection_query_parameters: OpenapiClient::PaymentProviderRegistrationDtoCollectionQueryParameters.new # PaymentProviderRegistrationDtoCollectionQueryParameters | 
}

begin
  # Lists the tenant's provider registrations
  result = api_instance.get_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentProviderRegistrationsApi->get_async: #{e}"
end
```

#### Using the get_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaymentProviderRegistrationDtoListEnvelope>, Integer, Hash)> get_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Lists the tenant's provider registrations
  data, status_code, headers = api_instance.get_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaymentProviderRegistrationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentProviderRegistrationsApi->get_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_provider_registration_dto_collection_query_parameters** | [**PaymentProviderRegistrationDtoCollectionQueryParameters**](PaymentProviderRegistrationDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**PaymentProviderRegistrationDtoListEnvelope**](PaymentProviderRegistrationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_count_async

> <Int32Envelope> get_count_async(tenant_id, opts)

Counts the tenant's provider registrations

Gets the count of provider registrations for the current tenant (OData sibling of the list).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentProviderRegistrationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  payment_provider_registration_dto_collection_query_parameters: OpenapiClient::PaymentProviderRegistrationDtoCollectionQueryParameters.new # PaymentProviderRegistrationDtoCollectionQueryParameters | 
}

begin
  # Counts the tenant's provider registrations
  result = api_instance.get_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentProviderRegistrationsApi->get_count_async: #{e}"
end
```

#### Using the get_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Counts the tenant's provider registrations
  data, status_code, headers = api_instance.get_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentProviderRegistrationsApi->get_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_provider_registration_dto_collection_query_parameters** | [**PaymentProviderRegistrationDtoCollectionQueryParameters**](PaymentProviderRegistrationDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## rotate_key_async

> <ProviderWebhookRegistrationCreatedDtoEnvelope> rotate_key_async(tenant_id, registration_id)

Rotates a registration's webhook key

Mints a fresh webhook key (invalidating the previous one) and reveals it once, plus its composed URL.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PaymentProviderRegistrationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
registration_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Rotates a registration's webhook key
  result = api_instance.rotate_key_async(tenant_id, registration_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentProviderRegistrationsApi->rotate_key_async: #{e}"
end
```

#### Using the rotate_key_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ProviderWebhookRegistrationCreatedDtoEnvelope>, Integer, Hash)> rotate_key_async_with_http_info(tenant_id, registration_id)

```ruby
begin
  # Rotates a registration's webhook key
  data, status_code, headers = api_instance.rotate_key_async_with_http_info(tenant_id, registration_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ProviderWebhookRegistrationCreatedDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PaymentProviderRegistrationsApi->rotate_key_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **registration_id** | **String** |  |  |

### Return type

[**ProviderWebhookRegistrationCreatedDtoEnvelope**](ProviderWebhookRegistrationCreatedDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

