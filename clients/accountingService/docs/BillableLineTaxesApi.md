# OpenapiClient::BillableLineTaxesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_billable_line_tax**](BillableLineTaxesApi.md#create_billable_line_tax) | **POST** /api/v2/AccountingService/BillableLines/{billableLineId}/Taxes | Create a new tax for a billable line. |
| [**delete_billable_line_tax**](BillableLineTaxesApi.md#delete_billable_line_tax) | **DELETE** /api/v2/AccountingService/BillableLines/{billableLineId}/Taxes/{taxId} | Delete a tax from a billable line. |
| [**get_billable_line_taxes**](BillableLineTaxesApi.md#get_billable_line_taxes) | **GET** /api/v2/AccountingService/BillableLines/{billableLineId}/Taxes | Get taxes for a billable line. |
| [**get_billable_line_taxes_count**](BillableLineTaxesApi.md#get_billable_line_taxes_count) | **GET** /api/v2/AccountingService/BillableLines/{billableLineId}/Taxes/Count | Get the count of taxes for a billable line. |
| [**patch_billable_line_tax_async**](BillableLineTaxesApi.md#patch_billable_line_tax_async) | **PATCH** /api/v2/AccountingService/BillableLines/{billableLineId}/Taxes/{taxId} | Patch a billable line tax |
| [**update_billable_line_tax**](BillableLineTaxesApi.md#update_billable_line_tax) | **PUT** /api/v2/AccountingService/BillableLines/{billableLineId}/Taxes/{taxId} | Update a tax for a billable line. |


## create_billable_line_tax

> <EmptyEnvelope> create_billable_line_tax(tenant_id, billable_line_id, opts)

Create a new tax for a billable line.

Creates a new tax entry for the specified billable line.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillableLineTaxesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
billable_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  applied_item_tax_record_create_dto: OpenapiClient::AppliedItemTaxRecordCreateDto.new # AppliedItemTaxRecordCreateDto | 
}

begin
  # Create a new tax for a billable line.
  result = api_instance.create_billable_line_tax(tenant_id, billable_line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillableLineTaxesApi->create_billable_line_tax: #{e}"
end
```

#### Using the create_billable_line_tax_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_billable_line_tax_with_http_info(tenant_id, billable_line_id, opts)

```ruby
begin
  # Create a new tax for a billable line.
  data, status_code, headers = api_instance.create_billable_line_tax_with_http_info(tenant_id, billable_line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillableLineTaxesApi->create_billable_line_tax_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **billable_line_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **applied_item_tax_record_create_dto** | [**AppliedItemTaxRecordCreateDto**](AppliedItemTaxRecordCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_billable_line_tax

> <EmptyEnvelope> delete_billable_line_tax(tenant_id, billable_line_id, tax_id, opts)

Delete a tax from a billable line.

Deletes the specified tax entry from the billable line.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillableLineTaxesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
billable_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tax_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tax from a billable line.
  result = api_instance.delete_billable_line_tax(tenant_id, billable_line_id, tax_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillableLineTaxesApi->delete_billable_line_tax: #{e}"
end
```

#### Using the delete_billable_line_tax_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_billable_line_tax_with_http_info(tenant_id, billable_line_id, tax_id, opts)

```ruby
begin
  # Delete a tax from a billable line.
  data, status_code, headers = api_instance.delete_billable_line_tax_with_http_info(tenant_id, billable_line_id, tax_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillableLineTaxesApi->delete_billable_line_tax_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **billable_line_id** | **String** |  |  |
| **tax_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_billable_line_taxes

> <AppliedItemTaxRecordDtoIReadOnlyListEnvelope> get_billable_line_taxes(tenant_id, billable_line_id, opts)

Get taxes for a billable line.

Retrieves the taxes applied to the specified billable line.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillableLineTaxesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
billable_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  applied_item_tax_record_dto_collection_query_parameters: OpenapiClient::AppliedItemTaxRecordDtoCollectionQueryParameters.new # AppliedItemTaxRecordDtoCollectionQueryParameters | 
}

begin
  # Get taxes for a billable line.
  result = api_instance.get_billable_line_taxes(tenant_id, billable_line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillableLineTaxesApi->get_billable_line_taxes: #{e}"
end
```

#### Using the get_billable_line_taxes_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AppliedItemTaxRecordDtoIReadOnlyListEnvelope>, Integer, Hash)> get_billable_line_taxes_with_http_info(tenant_id, billable_line_id, opts)

```ruby
begin
  # Get taxes for a billable line.
  data, status_code, headers = api_instance.get_billable_line_taxes_with_http_info(tenant_id, billable_line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AppliedItemTaxRecordDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillableLineTaxesApi->get_billable_line_taxes_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **billable_line_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **applied_item_tax_record_dto_collection_query_parameters** | [**AppliedItemTaxRecordDtoCollectionQueryParameters**](AppliedItemTaxRecordDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AppliedItemTaxRecordDtoIReadOnlyListEnvelope**](AppliedItemTaxRecordDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_billable_line_taxes_count

> <Int32Envelope> get_billable_line_taxes_count(tenant_id, billable_line_id, opts)

Get the count of taxes for a billable line.

Retrieves the total count of taxes applied to the specified billable line.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillableLineTaxesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
billable_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  applied_item_tax_record_dto_collection_query_parameters: OpenapiClient::AppliedItemTaxRecordDtoCollectionQueryParameters.new # AppliedItemTaxRecordDtoCollectionQueryParameters | 
}

begin
  # Get the count of taxes for a billable line.
  result = api_instance.get_billable_line_taxes_count(tenant_id, billable_line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillableLineTaxesApi->get_billable_line_taxes_count: #{e}"
end
```

#### Using the get_billable_line_taxes_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_billable_line_taxes_count_with_http_info(tenant_id, billable_line_id, opts)

```ruby
begin
  # Get the count of taxes for a billable line.
  data, status_code, headers = api_instance.get_billable_line_taxes_count_with_http_info(tenant_id, billable_line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillableLineTaxesApi->get_billable_line_taxes_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **billable_line_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **applied_item_tax_record_dto_collection_query_parameters** | [**AppliedItemTaxRecordDtoCollectionQueryParameters**](AppliedItemTaxRecordDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_billable_line_tax_async

> <EmptyEnvelope> patch_billable_line_tax_async(tenant_id, billable_line_id, tax_id, opts)

Patch a billable line tax

Partially updates a billable line tax.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillableLineTaxesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
billable_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tax_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a billable line tax
  result = api_instance.patch_billable_line_tax_async(tenant_id, billable_line_id, tax_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillableLineTaxesApi->patch_billable_line_tax_async: #{e}"
end
```

#### Using the patch_billable_line_tax_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_billable_line_tax_async_with_http_info(tenant_id, billable_line_id, tax_id, opts)

```ruby
begin
  # Patch a billable line tax
  data, status_code, headers = api_instance.patch_billable_line_tax_async_with_http_info(tenant_id, billable_line_id, tax_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillableLineTaxesApi->patch_billable_line_tax_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **billable_line_id** | **String** |  |  |
| **tax_id** | **String** |  |  |
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


## update_billable_line_tax

> <EmptyEnvelope> update_billable_line_tax(tenant_id, billable_line_id, tax_id, opts)

Update a tax for a billable line.

Updates the specified tax entry for the billable line.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillableLineTaxesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
billable_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tax_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  applied_item_tax_record_update_dto: OpenapiClient::AppliedItemTaxRecordUpdateDto.new # AppliedItemTaxRecordUpdateDto | 
}

begin
  # Update a tax for a billable line.
  result = api_instance.update_billable_line_tax(tenant_id, billable_line_id, tax_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillableLineTaxesApi->update_billable_line_tax: #{e}"
end
```

#### Using the update_billable_line_tax_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_billable_line_tax_with_http_info(tenant_id, billable_line_id, tax_id, opts)

```ruby
begin
  # Update a tax for a billable line.
  data, status_code, headers = api_instance.update_billable_line_tax_with_http_info(tenant_id, billable_line_id, tax_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillableLineTaxesApi->update_billable_line_tax_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **billable_line_id** | **String** |  |  |
| **tax_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **applied_item_tax_record_update_dto** | [**AppliedItemTaxRecordUpdateDto**](AppliedItemTaxRecordUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

