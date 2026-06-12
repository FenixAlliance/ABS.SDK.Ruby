# OpenapiClient::LedgersApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_ledger_async**](LedgersApi.md#create_ledger_async) | **POST** /api/v2/AccountingService/Ledgers | Creates a new ledger |
| [**delete_ledger_async**](LedgersApi.md#delete_ledger_async) | **DELETE** /api/v2/AccountingService/Ledgers/{ledgerId} | Deletes a ledger |
| [**get_ledger_details_async**](LedgersApi.md#get_ledger_details_async) | **GET** /api/v2/AccountingService/Ledgers/{ledgerId} | Gets a ledger by ID |
| [**get_ledgers_async**](LedgersApi.md#get_ledgers_async) | **GET** /api/v2/AccountingService/Ledgers | Retrieves all ledgers |
| [**get_ledgers_count_async**](LedgersApi.md#get_ledgers_count_async) | **GET** /api/v2/AccountingService/Ledgers/Count | Counts ledgers |
| [**patch_ledger_async**](LedgersApi.md#patch_ledger_async) | **PATCH** /api/v2/AccountingService/Ledgers/{ledgerId} | Patches a ledger |
| [**update_ledger_async**](LedgersApi.md#update_ledger_async) | **PUT** /api/v2/AccountingService/Ledgers/{ledgerId} | Updates a ledger |


## create_ledger_async

> <EmptyEnvelope> create_ledger_async(tenant_id, opts)

Creates a new ledger

Creates a new ledger for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LedgersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  create_ledger_dto: OpenapiClient::CreateLedgerDto.new # CreateLedgerDto | 
}

begin
  # Creates a new ledger
  result = api_instance.create_ledger_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgersApi->create_ledger_async: #{e}"
end
```

#### Using the create_ledger_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_ledger_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new ledger
  data, status_code, headers = api_instance.create_ledger_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgersApi->create_ledger_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **create_ledger_dto** | [**CreateLedgerDto**](CreateLedgerDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_ledger_async

> <EmptyEnvelope> delete_ledger_async(tenant_id, ledger_id, opts)

Deletes a ledger

Deletes the specified ledger.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LedgersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
ledger_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes a ledger
  result = api_instance.delete_ledger_async(tenant_id, ledger_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgersApi->delete_ledger_async: #{e}"
end
```

#### Using the delete_ledger_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_ledger_async_with_http_info(tenant_id, ledger_id, opts)

```ruby
begin
  # Deletes a ledger
  data, status_code, headers = api_instance.delete_ledger_async_with_http_info(tenant_id, ledger_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgersApi->delete_ledger_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **ledger_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_ledger_details_async

> <LedgerDtoEnvelope> get_ledger_details_async(tenant_id, ledger_id, opts)

Gets a ledger by ID

Retrieves the details of a ledger using its unique ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LedgersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
ledger_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets a ledger by ID
  result = api_instance.get_ledger_details_async(tenant_id, ledger_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgersApi->get_ledger_details_async: #{e}"
end
```

#### Using the get_ledger_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LedgerDtoEnvelope>, Integer, Hash)> get_ledger_details_async_with_http_info(tenant_id, ledger_id, opts)

```ruby
begin
  # Gets a ledger by ID
  data, status_code, headers = api_instance.get_ledger_details_async_with_http_info(tenant_id, ledger_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LedgerDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgersApi->get_ledger_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **ledger_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**LedgerDtoEnvelope**](LedgerDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_ledgers_async

> <LedgerDtoIReadOnlyListEnvelope> get_ledgers_async(tenant_id, opts)

Retrieves all ledgers

Gets all ledgers for the current tenant with OData support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LedgersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieves all ledgers
  result = api_instance.get_ledgers_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgersApi->get_ledgers_async: #{e}"
end
```

#### Using the get_ledgers_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LedgerDtoIReadOnlyListEnvelope>, Integer, Hash)> get_ledgers_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieves all ledgers
  data, status_code, headers = api_instance.get_ledgers_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LedgerDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgersApi->get_ledgers_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**LedgerDtoIReadOnlyListEnvelope**](LedgerDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_ledgers_count_async

> <Int32Envelope> get_ledgers_count_async(tenant_id, opts)

Counts ledgers

Gets the count of ledgers for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LedgersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Counts ledgers
  result = api_instance.get_ledgers_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgersApi->get_ledgers_count_async: #{e}"
end
```

#### Using the get_ledgers_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_ledgers_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Counts ledgers
  data, status_code, headers = api_instance.get_ledgers_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgersApi->get_ledgers_count_async_with_http_info: #{e}"
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


## patch_ledger_async

> <EmptyEnvelope> patch_ledger_async(tenant_id, ledger_id, opts)

Patches a ledger

Patches the specified ledger.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LedgersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
ledger_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patches a ledger
  result = api_instance.patch_ledger_async(tenant_id, ledger_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgersApi->patch_ledger_async: #{e}"
end
```

#### Using the patch_ledger_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_ledger_async_with_http_info(tenant_id, ledger_id, opts)

```ruby
begin
  # Patches a ledger
  data, status_code, headers = api_instance.patch_ledger_async_with_http_info(tenant_id, ledger_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgersApi->patch_ledger_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **ledger_id** | **String** |  |  |
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


## update_ledger_async

> <EmptyEnvelope> update_ledger_async(tenant_id, ledger_id, opts)

Updates a ledger

Updates the specified ledger.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LedgersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
ledger_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  update_ledger_dto: OpenapiClient::UpdateLedgerDto.new # UpdateLedgerDto | 
}

begin
  # Updates a ledger
  result = api_instance.update_ledger_async(tenant_id, ledger_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgersApi->update_ledger_async: #{e}"
end
```

#### Using the update_ledger_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_ledger_async_with_http_info(tenant_id, ledger_id, opts)

```ruby
begin
  # Updates a ledger
  data, status_code, headers = api_instance.update_ledger_async_with_http_info(tenant_id, ledger_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LedgersApi->update_ledger_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **ledger_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **update_ledger_dto** | [**UpdateLedgerDto**](UpdateLedgerDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

