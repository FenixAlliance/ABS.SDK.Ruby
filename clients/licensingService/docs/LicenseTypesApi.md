# OpenapiClient::LicenseTypesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_license_type_async**](LicenseTypesApi.md#create_license_type_async) | **POST** /api/v2/LicensingService/LicenseTypes | Create a new license type |
| [**delete_license_type_async**](LicenseTypesApi.md#delete_license_type_async) | **DELETE** /api/v2/LicensingService/LicenseTypes/{id} | Delete a license type |
| [**get_license_type_by_id_async**](LicenseTypesApi.md#get_license_type_by_id_async) | **GET** /api/v2/LicensingService/LicenseTypes/{id} | Get license type by ID |
| [**get_license_types_async**](LicenseTypesApi.md#get_license_types_async) | **GET** /api/v2/LicensingService/LicenseTypes | Get all license types |
| [**get_license_types_count_async**](LicenseTypesApi.md#get_license_types_count_async) | **GET** /api/v2/LicensingService/LicenseTypes/Count | Get license types count |
| [**patch_license_type_async**](LicenseTypesApi.md#patch_license_type_async) | **PATCH** /api/v2/LicensingService/LicenseTypes/{id} | Patch a license type |
| [**update_license_type_async**](LicenseTypesApi.md#update_license_type_async) | **PUT** /api/v2/LicensingService/LicenseTypes/{id} | Update a license type |


## create_license_type_async

> create_license_type_async(tenant_id, opts)

Create a new license type

Creates a new license type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  license_type_create_dto: OpenapiClient::LicenseTypeCreateDto.new({title: 'title_example'}) # LicenseTypeCreateDto | 
}

begin
  # Create a new license type
  api_instance.create_license_type_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseTypesApi->create_license_type_async: #{e}"
end
```

#### Using the create_license_type_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_license_type_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new license type
  data, status_code, headers = api_instance.create_license_type_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseTypesApi->create_license_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **license_type_create_dto** | [**LicenseTypeCreateDto**](LicenseTypeCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_license_type_async

> delete_license_type_async(tenant_id, id, opts)

Delete a license type

Deletes a license type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a license type
  api_instance.delete_license_type_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseTypesApi->delete_license_type_async: #{e}"
end
```

#### Using the delete_license_type_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_license_type_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a license type
  data, status_code, headers = api_instance.delete_license_type_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseTypesApi->delete_license_type_async_with_http_info: #{e}"
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


## get_license_type_by_id_async

> <LicenseTypeDto> get_license_type_by_id_async(tenant_id, id, opts)

Get license type by ID

Retrieves a specific license type by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get license type by ID
  result = api_instance.get_license_type_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseTypesApi->get_license_type_by_id_async: #{e}"
end
```

#### Using the get_license_type_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LicenseTypeDto>, Integer, Hash)> get_license_type_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get license type by ID
  data, status_code, headers = api_instance.get_license_type_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LicenseTypeDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseTypesApi->get_license_type_by_id_async_with_http_info: #{e}"
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

[**LicenseTypeDto**](LicenseTypeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_license_types_async

> <LicenseTypeDtoListEnvelope> get_license_types_async(tenant_id, opts)

Get all license types

Retrieves all license types for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  license_type_dto_collection_query_parameters: OpenapiClient::LicenseTypeDtoCollectionQueryParameters.new # LicenseTypeDtoCollectionQueryParameters | 
}

begin
  # Get all license types
  result = api_instance.get_license_types_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseTypesApi->get_license_types_async: #{e}"
end
```

#### Using the get_license_types_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LicenseTypeDtoListEnvelope>, Integer, Hash)> get_license_types_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all license types
  data, status_code, headers = api_instance.get_license_types_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LicenseTypeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseTypesApi->get_license_types_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **license_type_dto_collection_query_parameters** | [**LicenseTypeDtoCollectionQueryParameters**](LicenseTypeDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**LicenseTypeDtoListEnvelope**](LicenseTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_license_types_count_async

> <Int32Envelope> get_license_types_count_async(tenant_id, opts)

Get license types count

Returns the count of license types for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  license_type_dto_collection_query_parameters: OpenapiClient::LicenseTypeDtoCollectionQueryParameters.new # LicenseTypeDtoCollectionQueryParameters | 
}

begin
  # Get license types count
  result = api_instance.get_license_types_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseTypesApi->get_license_types_count_async: #{e}"
end
```

#### Using the get_license_types_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_license_types_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get license types count
  data, status_code, headers = api_instance.get_license_types_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseTypesApi->get_license_types_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **license_type_dto_collection_query_parameters** | [**LicenseTypeDtoCollectionQueryParameters**](LicenseTypeDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_license_type_async

> <EmptyEnvelope> patch_license_type_async(tenant_id, id, opts)

Patch a license type

Patch a license type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a license type
  result = api_instance.patch_license_type_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseTypesApi->patch_license_type_async: #{e}"
end
```

#### Using the patch_license_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_license_type_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a license type
  data, status_code, headers = api_instance.patch_license_type_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseTypesApi->patch_license_type_async_with_http_info: #{e}"
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


## update_license_type_async

> update_license_type_async(tenant_id, id, opts)

Update a license type

Updates an existing license type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  license_type_update_dto: OpenapiClient::LicenseTypeUpdateDto.new # LicenseTypeUpdateDto | 
}

begin
  # Update a license type
  api_instance.update_license_type_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseTypesApi->update_license_type_async: #{e}"
end
```

#### Using the update_license_type_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_license_type_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a license type
  data, status_code, headers = api_instance.update_license_type_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseTypesApi->update_license_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **license_type_update_dto** | [**LicenseTypeUpdateDto**](LicenseTypeUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

