# OpenapiClient::LedgerTypesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_ledger_type_async**](LedgerTypesApi.md#create_ledger_type_async) | **POST** /api/v2/AccountingService/LedgerTypes | Creates a new ledger type |
| [**delete_ledger_type_async**](LedgerTypesApi.md#delete_ledger_type_async) | **DELETE** /api/v2/AccountingService/LedgerTypes/{ledgerTypeId} | Deletes a ledger type |
| [**get_ledger_type_details_async**](LedgerTypesApi.md#get_ledger_type_details_async) | **GET** /api/v2/AccountingService/LedgerTypes/{ledgerTypeId} | Gets a ledger type by ID |
| [**get_ledger_types_async**](LedgerTypesApi.md#get_ledger_types_async) | **GET** /api/v2/AccountingService/LedgerTypes | Retrieves all ledger types |
| [**get_ledger_types_count_async**](LedgerTypesApi.md#get_ledger_types_count_async) | **GET** /api/v2/AccountingService/LedgerTypes/Count | Counts ledger types |
| [**update_ledger_type_async**](LedgerTypesApi.md#update_ledger_type_async) | **PUT** /api/v2/AccountingService/LedgerTypes/{ledgerTypeId} | Updates a ledger type |


## create_ledger_type_async

> <EmptyEnvelope> create_ledger_type_async(tenant_id, opts)

Creates a new ledger type

Creates a new ledger type for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LedgerTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  ledger_type_create_dto: OpenapiClient::LedgerTypeCreateDto.new({name: 'name_example'}) # LedgerTypeCreateDto | 
}

begin
  # Creates a new ledger type
  result = api_instance.create_ledger_type_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgerTypesApi->create_ledger_type_async: #{e}"
end
```

#### Using the create_ledger_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_ledger_type_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new ledger type
  data, status_code, headers = api_instance.create_ledger_type_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgerTypesApi->create_ledger_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **ledger_type_create_dto** | [**LedgerTypeCreateDto**](LedgerTypeCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_ledger_type_async

> <EmptyEnvelope> delete_ledger_type_async(tenant_id, ledger_type_id, opts)

Deletes a ledger type

Deletes the specified ledger type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LedgerTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
ledger_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes a ledger type
  result = api_instance.delete_ledger_type_async(tenant_id, ledger_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgerTypesApi->delete_ledger_type_async: #{e}"
end
```

#### Using the delete_ledger_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_ledger_type_async_with_http_info(tenant_id, ledger_type_id, opts)

```ruby
begin
  # Deletes a ledger type
  data, status_code, headers = api_instance.delete_ledger_type_async_with_http_info(tenant_id, ledger_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgerTypesApi->delete_ledger_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **ledger_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_ledger_type_details_async

> <LedgerTypeDtoEnvelope> get_ledger_type_details_async(tenant_id, ledger_type_id, opts)

Gets a ledger type by ID

Retrieves the details of a ledger type using its unique ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LedgerTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
ledger_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets a ledger type by ID
  result = api_instance.get_ledger_type_details_async(tenant_id, ledger_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgerTypesApi->get_ledger_type_details_async: #{e}"
end
```

#### Using the get_ledger_type_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LedgerTypeDtoEnvelope>, Integer, Hash)> get_ledger_type_details_async_with_http_info(tenant_id, ledger_type_id, opts)

```ruby
begin
  # Gets a ledger type by ID
  data, status_code, headers = api_instance.get_ledger_type_details_async_with_http_info(tenant_id, ledger_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LedgerTypeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgerTypesApi->get_ledger_type_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **ledger_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**LedgerTypeDtoEnvelope**](LedgerTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_ledger_types_async

> <LedgerTypeDtoIReadOnlyListEnvelope> get_ledger_types_async(tenant_id, opts)

Retrieves all ledger types

Gets all ledger types for the current tenant with OData support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LedgerTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieves all ledger types
  result = api_instance.get_ledger_types_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgerTypesApi->get_ledger_types_async: #{e}"
end
```

#### Using the get_ledger_types_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LedgerTypeDtoIReadOnlyListEnvelope>, Integer, Hash)> get_ledger_types_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieves all ledger types
  data, status_code, headers = api_instance.get_ledger_types_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LedgerTypeDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgerTypesApi->get_ledger_types_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**LedgerTypeDtoIReadOnlyListEnvelope**](LedgerTypeDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_ledger_types_count_async

> <Int32Envelope> get_ledger_types_count_async(tenant_id, opts)

Counts ledger types

Gets the count of ledger types for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LedgerTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Counts ledger types
  result = api_instance.get_ledger_types_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgerTypesApi->get_ledger_types_count_async: #{e}"
end
```

#### Using the get_ledger_types_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_ledger_types_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Counts ledger types
  data, status_code, headers = api_instance.get_ledger_types_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgerTypesApi->get_ledger_types_count_async_with_http_info: #{e}"
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


## update_ledger_type_async

> <EmptyEnvelope> update_ledger_type_async(tenant_id, ledger_type_id, opts)

Updates a ledger type

Updates the specified ledger type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LedgerTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
ledger_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  ledger_type_update_dto: OpenapiClient::LedgerTypeUpdateDto.new # LedgerTypeUpdateDto | 
}

begin
  # Updates a ledger type
  result = api_instance.update_ledger_type_async(tenant_id, ledger_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgerTypesApi->update_ledger_type_async: #{e}"
end
```

#### Using the update_ledger_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_ledger_type_async_with_http_info(tenant_id, ledger_type_id, opts)

```ruby
begin
  # Updates a ledger type
  data, status_code, headers = api_instance.update_ledger_type_async_with_http_info(tenant_id, ledger_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgerTypesApi->update_ledger_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **ledger_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **ledger_type_update_dto** | [**LedgerTypeUpdateDto**](LedgerTypeUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

