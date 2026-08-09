# OpenapiClient::LicensingCertificatesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_licensing_certificate_async**](LicensingCertificatesApi.md#create_licensing_certificate_async) | **POST** /api/v2/LicensingService/LicensingCertificates | Create a new licensing certificate |
| [**delete_licensing_certificate_async**](LicensingCertificatesApi.md#delete_licensing_certificate_async) | **DELETE** /api/v2/LicensingService/LicensingCertificates/{id} | Delete a licensing certificate |
| [**get_licensing_certificate_by_id_async**](LicensingCertificatesApi.md#get_licensing_certificate_by_id_async) | **GET** /api/v2/LicensingService/LicensingCertificates/{id} | Get licensing certificate by ID |
| [**get_licensing_certificates_async**](LicensingCertificatesApi.md#get_licensing_certificates_async) | **GET** /api/v2/LicensingService/LicensingCertificates | Get all licensing certificates |
| [**get_licensing_certificates_count_async**](LicensingCertificatesApi.md#get_licensing_certificates_count_async) | **GET** /api/v2/LicensingService/LicensingCertificates/Count | Get licensing certificates count |
| [**patch_licensing_certificate_async**](LicensingCertificatesApi.md#patch_licensing_certificate_async) | **PATCH** /api/v2/LicensingService/LicensingCertificates/{id} | Patch a licensing certificate |
| [**update_licensing_certificate_async**](LicensingCertificatesApi.md#update_licensing_certificate_async) | **PUT** /api/v2/LicensingService/LicensingCertificates/{id} | Update a licensing certificate |


## create_licensing_certificate_async

> create_licensing_certificate_async(tenant_id, opts)

Create a new licensing certificate

Creates a new licensing certificate for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicensingCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  licensing_certificate_create_dto: OpenapiClient::LicensingCertificateCreateDto.new({contact_id: 'contact_id_example'}) # LicensingCertificateCreateDto | 
}

begin
  # Create a new licensing certificate
  api_instance.create_licensing_certificate_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensingCertificatesApi->create_licensing_certificate_async: #{e}"
end
```

#### Using the create_licensing_certificate_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_licensing_certificate_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new licensing certificate
  data, status_code, headers = api_instance.create_licensing_certificate_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensingCertificatesApi->create_licensing_certificate_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **licensing_certificate_create_dto** | [**LicensingCertificateCreateDto**](LicensingCertificateCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_licensing_certificate_async

> delete_licensing_certificate_async(tenant_id, id, opts)

Delete a licensing certificate

Deletes a licensing certificate for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicensingCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a licensing certificate
  api_instance.delete_licensing_certificate_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensingCertificatesApi->delete_licensing_certificate_async: #{e}"
end
```

#### Using the delete_licensing_certificate_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_licensing_certificate_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a licensing certificate
  data, status_code, headers = api_instance.delete_licensing_certificate_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensingCertificatesApi->delete_licensing_certificate_async_with_http_info: #{e}"
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


## get_licensing_certificate_by_id_async

> <LicensingCertificateDto> get_licensing_certificate_by_id_async(tenant_id, id, opts)

Get licensing certificate by ID

Retrieves a specific licensing certificate by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicensingCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get licensing certificate by ID
  result = api_instance.get_licensing_certificate_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensingCertificatesApi->get_licensing_certificate_by_id_async: #{e}"
end
```

#### Using the get_licensing_certificate_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LicensingCertificateDto>, Integer, Hash)> get_licensing_certificate_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get licensing certificate by ID
  data, status_code, headers = api_instance.get_licensing_certificate_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LicensingCertificateDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensingCertificatesApi->get_licensing_certificate_by_id_async_with_http_info: #{e}"
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

[**LicensingCertificateDto**](LicensingCertificateDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_licensing_certificates_async

> <LicensingCertificateDtoListEnvelope> get_licensing_certificates_async(tenant_id, opts)

Get all licensing certificates

Retrieves all licensing certificates for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicensingCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  licensing_certificate_dto_collection_query_parameters: OpenapiClient::LicensingCertificateDtoCollectionQueryParameters.new # LicensingCertificateDtoCollectionQueryParameters | 
}

begin
  # Get all licensing certificates
  result = api_instance.get_licensing_certificates_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensingCertificatesApi->get_licensing_certificates_async: #{e}"
end
```

#### Using the get_licensing_certificates_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LicensingCertificateDtoListEnvelope>, Integer, Hash)> get_licensing_certificates_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all licensing certificates
  data, status_code, headers = api_instance.get_licensing_certificates_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LicensingCertificateDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensingCertificatesApi->get_licensing_certificates_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **licensing_certificate_dto_collection_query_parameters** | [**LicensingCertificateDtoCollectionQueryParameters**](LicensingCertificateDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**LicensingCertificateDtoListEnvelope**](LicensingCertificateDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_licensing_certificates_count_async

> <Int32Envelope> get_licensing_certificates_count_async(tenant_id, opts)

Get licensing certificates count

Returns the count of licensing certificates for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicensingCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  licensing_certificate_dto_collection_query_parameters: OpenapiClient::LicensingCertificateDtoCollectionQueryParameters.new # LicensingCertificateDtoCollectionQueryParameters | 
}

begin
  # Get licensing certificates count
  result = api_instance.get_licensing_certificates_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensingCertificatesApi->get_licensing_certificates_count_async: #{e}"
end
```

#### Using the get_licensing_certificates_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_licensing_certificates_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get licensing certificates count
  data, status_code, headers = api_instance.get_licensing_certificates_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensingCertificatesApi->get_licensing_certificates_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **licensing_certificate_dto_collection_query_parameters** | [**LicensingCertificateDtoCollectionQueryParameters**](LicensingCertificateDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_licensing_certificate_async

> <EmptyEnvelope> patch_licensing_certificate_async(tenant_id, id, opts)

Patch a licensing certificate

Patch a licensing certificate for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicensingCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a licensing certificate
  result = api_instance.patch_licensing_certificate_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensingCertificatesApi->patch_licensing_certificate_async: #{e}"
end
```

#### Using the patch_licensing_certificate_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_licensing_certificate_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a licensing certificate
  data, status_code, headers = api_instance.patch_licensing_certificate_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensingCertificatesApi->patch_licensing_certificate_async_with_http_info: #{e}"
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


## update_licensing_certificate_async

> update_licensing_certificate_async(tenant_id, id, opts)

Update a licensing certificate

Updates an existing licensing certificate for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicensingCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  licensing_certificate_update_dto: OpenapiClient::LicensingCertificateUpdateDto.new # LicensingCertificateUpdateDto | 
}

begin
  # Update a licensing certificate
  api_instance.update_licensing_certificate_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensingCertificatesApi->update_licensing_certificate_async: #{e}"
end
```

#### Using the update_licensing_certificate_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_licensing_certificate_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a licensing certificate
  data, status_code, headers = api_instance.update_licensing_certificate_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensingCertificatesApi->update_licensing_certificate_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **licensing_certificate_update_dto** | [**LicensingCertificateUpdateDto**](LicensingCertificateUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

