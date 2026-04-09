# OpenapiClient::EmailSignaturesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_email_signature_async**](EmailSignaturesApi.md#create_email_signature_async) | **POST** /api/v2/MarketingService/EmailSignatures | Create an email signature |
| [**delete_email_signature_async**](EmailSignaturesApi.md#delete_email_signature_async) | **DELETE** /api/v2/MarketingService/EmailSignatures/{emailsignatureId} | Delete an email signature |
| [**get_email_signature_details_async**](EmailSignaturesApi.md#get_email_signature_details_async) | **GET** /api/v2/MarketingService/EmailSignatures/{emailsignatureId} | Get email signature by ID |
| [**get_email_signatures_count_async**](EmailSignaturesApi.md#get_email_signatures_count_async) | **GET** /api/v2/MarketingService/EmailSignatures/Count | Get email signatures count |
| [**get_email_signatures_o_data_async**](EmailSignaturesApi.md#get_email_signatures_o_data_async) | **GET** /api/v2/MarketingService/EmailSignatures | Get email signatures |
| [**update_email_signature_async**](EmailSignaturesApi.md#update_email_signature_async) | **PUT** /api/v2/MarketingService/EmailSignatures/{emailsignatureId} | Update an email signature |


## create_email_signature_async

> <EmptyEnvelope> create_email_signature_async(tenant_id, email_signature_create_dto, opts)

Create an email signature

Creates a new email signature for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailSignaturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
email_signature_create_dto = OpenapiClient::EmailSignatureCreateDto.new # EmailSignatureCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create an email signature
  result = api_instance.create_email_signature_async(tenant_id, email_signature_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailSignaturesApi->create_email_signature_async: #{e}"
end
```

#### Using the create_email_signature_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_email_signature_async_with_http_info(tenant_id, email_signature_create_dto, opts)

```ruby
begin
  # Create an email signature
  data, status_code, headers = api_instance.create_email_signature_async_with_http_info(tenant_id, email_signature_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailSignaturesApi->create_email_signature_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **email_signature_create_dto** | [**EmailSignatureCreateDto**](EmailSignatureCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_email_signature_async

> <EmptyEnvelope> delete_email_signature_async(tenant_id, emailsignature_id, opts)

Delete an email signature

Deletes an email signature by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailSignaturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
emailsignature_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an email signature
  result = api_instance.delete_email_signature_async(tenant_id, emailsignature_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailSignaturesApi->delete_email_signature_async: #{e}"
end
```

#### Using the delete_email_signature_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_email_signature_async_with_http_info(tenant_id, emailsignature_id, opts)

```ruby
begin
  # Delete an email signature
  data, status_code, headers = api_instance.delete_email_signature_async_with_http_info(tenant_id, emailsignature_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailSignaturesApi->delete_email_signature_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **emailsignature_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_email_signature_details_async

> <EmailSignatureDtoEnvelope> get_email_signature_details_async(tenant_id, emailsignature_id, opts)

Get email signature by ID

Retrieves the details of a specific email signature by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailSignaturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
emailsignature_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get email signature by ID
  result = api_instance.get_email_signature_details_async(tenant_id, emailsignature_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailSignaturesApi->get_email_signature_details_async: #{e}"
end
```

#### Using the get_email_signature_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmailSignatureDtoEnvelope>, Integer, Hash)> get_email_signature_details_async_with_http_info(tenant_id, emailsignature_id, opts)

```ruby
begin
  # Get email signature by ID
  data, status_code, headers = api_instance.get_email_signature_details_async_with_http_info(tenant_id, emailsignature_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmailSignatureDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailSignaturesApi->get_email_signature_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **emailsignature_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmailSignatureDtoEnvelope**](EmailSignatureDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_email_signatures_count_async

> <Int32Envelope> get_email_signatures_count_async(tenant_id, opts)

Get email signatures count

Returns the count of email signatures for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailSignaturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get email signatures count
  result = api_instance.get_email_signatures_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailSignaturesApi->get_email_signatures_count_async: #{e}"
end
```

#### Using the get_email_signatures_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_email_signatures_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get email signatures count
  data, status_code, headers = api_instance.get_email_signatures_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailSignaturesApi->get_email_signatures_count_async_with_http_info: #{e}"
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


## get_email_signatures_o_data_async

> <EmailSignatureDtoListEnvelope> get_email_signatures_o_data_async(tenant_id, opts)

Get email signatures

Retrieves a collection of email signatures for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailSignaturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get email signatures
  result = api_instance.get_email_signatures_o_data_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailSignaturesApi->get_email_signatures_o_data_async: #{e}"
end
```

#### Using the get_email_signatures_o_data_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmailSignatureDtoListEnvelope>, Integer, Hash)> get_email_signatures_o_data_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get email signatures
  data, status_code, headers = api_instance.get_email_signatures_o_data_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmailSignatureDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailSignaturesApi->get_email_signatures_o_data_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmailSignatureDtoListEnvelope**](EmailSignatureDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_email_signature_async

> <EmptyEnvelope> update_email_signature_async(tenant_id, emailsignature_id, email_signature_update_dto, opts)

Update an email signature

Updates an existing email signature by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailSignaturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
emailsignature_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
email_signature_update_dto = OpenapiClient::EmailSignatureUpdateDto.new # EmailSignatureUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update an email signature
  result = api_instance.update_email_signature_async(tenant_id, emailsignature_id, email_signature_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailSignaturesApi->update_email_signature_async: #{e}"
end
```

#### Using the update_email_signature_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_email_signature_async_with_http_info(tenant_id, emailsignature_id, email_signature_update_dto, opts)

```ruby
begin
  # Update an email signature
  data, status_code, headers = api_instance.update_email_signature_async_with_http_info(tenant_id, emailsignature_id, email_signature_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailSignaturesApi->update_email_signature_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **emailsignature_id** | **String** |  |  |
| **email_signature_update_dto** | [**EmailSignatureUpdateDto**](EmailSignatureUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

