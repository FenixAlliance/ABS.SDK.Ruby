# OpenapiClient::FiscalIdentificationTypesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_fiscal_identification_type**](FiscalIdentificationTypesApi.md#create_fiscal_identification_type) | **POST** /api/v2/AccountingService/Fiscals/Authorities/IdentificationTypes | Create a fiscal identification type |
| [**delete_fiscal_identification_type**](FiscalIdentificationTypesApi.md#delete_fiscal_identification_type) | **DELETE** /api/v2/AccountingService/Fiscals/Authorities/IdentificationTypes/{identificationTypeId} | Delete a fiscal identification type |
| [**get_fiscal_identification_type**](FiscalIdentificationTypesApi.md#get_fiscal_identification_type) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/IdentificationTypes/{identificationTypeId} | Get fiscal identification type by ID |
| [**get_fiscal_identification_types**](FiscalIdentificationTypesApi.md#get_fiscal_identification_types) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{authorityId}/IdentificationTypes | Get fiscal identification types for an authority |
| [**get_fiscal_identification_types_count**](FiscalIdentificationTypesApi.md#get_fiscal_identification_types_count) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{authorityId}/IdentificationTypes/Count | Get fiscal identification types count |
| [**patch_fiscal_identification_type_async**](FiscalIdentificationTypesApi.md#patch_fiscal_identification_type_async) | **PATCH** /api/v2/AccountingService/Fiscals/Authorities/IdentificationTypes/{identificationTypeId} | Patch a fiscal identification type |
| [**update_fiscal_identification_type**](FiscalIdentificationTypesApi.md#update_fiscal_identification_type) | **PUT** /api/v2/AccountingService/Fiscals/Authorities/IdentificationTypes/{identificationTypeId} | Update a fiscal identification type |


## create_fiscal_identification_type

> <EmptyEnvelope> create_fiscal_identification_type(tenant_id, opts)

Create a fiscal identification type

Creates a new fiscal identification type for a fiscal authority.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalIdentificationTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  fiscal_identification_type_create_dto: OpenapiClient::FiscalIdentificationTypeCreateDto.new # FiscalIdentificationTypeCreateDto | 
}

begin
  # Create a fiscal identification type
  result = api_instance.create_fiscal_identification_type(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalIdentificationTypesApi->create_fiscal_identification_type: #{e}"
end
```

#### Using the create_fiscal_identification_type_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_fiscal_identification_type_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a fiscal identification type
  data, status_code, headers = api_instance.create_fiscal_identification_type_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalIdentificationTypesApi->create_fiscal_identification_type_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **fiscal_identification_type_create_dto** | [**FiscalIdentificationTypeCreateDto**](FiscalIdentificationTypeCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_fiscal_identification_type

> <EmptyEnvelope> delete_fiscal_identification_type(tenant_id, identification_type_id, opts)

Delete a fiscal identification type

Deletes a fiscal identification type identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalIdentificationTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
identification_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a fiscal identification type
  result = api_instance.delete_fiscal_identification_type(tenant_id, identification_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalIdentificationTypesApi->delete_fiscal_identification_type: #{e}"
end
```

#### Using the delete_fiscal_identification_type_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_fiscal_identification_type_with_http_info(tenant_id, identification_type_id, opts)

```ruby
begin
  # Delete a fiscal identification type
  data, status_code, headers = api_instance.delete_fiscal_identification_type_with_http_info(tenant_id, identification_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalIdentificationTypesApi->delete_fiscal_identification_type_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **identification_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_identification_type

> <FiscalIdentificationTypeDtoEnvelope> get_fiscal_identification_type(tenant_id, fiscal_authority_id, identification_type_id, opts)

Get fiscal identification type by ID

Retrieves a specific fiscal identification type by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalIdentificationTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
identification_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal identification type by ID
  result = api_instance.get_fiscal_identification_type(tenant_id, fiscal_authority_id, identification_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalIdentificationTypesApi->get_fiscal_identification_type: #{e}"
end
```

#### Using the get_fiscal_identification_type_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FiscalIdentificationTypeDtoEnvelope>, Integer, Hash)> get_fiscal_identification_type_with_http_info(tenant_id, fiscal_authority_id, identification_type_id, opts)

```ruby
begin
  # Get fiscal identification type by ID
  data, status_code, headers = api_instance.get_fiscal_identification_type_with_http_info(tenant_id, fiscal_authority_id, identification_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FiscalIdentificationTypeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalIdentificationTypesApi->get_fiscal_identification_type_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_authority_id** | **String** |  |  |
| **identification_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**FiscalIdentificationTypeDtoEnvelope**](FiscalIdentificationTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_identification_types

> <FiscalIdentificationTypeDtoListEnvelope> get_fiscal_identification_types(tenant_id, authority_id, opts)

Get fiscal identification types for an authority

Retrieves all fiscal identification types for the specified fiscal authority.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalIdentificationTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  fiscal_identification_type_dto_collection_query_parameters: OpenapiClient::FiscalIdentificationTypeDtoCollectionQueryParameters.new # FiscalIdentificationTypeDtoCollectionQueryParameters | 
}

begin
  # Get fiscal identification types for an authority
  result = api_instance.get_fiscal_identification_types(tenant_id, authority_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalIdentificationTypesApi->get_fiscal_identification_types: #{e}"
end
```

#### Using the get_fiscal_identification_types_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FiscalIdentificationTypeDtoListEnvelope>, Integer, Hash)> get_fiscal_identification_types_with_http_info(tenant_id, authority_id, opts)

```ruby
begin
  # Get fiscal identification types for an authority
  data, status_code, headers = api_instance.get_fiscal_identification_types_with_http_info(tenant_id, authority_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FiscalIdentificationTypeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalIdentificationTypesApi->get_fiscal_identification_types_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **authority_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **fiscal_identification_type_dto_collection_query_parameters** | [**FiscalIdentificationTypeDtoCollectionQueryParameters**](FiscalIdentificationTypeDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**FiscalIdentificationTypeDtoListEnvelope**](FiscalIdentificationTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_fiscal_identification_types_count

> <Int32Envelope> get_fiscal_identification_types_count(tenant_id, authority_id, opts)

Get fiscal identification types count

Returns the total count of fiscal identification types for the specified fiscal authority.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalIdentificationTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  fiscal_identification_type_dto_collection_query_parameters: OpenapiClient::FiscalIdentificationTypeDtoCollectionQueryParameters.new # FiscalIdentificationTypeDtoCollectionQueryParameters | 
}

begin
  # Get fiscal identification types count
  result = api_instance.get_fiscal_identification_types_count(tenant_id, authority_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalIdentificationTypesApi->get_fiscal_identification_types_count: #{e}"
end
```

#### Using the get_fiscal_identification_types_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_fiscal_identification_types_count_with_http_info(tenant_id, authority_id, opts)

```ruby
begin
  # Get fiscal identification types count
  data, status_code, headers = api_instance.get_fiscal_identification_types_count_with_http_info(tenant_id, authority_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalIdentificationTypesApi->get_fiscal_identification_types_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **authority_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **fiscal_identification_type_dto_collection_query_parameters** | [**FiscalIdentificationTypeDtoCollectionQueryParameters**](FiscalIdentificationTypeDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_fiscal_identification_type_async

> <EmptyEnvelope> patch_fiscal_identification_type_async(tenant_id, identification_type_id, opts)

Patch a fiscal identification type

Partially updates a fiscal identification type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalIdentificationTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
identification_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a fiscal identification type
  result = api_instance.patch_fiscal_identification_type_async(tenant_id, identification_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalIdentificationTypesApi->patch_fiscal_identification_type_async: #{e}"
end
```

#### Using the patch_fiscal_identification_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_fiscal_identification_type_async_with_http_info(tenant_id, identification_type_id, opts)

```ruby
begin
  # Patch a fiscal identification type
  data, status_code, headers = api_instance.patch_fiscal_identification_type_async_with_http_info(tenant_id, identification_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalIdentificationTypesApi->patch_fiscal_identification_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **identification_type_id** | **String** |  |  |
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


## update_fiscal_identification_type

> <EmptyEnvelope> update_fiscal_identification_type(tenant_id, identification_type_id, opts)

Update a fiscal identification type

Updates an existing fiscal identification type identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalIdentificationTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
identification_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  fiscal_identification_type_update_dto: OpenapiClient::FiscalIdentificationTypeUpdateDto.new # FiscalIdentificationTypeUpdateDto | 
}

begin
  # Update a fiscal identification type
  result = api_instance.update_fiscal_identification_type(tenant_id, identification_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalIdentificationTypesApi->update_fiscal_identification_type: #{e}"
end
```

#### Using the update_fiscal_identification_type_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_fiscal_identification_type_with_http_info(tenant_id, identification_type_id, opts)

```ruby
begin
  # Update a fiscal identification type
  data, status_code, headers = api_instance.update_fiscal_identification_type_with_http_info(tenant_id, identification_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalIdentificationTypesApi->update_fiscal_identification_type_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **identification_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **fiscal_identification_type_update_dto** | [**FiscalIdentificationTypeUpdateDto**](FiscalIdentificationTypeUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

