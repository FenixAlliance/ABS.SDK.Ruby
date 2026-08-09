# OpenapiClient::JobOfferFieldsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_job_offer_field_async**](JobOfferFieldsApi.md#create_job_offer_field_async) | **POST** /api/v2/HrmsService/JobOfferFields | Create a job offer field |
| [**delete_job_offer_field_async**](JobOfferFieldsApi.md#delete_job_offer_field_async) | **DELETE** /api/v2/HrmsService/JobOfferFields/{jobOfferFieldId} | Delete a job offer field |
| [**get_job_offer_field_by_id_async**](JobOfferFieldsApi.md#get_job_offer_field_by_id_async) | **GET** /api/v2/HrmsService/JobOfferFields/{jobOfferFieldId} | Get job offer field by ID |
| [**get_job_offer_fields_async**](JobOfferFieldsApi.md#get_job_offer_fields_async) | **GET** /api/v2/HrmsService/JobOfferFields | Get job offer fields |
| [**get_job_offer_fields_count_async**](JobOfferFieldsApi.md#get_job_offer_fields_count_async) | **GET** /api/v2/HrmsService/JobOfferFields/Count | Count job offer fields |
| [**patch_job_offer_field_async**](JobOfferFieldsApi.md#patch_job_offer_field_async) | **PATCH** /api/v2/HrmsService/JobOfferFields/{jobOfferFieldId} | Patch a job offer field |
| [**update_job_offer_field_async**](JobOfferFieldsApi.md#update_job_offer_field_async) | **PUT** /api/v2/HrmsService/JobOfferFields/{jobOfferFieldId} | Update a job offer field |


## create_job_offer_field_async

> <EmptyEnvelope> create_job_offer_field_async(tenant_id, opts)

Create a job offer field

Links a job field to a job offer for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobOfferFieldsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  job_offer_field_record_create_dto: OpenapiClient::JobOfferFieldRecordCreateDto.new({job_field_id: 'job_field_id_example'}) # JobOfferFieldRecordCreateDto | 
}

begin
  # Create a job offer field
  result = api_instance.create_job_offer_field_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOfferFieldsApi->create_job_offer_field_async: #{e}"
end
```

#### Using the create_job_offer_field_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_job_offer_field_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a job offer field
  data, status_code, headers = api_instance.create_job_offer_field_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOfferFieldsApi->create_job_offer_field_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **job_offer_field_record_create_dto** | [**JobOfferFieldRecordCreateDto**](JobOfferFieldRecordCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_job_offer_field_async

> <EmptyEnvelope> delete_job_offer_field_async(tenant_id, job_offer_field_id, opts)

Delete a job offer field

Removes a job-offer field link record for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobOfferFieldsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_offer_field_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a job offer field
  result = api_instance.delete_job_offer_field_async(tenant_id, job_offer_field_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOfferFieldsApi->delete_job_offer_field_async: #{e}"
end
```

#### Using the delete_job_offer_field_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_job_offer_field_async_with_http_info(tenant_id, job_offer_field_id, opts)

```ruby
begin
  # Delete a job offer field
  data, status_code, headers = api_instance.delete_job_offer_field_async_with_http_info(tenant_id, job_offer_field_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOfferFieldsApi->delete_job_offer_field_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_offer_field_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_job_offer_field_by_id_async

> <JobOfferFieldRecordDtoEnvelope> get_job_offer_field_by_id_async(tenant_id, job_offer_field_id, opts)

Get job offer field by ID

Retrieves a specific job-offer field link record by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobOfferFieldsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_offer_field_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get job offer field by ID
  result = api_instance.get_job_offer_field_by_id_async(tenant_id, job_offer_field_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOfferFieldsApi->get_job_offer_field_by_id_async: #{e}"
end
```

#### Using the get_job_offer_field_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JobOfferFieldRecordDtoEnvelope>, Integer, Hash)> get_job_offer_field_by_id_async_with_http_info(tenant_id, job_offer_field_id, opts)

```ruby
begin
  # Get job offer field by ID
  data, status_code, headers = api_instance.get_job_offer_field_by_id_async_with_http_info(tenant_id, job_offer_field_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JobOfferFieldRecordDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOfferFieldsApi->get_job_offer_field_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_offer_field_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**JobOfferFieldRecordDtoEnvelope**](JobOfferFieldRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_job_offer_fields_async

> <JobOfferFieldRecordDtoListEnvelope> get_job_offer_fields_async(tenant_id, opts)

Get job offer fields

Retrieves job-offer field link records for the tenant. Filter with `$filter=JobOfferId eq '...'` or `JobFieldId eq '...'`.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobOfferFieldsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  job_offer_field_record_dto_collection_query_parameters: OpenapiClient::JobOfferFieldRecordDtoCollectionQueryParameters.new # JobOfferFieldRecordDtoCollectionQueryParameters | 
}

begin
  # Get job offer fields
  result = api_instance.get_job_offer_fields_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOfferFieldsApi->get_job_offer_fields_async: #{e}"
end
```

#### Using the get_job_offer_fields_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JobOfferFieldRecordDtoListEnvelope>, Integer, Hash)> get_job_offer_fields_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get job offer fields
  data, status_code, headers = api_instance.get_job_offer_fields_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JobOfferFieldRecordDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOfferFieldsApi->get_job_offer_fields_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **job_offer_field_record_dto_collection_query_parameters** | [**JobOfferFieldRecordDtoCollectionQueryParameters**](JobOfferFieldRecordDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**JobOfferFieldRecordDtoListEnvelope**](JobOfferFieldRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_job_offer_fields_count_async

> <Int32Envelope> get_job_offer_fields_count_async(tenant_id, opts)

Count job offer fields

Counts job-offer field link records for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobOfferFieldsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  job_offer_field_record_dto_collection_query_parameters: OpenapiClient::JobOfferFieldRecordDtoCollectionQueryParameters.new # JobOfferFieldRecordDtoCollectionQueryParameters | 
}

begin
  # Count job offer fields
  result = api_instance.get_job_offer_fields_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOfferFieldsApi->get_job_offer_fields_count_async: #{e}"
end
```

#### Using the get_job_offer_fields_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_job_offer_fields_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count job offer fields
  data, status_code, headers = api_instance.get_job_offer_fields_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOfferFieldsApi->get_job_offer_fields_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **job_offer_field_record_dto_collection_query_parameters** | [**JobOfferFieldRecordDtoCollectionQueryParameters**](JobOfferFieldRecordDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_job_offer_field_async

> <EmptyEnvelope> patch_job_offer_field_async(tenant_id, job_offer_field_id, opts)

Patch a job offer field

Partially updates an existing job-offer field link record for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobOfferFieldsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_offer_field_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a job offer field
  result = api_instance.patch_job_offer_field_async(tenant_id, job_offer_field_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOfferFieldsApi->patch_job_offer_field_async: #{e}"
end
```

#### Using the patch_job_offer_field_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_job_offer_field_async_with_http_info(tenant_id, job_offer_field_id, opts)

```ruby
begin
  # Patch a job offer field
  data, status_code, headers = api_instance.patch_job_offer_field_async_with_http_info(tenant_id, job_offer_field_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOfferFieldsApi->patch_job_offer_field_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_offer_field_id** | **String** |  |  |
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


## update_job_offer_field_async

> <EmptyEnvelope> update_job_offer_field_async(tenant_id, job_offer_field_id, opts)

Update a job offer field

Updates an existing job-offer field link record for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobOfferFieldsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_offer_field_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  job_offer_field_record_update_dto: OpenapiClient::JobOfferFieldRecordUpdateDto.new # JobOfferFieldRecordUpdateDto | 
}

begin
  # Update a job offer field
  result = api_instance.update_job_offer_field_async(tenant_id, job_offer_field_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOfferFieldsApi->update_job_offer_field_async: #{e}"
end
```

#### Using the update_job_offer_field_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_job_offer_field_async_with_http_info(tenant_id, job_offer_field_id, opts)

```ruby
begin
  # Update a job offer field
  data, status_code, headers = api_instance.update_job_offer_field_async_with_http_info(tenant_id, job_offer_field_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOfferFieldsApi->update_job_offer_field_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_offer_field_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **job_offer_field_record_update_dto** | [**JobOfferFieldRecordUpdateDto**](JobOfferFieldRecordUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

