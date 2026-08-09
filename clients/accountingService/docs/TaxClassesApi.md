# OpenapiClient::TaxClassesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_tax_class**](TaxClassesApi.md#create_tax_class) | **POST** /api/v2/AccountingService/TaxClasses | Create a tax class |
| [**delete_tax_class**](TaxClassesApi.md#delete_tax_class) | **DELETE** /api/v2/AccountingService/TaxClasses/{id} | Delete a tax class |
| [**get_tax_class**](TaxClassesApi.md#get_tax_class) | **GET** /api/v2/AccountingService/TaxClasses/{id} | Get tax class by ID |
| [**get_tax_classes**](TaxClassesApi.md#get_tax_classes) | **GET** /api/v2/AccountingService/TaxClasses | Get all tax classes for a tenant |
| [**get_tax_classes_count**](TaxClassesApi.md#get_tax_classes_count) | **GET** /api/v2/AccountingService/TaxClasses/Count | Get tax classes count |
| [**patch_tax_class**](TaxClassesApi.md#patch_tax_class) | **PATCH** /api/v2/AccountingService/TaxClasses/{id} | Patch a tax class |
| [**update_tax_class**](TaxClassesApi.md#update_tax_class) | **PUT** /api/v2/AccountingService/TaxClasses/{id} | Update a tax class |


## create_tax_class

> <EmptyEnvelope> create_tax_class(tenant_id, opts)

Create a tax class

Creates a new tax class for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxClassesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tax_class_create_dto: OpenapiClient::TaxClassCreateDto.new # TaxClassCreateDto | 
}

begin
  # Create a tax class
  result = api_instance.create_tax_class(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxClassesApi->create_tax_class: #{e}"
end
```

#### Using the create_tax_class_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tax_class_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a tax class
  data, status_code, headers = api_instance.create_tax_class_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxClassesApi->create_tax_class_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tax_class_create_dto** | [**TaxClassCreateDto**](TaxClassCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_tax_class

> <EmptyEnvelope> delete_tax_class(tenant_id, id, opts)

Delete a tax class

Deletes a tax class identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxClassesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tax class
  result = api_instance.delete_tax_class(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxClassesApi->delete_tax_class: #{e}"
end
```

#### Using the delete_tax_class_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tax_class_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a tax class
  data, status_code, headers = api_instance.delete_tax_class_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxClassesApi->delete_tax_class_with_http_info: #{e}"
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


## get_tax_class

> <TaxClassDtoEnvelope> get_tax_class(tenant_id, id, opts)

Get tax class by ID

Retrieves a specific tax class by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxClassesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get tax class by ID
  result = api_instance.get_tax_class(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxClassesApi->get_tax_class: #{e}"
end
```

#### Using the get_tax_class_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TaxClassDtoEnvelope>, Integer, Hash)> get_tax_class_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get tax class by ID
  data, status_code, headers = api_instance.get_tax_class_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TaxClassDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxClassesApi->get_tax_class_with_http_info: #{e}"
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

[**TaxClassDtoEnvelope**](TaxClassDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tax_classes

> <TaxClassDtoListEnvelope> get_tax_classes(tenant_id, opts)

Get all tax classes for a tenant

Retrieves all tax classes for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxClassesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tax_class_dto_collection_query_parameters: OpenapiClient::TaxClassDtoCollectionQueryParameters.new # TaxClassDtoCollectionQueryParameters | 
}

begin
  # Get all tax classes for a tenant
  result = api_instance.get_tax_classes(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxClassesApi->get_tax_classes: #{e}"
end
```

#### Using the get_tax_classes_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TaxClassDtoListEnvelope>, Integer, Hash)> get_tax_classes_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all tax classes for a tenant
  data, status_code, headers = api_instance.get_tax_classes_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TaxClassDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxClassesApi->get_tax_classes_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tax_class_dto_collection_query_parameters** | [**TaxClassDtoCollectionQueryParameters**](TaxClassDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**TaxClassDtoListEnvelope**](TaxClassDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_tax_classes_count

> <Int32Envelope> get_tax_classes_count(tenant_id, opts)

Get tax classes count

Returns the count of tax classes for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxClassesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tax_class_dto_collection_query_parameters: OpenapiClient::TaxClassDtoCollectionQueryParameters.new # TaxClassDtoCollectionQueryParameters | 
}

begin
  # Get tax classes count
  result = api_instance.get_tax_classes_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxClassesApi->get_tax_classes_count: #{e}"
end
```

#### Using the get_tax_classes_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tax_classes_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get tax classes count
  data, status_code, headers = api_instance.get_tax_classes_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxClassesApi->get_tax_classes_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tax_class_dto_collection_query_parameters** | [**TaxClassDtoCollectionQueryParameters**](TaxClassDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_tax_class

> <EmptyEnvelope> patch_tax_class(tenant_id, id, opts)

Patch a tax class

Partially updates an existing tax class identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxClassesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a tax class
  result = api_instance.patch_tax_class(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxClassesApi->patch_tax_class: #{e}"
end
```

#### Using the patch_tax_class_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_tax_class_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a tax class
  data, status_code, headers = api_instance.patch_tax_class_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxClassesApi->patch_tax_class_with_http_info: #{e}"
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


## update_tax_class

> <EmptyEnvelope> update_tax_class(tenant_id, id, opts)

Update a tax class

Updates an existing tax class identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxClassesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tax_class_update_dto: OpenapiClient::TaxClassUpdateDto.new # TaxClassUpdateDto | 
}

begin
  # Update a tax class
  result = api_instance.update_tax_class(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxClassesApi->update_tax_class: #{e}"
end
```

#### Using the update_tax_class_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tax_class_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a tax class
  data, status_code, headers = api_instance.update_tax_class_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxClassesApi->update_tax_class_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tax_class_update_dto** | [**TaxClassUpdateDto**](TaxClassUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

