# OpenapiClient::TaxPoliciesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_applied_tax_policy_record**](TaxPoliciesApi.md#create_applied_tax_policy_record) | **POST** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/AppliedTaxPolicyRecords | Create an applied tax policy record |
| [**create_item_tax_policy_record**](TaxPoliciesApi.md#create_item_tax_policy_record) | **POST** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/ItemTaxPolicyRecords | Create an item tax policy record |
| [**create_tax_policy**](TaxPoliciesApi.md#create_tax_policy) | **POST** /api/v2/AccountingService/TaxPolicies | Create a tax policy |
| [**delete_applied_tax_policy_record**](TaxPoliciesApi.md#delete_applied_tax_policy_record) | **DELETE** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/AppliedTaxPolicyRecords/{appliedTaxPolicyRecordId} | Delete an applied tax policy record |
| [**delete_item_tax_policy_record**](TaxPoliciesApi.md#delete_item_tax_policy_record) | **DELETE** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/ItemTaxPolicyRecords/{itemTaxPolicyRecordId} | Delete an item tax policy record |
| [**delete_tax_policy**](TaxPoliciesApi.md#delete_tax_policy) | **DELETE** /api/v2/AccountingService/TaxPolicies/{id} | Delete a tax policy |
| [**get_applied_tax_policy_record**](TaxPoliciesApi.md#get_applied_tax_policy_record) | **GET** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/AppliedTaxPolicyRecords/{appliedTaxPolicyRecordId} | Get applied tax policy record by ID |
| [**get_applied_tax_policy_records**](TaxPoliciesApi.md#get_applied_tax_policy_records) | **GET** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/AppliedTaxPolicyRecords | Get applied tax policy records |
| [**get_applied_tax_policy_records_count**](TaxPoliciesApi.md#get_applied_tax_policy_records_count) | **GET** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/AppliedTaxPolicyRecords/Count | Get applied tax policy records count |
| [**get_item_tax_policy_record**](TaxPoliciesApi.md#get_item_tax_policy_record) | **GET** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/ItemTaxPolicyRecords/{itemTaxPolicyRecordId} | Get item tax policy record by ID |
| [**get_item_tax_policy_records**](TaxPoliciesApi.md#get_item_tax_policy_records) | **GET** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/ItemTaxPolicyRecords | Get item tax policy records |
| [**get_tax_policies**](TaxPoliciesApi.md#get_tax_policies) | **GET** /api/v2/AccountingService/TaxPolicies | Get all tax policies for a tenant |
| [**get_tax_policies_by_authority**](TaxPoliciesApi.md#get_tax_policies_by_authority) | **GET** /api/v2/AccountingService/TaxPolicies/ByAuthority/{authorityId} | Get tax policies by fiscal authority |
| [**get_tax_policies_count**](TaxPoliciesApi.md#get_tax_policies_count) | **GET** /api/v2/AccountingService/TaxPolicies/Count | Get tax policies count |
| [**get_tax_policy**](TaxPoliciesApi.md#get_tax_policy) | **GET** /api/v2/AccountingService/TaxPolicies/{id} | Get tax policy by ID |
| [**patch_applied_tax_policy_record**](TaxPoliciesApi.md#patch_applied_tax_policy_record) | **PATCH** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/AppliedTaxPolicyRecords/{appliedTaxPolicyRecordId} | Patch an applied tax policy record |
| [**patch_item_tax_policy_record**](TaxPoliciesApi.md#patch_item_tax_policy_record) | **PATCH** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/ItemTaxPolicyRecords/{itemTaxPolicyRecordId} | Patch an item tax policy record |
| [**patch_tax_policy**](TaxPoliciesApi.md#patch_tax_policy) | **PATCH** /api/v2/AccountingService/TaxPolicies/{id} | Patch a tax policy |
| [**update_applied_tax_policy_record**](TaxPoliciesApi.md#update_applied_tax_policy_record) | **PUT** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/AppliedTaxPolicyRecords/{appliedTaxPolicyRecordId} | Update an applied tax policy record |
| [**update_item_tax_policy_record**](TaxPoliciesApi.md#update_item_tax_policy_record) | **PUT** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/ItemTaxPolicyRecords/{itemTaxPolicyRecordId} | Update an item tax policy record |
| [**update_tax_policy**](TaxPoliciesApi.md#update_tax_policy) | **PUT** /api/v2/AccountingService/TaxPolicies/{id} | Update a tax policy |


## create_applied_tax_policy_record

> <EmptyEnvelope> create_applied_tax_policy_record(tenant_id, tax_policy_id, opts)

Create an applied tax policy record

Creates a new applied tax policy record for the specified tax policy.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tax_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  applied_tax_policy_record_create_dto: OpenapiClient::AppliedTaxPolicyRecordCreateDto.new # AppliedTaxPolicyRecordCreateDto | 
}

begin
  # Create an applied tax policy record
  result = api_instance.create_applied_tax_policy_record(tenant_id, tax_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->create_applied_tax_policy_record: #{e}"
end
```

#### Using the create_applied_tax_policy_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_applied_tax_policy_record_with_http_info(tenant_id, tax_policy_id, opts)

```ruby
begin
  # Create an applied tax policy record
  data, status_code, headers = api_instance.create_applied_tax_policy_record_with_http_info(tenant_id, tax_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->create_applied_tax_policy_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tax_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **applied_tax_policy_record_create_dto** | [**AppliedTaxPolicyRecordCreateDto**](AppliedTaxPolicyRecordCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_item_tax_policy_record

> <EmptyEnvelope> create_item_tax_policy_record(tenant_id, tax_policy_id, opts)

Create an item tax policy record

Creates a new item tax policy record for the specified tax policy.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tax_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_tax_policy_record_create_dto: OpenapiClient::ItemTaxPolicyRecordCreateDto.new # ItemTaxPolicyRecordCreateDto | 
}

begin
  # Create an item tax policy record
  result = api_instance.create_item_tax_policy_record(tenant_id, tax_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->create_item_tax_policy_record: #{e}"
end
```

#### Using the create_item_tax_policy_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_item_tax_policy_record_with_http_info(tenant_id, tax_policy_id, opts)

```ruby
begin
  # Create an item tax policy record
  data, status_code, headers = api_instance.create_item_tax_policy_record_with_http_info(tenant_id, tax_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->create_item_tax_policy_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tax_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_tax_policy_record_create_dto** | [**ItemTaxPolicyRecordCreateDto**](ItemTaxPolicyRecordCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_tax_policy

> <EmptyEnvelope> create_tax_policy(tenant_id, opts)

Create a tax policy

Creates a new tax policy for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tax_policy_create_dto: OpenapiClient::TaxPolicyCreateDto.new # TaxPolicyCreateDto | 
}

begin
  # Create a tax policy
  result = api_instance.create_tax_policy(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->create_tax_policy: #{e}"
end
```

#### Using the create_tax_policy_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tax_policy_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a tax policy
  data, status_code, headers = api_instance.create_tax_policy_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->create_tax_policy_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tax_policy_create_dto** | [**TaxPolicyCreateDto**](TaxPolicyCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_applied_tax_policy_record

> <EmptyEnvelope> delete_applied_tax_policy_record(tenant_id, tax_policy_id, applied_tax_policy_record_id, opts)

Delete an applied tax policy record

Deletes an applied tax policy record identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tax_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
applied_tax_policy_record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an applied tax policy record
  result = api_instance.delete_applied_tax_policy_record(tenant_id, tax_policy_id, applied_tax_policy_record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->delete_applied_tax_policy_record: #{e}"
end
```

#### Using the delete_applied_tax_policy_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_applied_tax_policy_record_with_http_info(tenant_id, tax_policy_id, applied_tax_policy_record_id, opts)

```ruby
begin
  # Delete an applied tax policy record
  data, status_code, headers = api_instance.delete_applied_tax_policy_record_with_http_info(tenant_id, tax_policy_id, applied_tax_policy_record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->delete_applied_tax_policy_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tax_policy_id** | **String** |  |  |
| **applied_tax_policy_record_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_item_tax_policy_record

> <EmptyEnvelope> delete_item_tax_policy_record(tenant_id, tax_policy_id, item_tax_policy_record_id, opts)

Delete an item tax policy record

Deletes an item tax policy record identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tax_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_tax_policy_record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an item tax policy record
  result = api_instance.delete_item_tax_policy_record(tenant_id, tax_policy_id, item_tax_policy_record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->delete_item_tax_policy_record: #{e}"
end
```

#### Using the delete_item_tax_policy_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_item_tax_policy_record_with_http_info(tenant_id, tax_policy_id, item_tax_policy_record_id, opts)

```ruby
begin
  # Delete an item tax policy record
  data, status_code, headers = api_instance.delete_item_tax_policy_record_with_http_info(tenant_id, tax_policy_id, item_tax_policy_record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->delete_item_tax_policy_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tax_policy_id** | **String** |  |  |
| **item_tax_policy_record_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_tax_policy

> <EmptyEnvelope> delete_tax_policy(tenant_id, id, opts)

Delete a tax policy

Deletes a tax policy identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tax policy
  result = api_instance.delete_tax_policy(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->delete_tax_policy: #{e}"
end
```

#### Using the delete_tax_policy_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tax_policy_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a tax policy
  data, status_code, headers = api_instance.delete_tax_policy_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->delete_tax_policy_with_http_info: #{e}"
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

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_applied_tax_policy_record

> <AppliedTaxPolicyRecordDtoEnvelope> get_applied_tax_policy_record(tenant_id, tax_policy_id, applied_tax_policy_record_id, opts)

Get applied tax policy record by ID

Retrieves a specific applied tax policy record by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tax_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
applied_tax_policy_record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get applied tax policy record by ID
  result = api_instance.get_applied_tax_policy_record(tenant_id, tax_policy_id, applied_tax_policy_record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->get_applied_tax_policy_record: #{e}"
end
```

#### Using the get_applied_tax_policy_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AppliedTaxPolicyRecordDtoEnvelope>, Integer, Hash)> get_applied_tax_policy_record_with_http_info(tenant_id, tax_policy_id, applied_tax_policy_record_id, opts)

```ruby
begin
  # Get applied tax policy record by ID
  data, status_code, headers = api_instance.get_applied_tax_policy_record_with_http_info(tenant_id, tax_policy_id, applied_tax_policy_record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AppliedTaxPolicyRecordDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->get_applied_tax_policy_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tax_policy_id** | **String** |  |  |
| **applied_tax_policy_record_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**AppliedTaxPolicyRecordDtoEnvelope**](AppliedTaxPolicyRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_applied_tax_policy_records

> <AppliedTaxPolicyRecordDtoListEnvelope> get_applied_tax_policy_records(tenant_id, tax_policy_id, opts)

Get applied tax policy records

Retrieves all applied tax policy records for the specified tax policy.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tax_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  applied_tax_policy_record_dto_collection_query_parameters: OpenapiClient::AppliedTaxPolicyRecordDtoCollectionQueryParameters.new # AppliedTaxPolicyRecordDtoCollectionQueryParameters | 
}

begin
  # Get applied tax policy records
  result = api_instance.get_applied_tax_policy_records(tenant_id, tax_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->get_applied_tax_policy_records: #{e}"
end
```

#### Using the get_applied_tax_policy_records_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AppliedTaxPolicyRecordDtoListEnvelope>, Integer, Hash)> get_applied_tax_policy_records_with_http_info(tenant_id, tax_policy_id, opts)

```ruby
begin
  # Get applied tax policy records
  data, status_code, headers = api_instance.get_applied_tax_policy_records_with_http_info(tenant_id, tax_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AppliedTaxPolicyRecordDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->get_applied_tax_policy_records_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tax_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **applied_tax_policy_record_dto_collection_query_parameters** | [**AppliedTaxPolicyRecordDtoCollectionQueryParameters**](AppliedTaxPolicyRecordDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AppliedTaxPolicyRecordDtoListEnvelope**](AppliedTaxPolicyRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_applied_tax_policy_records_count

> <Int32Envelope> get_applied_tax_policy_records_count(tenant_id, tax_policy_id, opts)

Get applied tax policy records count

Returns the total count of applied tax policy records for the specified tax policy.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tax_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  applied_tax_policy_record_dto_collection_query_parameters: OpenapiClient::AppliedTaxPolicyRecordDtoCollectionQueryParameters.new # AppliedTaxPolicyRecordDtoCollectionQueryParameters | 
}

begin
  # Get applied tax policy records count
  result = api_instance.get_applied_tax_policy_records_count(tenant_id, tax_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->get_applied_tax_policy_records_count: #{e}"
end
```

#### Using the get_applied_tax_policy_records_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_applied_tax_policy_records_count_with_http_info(tenant_id, tax_policy_id, opts)

```ruby
begin
  # Get applied tax policy records count
  data, status_code, headers = api_instance.get_applied_tax_policy_records_count_with_http_info(tenant_id, tax_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->get_applied_tax_policy_records_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tax_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **applied_tax_policy_record_dto_collection_query_parameters** | [**AppliedTaxPolicyRecordDtoCollectionQueryParameters**](AppliedTaxPolicyRecordDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_item_tax_policy_record

> <ItemTaxPolicyRecordDtoEnvelope> get_item_tax_policy_record(tenant_id, tax_policy_id, item_tax_policy_record_id, opts)

Get item tax policy record by ID

Retrieves a specific item tax policy record by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tax_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_tax_policy_record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item tax policy record by ID
  result = api_instance.get_item_tax_policy_record(tenant_id, tax_policy_id, item_tax_policy_record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->get_item_tax_policy_record: #{e}"
end
```

#### Using the get_item_tax_policy_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTaxPolicyRecordDtoEnvelope>, Integer, Hash)> get_item_tax_policy_record_with_http_info(tenant_id, tax_policy_id, item_tax_policy_record_id, opts)

```ruby
begin
  # Get item tax policy record by ID
  data, status_code, headers = api_instance.get_item_tax_policy_record_with_http_info(tenant_id, tax_policy_id, item_tax_policy_record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTaxPolicyRecordDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->get_item_tax_policy_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tax_policy_id** | **String** |  |  |
| **item_tax_policy_record_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTaxPolicyRecordDtoEnvelope**](ItemTaxPolicyRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_tax_policy_records

> <ItemTaxPolicyRecordDtoListEnvelope> get_item_tax_policy_records(tenant_id, tax_policy_id, opts)

Get item tax policy records

Retrieves all item tax policy records for the specified tax policy.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tax_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_tax_policy_record_dto_collection_query_parameters: OpenapiClient::ItemTaxPolicyRecordDtoCollectionQueryParameters.new # ItemTaxPolicyRecordDtoCollectionQueryParameters | 
}

begin
  # Get item tax policy records
  result = api_instance.get_item_tax_policy_records(tenant_id, tax_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->get_item_tax_policy_records: #{e}"
end
```

#### Using the get_item_tax_policy_records_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTaxPolicyRecordDtoListEnvelope>, Integer, Hash)> get_item_tax_policy_records_with_http_info(tenant_id, tax_policy_id, opts)

```ruby
begin
  # Get item tax policy records
  data, status_code, headers = api_instance.get_item_tax_policy_records_with_http_info(tenant_id, tax_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTaxPolicyRecordDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->get_item_tax_policy_records_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tax_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_tax_policy_record_dto_collection_query_parameters** | [**ItemTaxPolicyRecordDtoCollectionQueryParameters**](ItemTaxPolicyRecordDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ItemTaxPolicyRecordDtoListEnvelope**](ItemTaxPolicyRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_tax_policies

> <TaxPolicyDtoListEnvelope> get_tax_policies(tenant_id, opts)

Get all tax policies for a tenant

Retrieves all tax policies for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tax_policy_dto_collection_query_parameters: OpenapiClient::TaxPolicyDtoCollectionQueryParameters.new # TaxPolicyDtoCollectionQueryParameters | 
}

begin
  # Get all tax policies for a tenant
  result = api_instance.get_tax_policies(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->get_tax_policies: #{e}"
end
```

#### Using the get_tax_policies_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TaxPolicyDtoListEnvelope>, Integer, Hash)> get_tax_policies_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all tax policies for a tenant
  data, status_code, headers = api_instance.get_tax_policies_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TaxPolicyDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->get_tax_policies_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tax_policy_dto_collection_query_parameters** | [**TaxPolicyDtoCollectionQueryParameters**](TaxPolicyDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**TaxPolicyDtoListEnvelope**](TaxPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_tax_policies_by_authority

> <TaxPolicyDtoListEnvelope> get_tax_policies_by_authority(tenant_id, authority_id, opts)

Get tax policies by fiscal authority

Retrieves all tax policies associated with the specified fiscal authority.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tax_policy_dto_collection_query_parameters: OpenapiClient::TaxPolicyDtoCollectionQueryParameters.new # TaxPolicyDtoCollectionQueryParameters | 
}

begin
  # Get tax policies by fiscal authority
  result = api_instance.get_tax_policies_by_authority(tenant_id, authority_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->get_tax_policies_by_authority: #{e}"
end
```

#### Using the get_tax_policies_by_authority_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TaxPolicyDtoListEnvelope>, Integer, Hash)> get_tax_policies_by_authority_with_http_info(tenant_id, authority_id, opts)

```ruby
begin
  # Get tax policies by fiscal authority
  data, status_code, headers = api_instance.get_tax_policies_by_authority_with_http_info(tenant_id, authority_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TaxPolicyDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->get_tax_policies_by_authority_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **authority_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tax_policy_dto_collection_query_parameters** | [**TaxPolicyDtoCollectionQueryParameters**](TaxPolicyDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**TaxPolicyDtoListEnvelope**](TaxPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_tax_policies_count

> <Int32Envelope> get_tax_policies_count(tenant_id, opts)

Get tax policies count

Returns the count of tax policies for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tax_policy_dto_collection_query_parameters: OpenapiClient::TaxPolicyDtoCollectionQueryParameters.new # TaxPolicyDtoCollectionQueryParameters | 
}

begin
  # Get tax policies count
  result = api_instance.get_tax_policies_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->get_tax_policies_count: #{e}"
end
```

#### Using the get_tax_policies_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tax_policies_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get tax policies count
  data, status_code, headers = api_instance.get_tax_policies_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->get_tax_policies_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tax_policy_dto_collection_query_parameters** | [**TaxPolicyDtoCollectionQueryParameters**](TaxPolicyDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_tax_policy

> <TaxPolicyDtoEnvelope> get_tax_policy(tenant_id, id, opts)

Get tax policy by ID

Retrieves a specific tax policy by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get tax policy by ID
  result = api_instance.get_tax_policy(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->get_tax_policy: #{e}"
end
```

#### Using the get_tax_policy_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TaxPolicyDtoEnvelope>, Integer, Hash)> get_tax_policy_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get tax policy by ID
  data, status_code, headers = api_instance.get_tax_policy_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TaxPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->get_tax_policy_with_http_info: #{e}"
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

[**TaxPolicyDtoEnvelope**](TaxPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_applied_tax_policy_record

> <EmptyEnvelope> patch_applied_tax_policy_record(tenant_id, tax_policy_id, applied_tax_policy_record_id, opts)

Patch an applied tax policy record

Partially updates an existing applied tax policy record identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tax_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
applied_tax_policy_record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch an applied tax policy record
  result = api_instance.patch_applied_tax_policy_record(tenant_id, tax_policy_id, applied_tax_policy_record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->patch_applied_tax_policy_record: #{e}"
end
```

#### Using the patch_applied_tax_policy_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_applied_tax_policy_record_with_http_info(tenant_id, tax_policy_id, applied_tax_policy_record_id, opts)

```ruby
begin
  # Patch an applied tax policy record
  data, status_code, headers = api_instance.patch_applied_tax_policy_record_with_http_info(tenant_id, tax_policy_id, applied_tax_policy_record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->patch_applied_tax_policy_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tax_policy_id** | **String** |  |  |
| **applied_tax_policy_record_id** | **String** |  |  |
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


## patch_item_tax_policy_record

> <EmptyEnvelope> patch_item_tax_policy_record(tenant_id, tax_policy_id, item_tax_policy_record_id, opts)

Patch an item tax policy record

Partially updates an existing item tax policy record identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tax_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_tax_policy_record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch an item tax policy record
  result = api_instance.patch_item_tax_policy_record(tenant_id, tax_policy_id, item_tax_policy_record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->patch_item_tax_policy_record: #{e}"
end
```

#### Using the patch_item_tax_policy_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_item_tax_policy_record_with_http_info(tenant_id, tax_policy_id, item_tax_policy_record_id, opts)

```ruby
begin
  # Patch an item tax policy record
  data, status_code, headers = api_instance.patch_item_tax_policy_record_with_http_info(tenant_id, tax_policy_id, item_tax_policy_record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->patch_item_tax_policy_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tax_policy_id** | **String** |  |  |
| **item_tax_policy_record_id** | **String** |  |  |
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


## patch_tax_policy

> <EmptyEnvelope> patch_tax_policy(tenant_id, id, opts)

Patch a tax policy

Partially updates an existing tax policy identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a tax policy
  result = api_instance.patch_tax_policy(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->patch_tax_policy: #{e}"
end
```

#### Using the patch_tax_policy_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_tax_policy_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a tax policy
  data, status_code, headers = api_instance.patch_tax_policy_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->patch_tax_policy_with_http_info: #{e}"
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


## update_applied_tax_policy_record

> <EmptyEnvelope> update_applied_tax_policy_record(tenant_id, tax_policy_id, applied_tax_policy_record_id, opts)

Update an applied tax policy record

Updates an existing applied tax policy record identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tax_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
applied_tax_policy_record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  applied_tax_policy_record_update_dto: OpenapiClient::AppliedTaxPolicyRecordUpdateDto.new # AppliedTaxPolicyRecordUpdateDto | 
}

begin
  # Update an applied tax policy record
  result = api_instance.update_applied_tax_policy_record(tenant_id, tax_policy_id, applied_tax_policy_record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->update_applied_tax_policy_record: #{e}"
end
```

#### Using the update_applied_tax_policy_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_applied_tax_policy_record_with_http_info(tenant_id, tax_policy_id, applied_tax_policy_record_id, opts)

```ruby
begin
  # Update an applied tax policy record
  data, status_code, headers = api_instance.update_applied_tax_policy_record_with_http_info(tenant_id, tax_policy_id, applied_tax_policy_record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->update_applied_tax_policy_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tax_policy_id** | **String** |  |  |
| **applied_tax_policy_record_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **applied_tax_policy_record_update_dto** | [**AppliedTaxPolicyRecordUpdateDto**](AppliedTaxPolicyRecordUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_item_tax_policy_record

> <EmptyEnvelope> update_item_tax_policy_record(tenant_id, tax_policy_id, item_tax_policy_record_id, opts)

Update an item tax policy record

Updates an existing item tax policy record identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tax_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_tax_policy_record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_tax_policy_record_update_dto: OpenapiClient::ItemTaxPolicyRecordUpdateDto.new # ItemTaxPolicyRecordUpdateDto | 
}

begin
  # Update an item tax policy record
  result = api_instance.update_item_tax_policy_record(tenant_id, tax_policy_id, item_tax_policy_record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->update_item_tax_policy_record: #{e}"
end
```

#### Using the update_item_tax_policy_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_item_tax_policy_record_with_http_info(tenant_id, tax_policy_id, item_tax_policy_record_id, opts)

```ruby
begin
  # Update an item tax policy record
  data, status_code, headers = api_instance.update_item_tax_policy_record_with_http_info(tenant_id, tax_policy_id, item_tax_policy_record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->update_item_tax_policy_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tax_policy_id** | **String** |  |  |
| **item_tax_policy_record_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_tax_policy_record_update_dto** | [**ItemTaxPolicyRecordUpdateDto**](ItemTaxPolicyRecordUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_tax_policy

> <EmptyEnvelope> update_tax_policy(tenant_id, id, opts)

Update a tax policy

Updates an existing tax policy identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tax_policy_update_dto: OpenapiClient::TaxPolicyUpdateDto.new # TaxPolicyUpdateDto | 
}

begin
  # Update a tax policy
  result = api_instance.update_tax_policy(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->update_tax_policy: #{e}"
end
```

#### Using the update_tax_policy_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tax_policy_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a tax policy
  data, status_code, headers = api_instance.update_tax_policy_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxPoliciesApi->update_tax_policy_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tax_policy_update_dto** | [**TaxPolicyUpdateDto**](TaxPolicyUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

