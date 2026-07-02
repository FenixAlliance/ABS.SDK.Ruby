# OpenapiClient::FiscalResponsibilityRecordsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_fiscal_responsibility_record**](FiscalResponsibilityRecordsApi.md#create_fiscal_responsibility_record) | **POST** /api/v2/AccountingService/Fiscals/Authorities/FiscalResponsibilityRecords | Create a fiscal responsibility record |
| [**delete_fiscal_responsibility_record**](FiscalResponsibilityRecordsApi.md#delete_fiscal_responsibility_record) | **DELETE** /api/v2/AccountingService/Fiscals/Authorities/FiscalResponsibilityRecords/{fiscalResponsibilityRecordId} | Delete a fiscal responsibility record |
| [**get_fiscal_responsibility_record**](FiscalResponsibilityRecordsApi.md#get_fiscal_responsibility_record) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalResponsibilities/{fiscalResponsibilityId}/FiscalResponsibilityRecords/{fiscalResponsibilityRecordId} | Get fiscal responsibility record by ID |
| [**get_fiscal_responsibility_records**](FiscalResponsibilityRecordsApi.md#get_fiscal_responsibility_records) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalResponsibilities/{fiscalResponsibilityId}/FiscalResponsibilityRecords | Get fiscal responsibility records |
| [**get_fiscal_responsibility_records_count**](FiscalResponsibilityRecordsApi.md#get_fiscal_responsibility_records_count) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalResponsibilities/{fiscalResponsibilityId}/FiscalResponsibilityRecords/Count | Get fiscal responsibility records count |
| [**patch_fiscal_responsibility_record_async**](FiscalResponsibilityRecordsApi.md#patch_fiscal_responsibility_record_async) | **PATCH** /api/v2/AccountingService/Fiscals/Authorities/FiscalResponsibilityRecords/{fiscalResponsibilityRecordId} | Patch a fiscal responsibility record |
| [**update_fiscal_responsibility_record**](FiscalResponsibilityRecordsApi.md#update_fiscal_responsibility_record) | **PUT** /api/v2/AccountingService/Fiscals/Authorities/FiscalResponsibilityRecords/{fiscalResponsibilityRecordId} | Update a fiscal responsibility record |


## create_fiscal_responsibility_record

> <EmptyEnvelope> create_fiscal_responsibility_record(tenant_id, opts)

Create a fiscal responsibility record

Creates a new fiscal responsibility record for a fiscal responsibility.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalResponsibilityRecordsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  fiscal_responsibility_record_create_dto: OpenapiClient::FiscalResponsibilityRecordCreateDto.new # FiscalResponsibilityRecordCreateDto | 
}

begin
  # Create a fiscal responsibility record
  result = api_instance.create_fiscal_responsibility_record(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilityRecordsApi->create_fiscal_responsibility_record: #{e}"
end
```

#### Using the create_fiscal_responsibility_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_fiscal_responsibility_record_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a fiscal responsibility record
  data, status_code, headers = api_instance.create_fiscal_responsibility_record_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilityRecordsApi->create_fiscal_responsibility_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **fiscal_responsibility_record_create_dto** | [**FiscalResponsibilityRecordCreateDto**](FiscalResponsibilityRecordCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_fiscal_responsibility_record

> <EmptyEnvelope> delete_fiscal_responsibility_record(tenant_id, fiscal_responsibility_record_id, opts)

Delete a fiscal responsibility record

Deletes a fiscal responsibility record identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalResponsibilityRecordsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_responsibility_record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a fiscal responsibility record
  result = api_instance.delete_fiscal_responsibility_record(tenant_id, fiscal_responsibility_record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilityRecordsApi->delete_fiscal_responsibility_record: #{e}"
end
```

#### Using the delete_fiscal_responsibility_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_fiscal_responsibility_record_with_http_info(tenant_id, fiscal_responsibility_record_id, opts)

```ruby
begin
  # Delete a fiscal responsibility record
  data, status_code, headers = api_instance.delete_fiscal_responsibility_record_with_http_info(tenant_id, fiscal_responsibility_record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilityRecordsApi->delete_fiscal_responsibility_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_responsibility_record_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_responsibility_record

> <FiscalResponsibilityRecordDtoEnvelope> get_fiscal_responsibility_record(tenant_id, fiscal_authority_id, fiscal_responsibility_id, fiscal_responsibility_record_id, opts)

Get fiscal responsibility record by ID

Retrieves a specific fiscal responsibility record by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalResponsibilityRecordsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_responsibility_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_responsibility_record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal responsibility record by ID
  result = api_instance.get_fiscal_responsibility_record(tenant_id, fiscal_authority_id, fiscal_responsibility_id, fiscal_responsibility_record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilityRecordsApi->get_fiscal_responsibility_record: #{e}"
end
```

#### Using the get_fiscal_responsibility_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FiscalResponsibilityRecordDtoEnvelope>, Integer, Hash)> get_fiscal_responsibility_record_with_http_info(tenant_id, fiscal_authority_id, fiscal_responsibility_id, fiscal_responsibility_record_id, opts)

```ruby
begin
  # Get fiscal responsibility record by ID
  data, status_code, headers = api_instance.get_fiscal_responsibility_record_with_http_info(tenant_id, fiscal_authority_id, fiscal_responsibility_id, fiscal_responsibility_record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FiscalResponsibilityRecordDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilityRecordsApi->get_fiscal_responsibility_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_authority_id** | **String** |  |  |
| **fiscal_responsibility_id** | **String** |  |  |
| **fiscal_responsibility_record_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**FiscalResponsibilityRecordDtoEnvelope**](FiscalResponsibilityRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_responsibility_records

> <FiscalResponsibilityRecordDtoListEnvelope> get_fiscal_responsibility_records(tenant_id, fiscal_authority_id, fiscal_responsibility_id, opts)

Get fiscal responsibility records

Retrieves all fiscal responsibility records for the specified fiscal responsibility.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalResponsibilityRecordsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_responsibility_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal responsibility records
  result = api_instance.get_fiscal_responsibility_records(tenant_id, fiscal_authority_id, fiscal_responsibility_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilityRecordsApi->get_fiscal_responsibility_records: #{e}"
end
```

#### Using the get_fiscal_responsibility_records_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FiscalResponsibilityRecordDtoListEnvelope>, Integer, Hash)> get_fiscal_responsibility_records_with_http_info(tenant_id, fiscal_authority_id, fiscal_responsibility_id, opts)

```ruby
begin
  # Get fiscal responsibility records
  data, status_code, headers = api_instance.get_fiscal_responsibility_records_with_http_info(tenant_id, fiscal_authority_id, fiscal_responsibility_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FiscalResponsibilityRecordDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilityRecordsApi->get_fiscal_responsibility_records_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_authority_id** | **String** |  |  |
| **fiscal_responsibility_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**FiscalResponsibilityRecordDtoListEnvelope**](FiscalResponsibilityRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_responsibility_records_count

> <Int32Envelope> get_fiscal_responsibility_records_count(tenant_id, fiscal_authority_id, fiscal_responsibility_id, opts)

Get fiscal responsibility records count

Returns the total count of fiscal responsibility records for the specified fiscal responsibility.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalResponsibilityRecordsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_responsibility_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal responsibility records count
  result = api_instance.get_fiscal_responsibility_records_count(tenant_id, fiscal_authority_id, fiscal_responsibility_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilityRecordsApi->get_fiscal_responsibility_records_count: #{e}"
end
```

#### Using the get_fiscal_responsibility_records_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_fiscal_responsibility_records_count_with_http_info(tenant_id, fiscal_authority_id, fiscal_responsibility_id, opts)

```ruby
begin
  # Get fiscal responsibility records count
  data, status_code, headers = api_instance.get_fiscal_responsibility_records_count_with_http_info(tenant_id, fiscal_authority_id, fiscal_responsibility_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilityRecordsApi->get_fiscal_responsibility_records_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_authority_id** | **String** |  |  |
| **fiscal_responsibility_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_fiscal_responsibility_record_async

> <EmptyEnvelope> patch_fiscal_responsibility_record_async(tenant_id, fiscal_responsibility_record_id, opts)

Patch a fiscal responsibility record

Partially updates a fiscal responsibility record.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalResponsibilityRecordsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_responsibility_record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a fiscal responsibility record
  result = api_instance.patch_fiscal_responsibility_record_async(tenant_id, fiscal_responsibility_record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilityRecordsApi->patch_fiscal_responsibility_record_async: #{e}"
end
```

#### Using the patch_fiscal_responsibility_record_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_fiscal_responsibility_record_async_with_http_info(tenant_id, fiscal_responsibility_record_id, opts)

```ruby
begin
  # Patch a fiscal responsibility record
  data, status_code, headers = api_instance.patch_fiscal_responsibility_record_async_with_http_info(tenant_id, fiscal_responsibility_record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilityRecordsApi->patch_fiscal_responsibility_record_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_responsibility_record_id** | **String** |  |  |
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


## update_fiscal_responsibility_record

> <EmptyEnvelope> update_fiscal_responsibility_record(tenant_id, fiscal_responsibility_record_id, opts)

Update a fiscal responsibility record

Updates an existing fiscal responsibility record identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalResponsibilityRecordsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_responsibility_record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  fiscal_responsibility_record_update_dto: OpenapiClient::FiscalResponsibilityRecordUpdateDto.new # FiscalResponsibilityRecordUpdateDto | 
}

begin
  # Update a fiscal responsibility record
  result = api_instance.update_fiscal_responsibility_record(tenant_id, fiscal_responsibility_record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilityRecordsApi->update_fiscal_responsibility_record: #{e}"
end
```

#### Using the update_fiscal_responsibility_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_fiscal_responsibility_record_with_http_info(tenant_id, fiscal_responsibility_record_id, opts)

```ruby
begin
  # Update a fiscal responsibility record
  data, status_code, headers = api_instance.update_fiscal_responsibility_record_with_http_info(tenant_id, fiscal_responsibility_record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilityRecordsApi->update_fiscal_responsibility_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_responsibility_record_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **fiscal_responsibility_record_update_dto** | [**FiscalResponsibilityRecordUpdateDto**](FiscalResponsibilityRecordUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

