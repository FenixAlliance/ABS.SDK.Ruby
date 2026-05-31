# OpenapiClient::TeamRecordsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_tenant_team_record**](TeamRecordsApi.md#create_tenant_team_record) | **POST** /api/v2/TenantsService/TeamRecords | Create a new tenant team record |
| [**delete_tenant_team_record**](TeamRecordsApi.md#delete_tenant_team_record) | **DELETE** /api/v2/TenantsService/TeamRecords/{tenantTeamRecordId} | Delete a tenant team record |
| [**get_tenant_team_record_by_id**](TeamRecordsApi.md#get_tenant_team_record_by_id) | **GET** /api/v2/TenantsService/TeamRecords/{tenantTeamRecordId} | Retrieve a single tenant team record by its ID |
| [**get_tenant_team_records**](TeamRecordsApi.md#get_tenant_team_records) | **GET** /api/v2/TenantsService/TeamRecords | Retrieve a list of tenant team records |
| [**get_tenant_team_records_count**](TeamRecordsApi.md#get_tenant_team_records_count) | **GET** /api/v2/TenantsService/TeamRecords/Count | Get the count of tenant team records |
| [**update_tenant_team_record**](TeamRecordsApi.md#update_tenant_team_record) | **PUT** /api/v2/TenantsService/TeamRecords/{tenantTeamRecordId} | Update a tenant team record |


## create_tenant_team_record

> <EmptyEnvelope> create_tenant_team_record(tenant_id, opts)

Create a new tenant team record

Create a new tenant team record

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamRecordsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_team_record_create_dto: OpenapiClient::TenantTeamRecordCreateDto.new({business_team_id: 'business_team_id_example'}) # TenantTeamRecordCreateDto | 
}

begin
  # Create a new tenant team record
  result = api_instance.create_tenant_team_record(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamRecordsApi->create_tenant_team_record: #{e}"
end
```

#### Using the create_tenant_team_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tenant_team_record_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new tenant team record
  data, status_code, headers = api_instance.create_tenant_team_record_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamRecordsApi->create_tenant_team_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_team_record_create_dto** | [**TenantTeamRecordCreateDto**](TenantTeamRecordCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_tenant_team_record

> <EmptyEnvelope> delete_tenant_team_record(tenant_id, tenant_team_record_id, opts)

Delete a tenant team record

Delete a tenant team record

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamRecordsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_team_record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tenant team record
  result = api_instance.delete_tenant_team_record(tenant_id, tenant_team_record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamRecordsApi->delete_tenant_team_record: #{e}"
end
```

#### Using the delete_tenant_team_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tenant_team_record_with_http_info(tenant_id, tenant_team_record_id, opts)

```ruby
begin
  # Delete a tenant team record
  data, status_code, headers = api_instance.delete_tenant_team_record_with_http_info(tenant_id, tenant_team_record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamRecordsApi->delete_tenant_team_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_team_record_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_team_record_by_id

> <TenantTeamRecordDtoEnvelope> get_tenant_team_record_by_id(tenant_id, tenant_team_record_id, opts)

Retrieve a single tenant team record by its ID

Retrieve a single tenant team record by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamRecordsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_team_record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single tenant team record by its ID
  result = api_instance.get_tenant_team_record_by_id(tenant_id, tenant_team_record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamRecordsApi->get_tenant_team_record_by_id: #{e}"
end
```

#### Using the get_tenant_team_record_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantTeamRecordDtoEnvelope>, Integer, Hash)> get_tenant_team_record_by_id_with_http_info(tenant_id, tenant_team_record_id, opts)

```ruby
begin
  # Retrieve a single tenant team record by its ID
  data, status_code, headers = api_instance.get_tenant_team_record_by_id_with_http_info(tenant_id, tenant_team_record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantTeamRecordDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamRecordsApi->get_tenant_team_record_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_team_record_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantTeamRecordDtoEnvelope**](TenantTeamRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_team_records

> <TenantTeamRecordDtoListEnvelope> get_tenant_team_records(tenant_id, opts)

Retrieve a list of tenant team records

Retrieve a list of tenant team records

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamRecordsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of tenant team records
  result = api_instance.get_tenant_team_records(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamRecordsApi->get_tenant_team_records: #{e}"
end
```

#### Using the get_tenant_team_records_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantTeamRecordDtoListEnvelope>, Integer, Hash)> get_tenant_team_records_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of tenant team records
  data, status_code, headers = api_instance.get_tenant_team_records_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantTeamRecordDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamRecordsApi->get_tenant_team_records_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantTeamRecordDtoListEnvelope**](TenantTeamRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_team_records_count

> <Int32Envelope> get_tenant_team_records_count(tenant_id, opts)

Get the count of tenant team records

Get the count of tenant team records

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamRecordsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of tenant team records
  result = api_instance.get_tenant_team_records_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamRecordsApi->get_tenant_team_records_count: #{e}"
end
```

#### Using the get_tenant_team_records_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tenant_team_records_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of tenant team records
  data, status_code, headers = api_instance.get_tenant_team_records_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamRecordsApi->get_tenant_team_records_count_with_http_info: #{e}"
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


## update_tenant_team_record

> <EmptyEnvelope> update_tenant_team_record(tenant_id, tenant_team_record_id, opts)

Update a tenant team record

Update a tenant team record

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamRecordsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_team_record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_team_record_update_dto: OpenapiClient::TenantTeamRecordUpdateDto.new # TenantTeamRecordUpdateDto | 
}

begin
  # Update a tenant team record
  result = api_instance.update_tenant_team_record(tenant_id, tenant_team_record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamRecordsApi->update_tenant_team_record: #{e}"
end
```

#### Using the update_tenant_team_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tenant_team_record_with_http_info(tenant_id, tenant_team_record_id, opts)

```ruby
begin
  # Update a tenant team record
  data, status_code, headers = api_instance.update_tenant_team_record_with_http_info(tenant_id, tenant_team_record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamRecordsApi->update_tenant_team_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_team_record_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_team_record_update_dto** | [**TenantTeamRecordUpdateDto**](TenantTeamRecordUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

