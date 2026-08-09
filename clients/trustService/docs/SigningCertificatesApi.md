# OpenapiClient::SigningCertificatesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_signing_certificate_async**](SigningCertificatesApi.md#create_signing_certificate_async) | **POST** /api/v2/TrustService/SigningCertificates | Create a new signing certificate |
| [**delete_signing_certificate_async**](SigningCertificatesApi.md#delete_signing_certificate_async) | **DELETE** /api/v2/TrustService/SigningCertificates/{id} | Delete a signing certificate |
| [**get_signing_certificate_by_id_async**](SigningCertificatesApi.md#get_signing_certificate_by_id_async) | **GET** /api/v2/TrustService/SigningCertificates/{id} | Get signing certificate by ID |
| [**get_signing_certificates_async**](SigningCertificatesApi.md#get_signing_certificates_async) | **GET** /api/v2/TrustService/SigningCertificates | Get all signing certificates |
| [**get_signing_certificates_count_async**](SigningCertificatesApi.md#get_signing_certificates_count_async) | **GET** /api/v2/TrustService/SigningCertificates/Count | Get signing certificates count |
| [**import_signing_certificate_async**](SigningCertificatesApi.md#import_signing_certificate_async) | **POST** /api/v2/TrustService/SigningCertificates/Import | Import a PFX/P12 signing certificate into custody |
| [**patch_signing_certificate_async**](SigningCertificatesApi.md#patch_signing_certificate_async) | **PATCH** /api/v2/TrustService/SigningCertificates/{id} | Patch a signing certificate |
| [**update_signing_certificate_async**](SigningCertificatesApi.md#update_signing_certificate_async) | **PUT** /api/v2/TrustService/SigningCertificates/{id} | Update a signing certificate |


## create_signing_certificate_async

> create_signing_certificate_async(tenant_id, opts)

Create a new signing certificate

Creates a new signing certificate for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signing_certificate_create_dto: OpenapiClient::SigningCertificateCreateDto.new({title: 'title_example', contact_id: 'contact_id_example'}) # SigningCertificateCreateDto | 
}

begin
  # Create a new signing certificate
  api_instance.create_signing_certificate_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningCertificatesApi->create_signing_certificate_async: #{e}"
end
```

#### Using the create_signing_certificate_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_signing_certificate_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new signing certificate
  data, status_code, headers = api_instance.create_signing_certificate_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningCertificatesApi->create_signing_certificate_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signing_certificate_create_dto** | [**SigningCertificateCreateDto**](SigningCertificateCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_signing_certificate_async

> delete_signing_certificate_async(tenant_id, id, opts)

Delete a signing certificate

Deletes a signing certificate for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a signing certificate
  api_instance.delete_signing_certificate_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningCertificatesApi->delete_signing_certificate_async: #{e}"
end
```

#### Using the delete_signing_certificate_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_signing_certificate_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a signing certificate
  data, status_code, headers = api_instance.delete_signing_certificate_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningCertificatesApi->delete_signing_certificate_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_signing_certificate_by_id_async

> <SigningCertificateDto> get_signing_certificate_by_id_async(tenant_id, id, opts)

Get signing certificate by ID

Retrieves a specific signing certificate by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get signing certificate by ID
  result = api_instance.get_signing_certificate_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningCertificatesApi->get_signing_certificate_by_id_async: #{e}"
end
```

#### Using the get_signing_certificate_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SigningCertificateDto>, Integer, Hash)> get_signing_certificate_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get signing certificate by ID
  data, status_code, headers = api_instance.get_signing_certificate_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SigningCertificateDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningCertificatesApi->get_signing_certificate_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SigningCertificateDto**](SigningCertificateDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_signing_certificates_async

> <SigningCertificateDtoListEnvelope> get_signing_certificates_async(tenant_id, opts)

Get all signing certificates

Retrieves all signing certificates for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signing_certificate_dto_collection_query_parameters: OpenapiClient::SigningCertificateDtoCollectionQueryParameters.new # SigningCertificateDtoCollectionQueryParameters | 
}

begin
  # Get all signing certificates
  result = api_instance.get_signing_certificates_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningCertificatesApi->get_signing_certificates_async: #{e}"
end
```

#### Using the get_signing_certificates_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SigningCertificateDtoListEnvelope>, Integer, Hash)> get_signing_certificates_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all signing certificates
  data, status_code, headers = api_instance.get_signing_certificates_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SigningCertificateDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningCertificatesApi->get_signing_certificates_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signing_certificate_dto_collection_query_parameters** | [**SigningCertificateDtoCollectionQueryParameters**](SigningCertificateDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**SigningCertificateDtoListEnvelope**](SigningCertificateDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_signing_certificates_count_async

> <Int32Envelope> get_signing_certificates_count_async(tenant_id, opts)

Get signing certificates count

Returns the count of signing certificates for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signing_certificate_dto_collection_query_parameters: OpenapiClient::SigningCertificateDtoCollectionQueryParameters.new # SigningCertificateDtoCollectionQueryParameters | 
}

begin
  # Get signing certificates count
  result = api_instance.get_signing_certificates_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningCertificatesApi->get_signing_certificates_count_async: #{e}"
end
```

#### Using the get_signing_certificates_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_signing_certificates_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get signing certificates count
  data, status_code, headers = api_instance.get_signing_certificates_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningCertificatesApi->get_signing_certificates_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signing_certificate_dto_collection_query_parameters** | [**SigningCertificateDtoCollectionQueryParameters**](SigningCertificateDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## import_signing_certificate_async

> import_signing_certificate_async(tenant_id, opts)

Import a PFX/P12 signing certificate into custody

Parses the uploaded PFX/P12, imports the private material into the configured signing custody, and creates the certificate metadata record. The PFX and password are used only for the request — never returned or stored.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  file: File.new('/path/to/some/file'), # File | 
  password: 'password_example', # String | 
  title: 'title_example', # String | 
  contact_id: 'contact_id_example' # String | 
}

begin
  # Import a PFX/P12 signing certificate into custody
  api_instance.import_signing_certificate_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningCertificatesApi->import_signing_certificate_async: #{e}"
end
```

#### Using the import_signing_certificate_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> import_signing_certificate_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Import a PFX/P12 signing certificate into custody
  data, status_code, headers = api_instance.import_signing_certificate_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningCertificatesApi->import_signing_certificate_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **id** | **String** |  | [optional] |
| **file** | **File** |  | [optional] |
| **password** | **String** |  | [optional] |
| **title** | **String** |  | [optional] |
| **contact_id** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data, application/json, application/xml
- **Accept**: application/json, application/xml


## patch_signing_certificate_async

> <EmptyEnvelope> patch_signing_certificate_async(tenant_id, id, opts)

Patch a signing certificate

Patch a signing certificate

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a signing certificate
  result = api_instance.patch_signing_certificate_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningCertificatesApi->patch_signing_certificate_async: #{e}"
end
```

#### Using the patch_signing_certificate_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_signing_certificate_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a signing certificate
  data, status_code, headers = api_instance.patch_signing_certificate_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningCertificatesApi->patch_signing_certificate_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
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


## update_signing_certificate_async

> update_signing_certificate_async(tenant_id, id, opts)

Update a signing certificate

Updates an existing signing certificate for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signing_certificate_update_dto: OpenapiClient::SigningCertificateUpdateDto.new({title: 'title_example', contact_id: 'contact_id_example'}) # SigningCertificateUpdateDto | 
}

begin
  # Update a signing certificate
  api_instance.update_signing_certificate_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningCertificatesApi->update_signing_certificate_async: #{e}"
end
```

#### Using the update_signing_certificate_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_signing_certificate_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a signing certificate
  data, status_code, headers = api_instance.update_signing_certificate_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningCertificatesApi->update_signing_certificate_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signing_certificate_update_dto** | [**SigningCertificateUpdateDto**](SigningCertificateUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

