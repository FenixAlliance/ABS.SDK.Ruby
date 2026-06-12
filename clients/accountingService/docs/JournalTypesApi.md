# OpenapiClient::JournalTypesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_journal_type_async**](JournalTypesApi.md#create_journal_type_async) | **POST** /api/v2/AccountingService/JournalTypes | Creates a new journal type |
| [**delete_journal_type_async**](JournalTypesApi.md#delete_journal_type_async) | **DELETE** /api/v2/AccountingService/JournalTypes/{journalTypeId} | Deletes a journal type |
| [**get_journal_type_details_async**](JournalTypesApi.md#get_journal_type_details_async) | **GET** /api/v2/AccountingService/JournalTypes/{journalTypeId} | Retrieves a journal type by ID |
| [**get_journal_types_async**](JournalTypesApi.md#get_journal_types_async) | **GET** /api/v2/AccountingService/JournalTypes | Retrieves all journal types |
| [**get_journal_types_count_async**](JournalTypesApi.md#get_journal_types_count_async) | **GET** /api/v2/AccountingService/JournalTypes/Count | Counts journal types |
| [**patch_journal_type_async**](JournalTypesApi.md#patch_journal_type_async) | **PATCH** /api/v2/AccountingService/JournalTypes/{journalTypeId} | Patch a journal type |
| [**update_journal_type_async**](JournalTypesApi.md#update_journal_type_async) | **PUT** /api/v2/AccountingService/JournalTypes/{journalTypeId} | Updates an existing journal type |


## create_journal_type_async

> <EmptyEnvelope> create_journal_type_async(tenant_id, opts)

Creates a new journal type

Adds a new journal type to the tenant's catalog.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  journal_type_create_dto: OpenapiClient::JournalTypeCreateDto.new # JournalTypeCreateDto | 
}

begin
  # Creates a new journal type
  result = api_instance.create_journal_type_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalTypesApi->create_journal_type_async: #{e}"
end
```

#### Using the create_journal_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_journal_type_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new journal type
  data, status_code, headers = api_instance.create_journal_type_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalTypesApi->create_journal_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **journal_type_create_dto** | [**JournalTypeCreateDto**](JournalTypeCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_journal_type_async

> <EmptyEnvelope> delete_journal_type_async(tenant_id, journal_type_id, opts)

Deletes a journal type

Removes a journal type from the tenant's configuration.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes a journal type
  result = api_instance.delete_journal_type_async(tenant_id, journal_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalTypesApi->delete_journal_type_async: #{e}"
end
```

#### Using the delete_journal_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_journal_type_async_with_http_info(tenant_id, journal_type_id, opts)

```ruby
begin
  # Deletes a journal type
  data, status_code, headers = api_instance.delete_journal_type_async_with_http_info(tenant_id, journal_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalTypesApi->delete_journal_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_journal_type_details_async

> <JournalTypeDtoEnvelope> get_journal_type_details_async(tenant_id, journal_type_id, opts)

Retrieves a journal type by ID

Fetches the journal type matching the specified ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieves a journal type by ID
  result = api_instance.get_journal_type_details_async(tenant_id, journal_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalTypesApi->get_journal_type_details_async: #{e}"
end
```

#### Using the get_journal_type_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JournalTypeDtoEnvelope>, Integer, Hash)> get_journal_type_details_async_with_http_info(tenant_id, journal_type_id, opts)

```ruby
begin
  # Retrieves a journal type by ID
  data, status_code, headers = api_instance.get_journal_type_details_async_with_http_info(tenant_id, journal_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JournalTypeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalTypesApi->get_journal_type_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**JournalTypeDtoEnvelope**](JournalTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_journal_types_async

> <JournalTypeDtoIReadOnlyListEnvelope> get_journal_types_async(tenant_id, opts)

Retrieves all journal types

Fetches all journal types for the current tenant with OData support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieves all journal types
  result = api_instance.get_journal_types_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalTypesApi->get_journal_types_async: #{e}"
end
```

#### Using the get_journal_types_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JournalTypeDtoIReadOnlyListEnvelope>, Integer, Hash)> get_journal_types_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieves all journal types
  data, status_code, headers = api_instance.get_journal_types_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JournalTypeDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalTypesApi->get_journal_types_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**JournalTypeDtoIReadOnlyListEnvelope**](JournalTypeDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_journal_types_count_async

> <Int32Envelope> get_journal_types_count_async(tenant_id, opts)

Counts journal types

Returns the total number of journal types available for the tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Counts journal types
  result = api_instance.get_journal_types_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalTypesApi->get_journal_types_count_async: #{e}"
end
```

#### Using the get_journal_types_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_journal_types_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Counts journal types
  data, status_code, headers = api_instance.get_journal_types_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalTypesApi->get_journal_types_count_async_with_http_info: #{e}"
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


## patch_journal_type_async

> <EmptyEnvelope> patch_journal_type_async(tenant_id, journal_type_id, opts)

Patch a journal type

Partially updates a journal type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a journal type
  result = api_instance.patch_journal_type_async(tenant_id, journal_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalTypesApi->patch_journal_type_async: #{e}"
end
```

#### Using the patch_journal_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_journal_type_async_with_http_info(tenant_id, journal_type_id, opts)

```ruby
begin
  # Patch a journal type
  data, status_code, headers = api_instance.patch_journal_type_async_with_http_info(tenant_id, journal_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalTypesApi->patch_journal_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_type_id** | **String** |  |  |
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


## update_journal_type_async

> <EmptyEnvelope> update_journal_type_async(tenant_id, journal_type_id, opts)

Updates an existing journal type

Modifies the details of a specific journal type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  journal_type_update_dto: OpenapiClient::JournalTypeUpdateDto.new # JournalTypeUpdateDto | 
}

begin
  # Updates an existing journal type
  result = api_instance.update_journal_type_async(tenant_id, journal_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalTypesApi->update_journal_type_async: #{e}"
end
```

#### Using the update_journal_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_journal_type_async_with_http_info(tenant_id, journal_type_id, opts)

```ruby
begin
  # Updates an existing journal type
  data, status_code, headers = api_instance.update_journal_type_async_with_http_info(tenant_id, journal_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalTypesApi->update_journal_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **journal_type_update_dto** | [**JournalTypeUpdateDto**](JournalTypeUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

