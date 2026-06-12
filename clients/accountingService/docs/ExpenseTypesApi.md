# OpenapiClient::ExpenseTypesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_expense_type**](ExpenseTypesApi.md#create_expense_type) | **POST** /api/v2/AccountingService/ExpenseTypes | Create an expense type |
| [**delete_expense_type**](ExpenseTypesApi.md#delete_expense_type) | **DELETE** /api/v2/AccountingService/ExpenseTypes/{expenseTypeId} | Delete an expense type |
| [**get_expense_type**](ExpenseTypesApi.md#get_expense_type) | **GET** /api/v2/AccountingService/ExpenseTypes/{expenseTypeId} | Get an expense type by id |
| [**get_expense_types**](ExpenseTypesApi.md#get_expense_types) | **GET** /api/v2/AccountingService/ExpenseTypes | Get all expense types for a tenant |
| [**get_expense_types_count**](ExpenseTypesApi.md#get_expense_types_count) | **GET** /api/v2/AccountingService/ExpenseTypes/Count | Get the count of expense types for a tenant |
| [**patch_expense_type**](ExpenseTypesApi.md#patch_expense_type) | **PATCH** /api/v2/AccountingService/ExpenseTypes/{expenseTypeId} | Patch an expense type |
| [**update_expense_type**](ExpenseTypesApi.md#update_expense_type) | **PUT** /api/v2/AccountingService/ExpenseTypes/{expenseTypeId} | Update an expense type |


## create_expense_type

> <EmptyEnvelope> create_expense_type(tenant_id, expense_type_create_dto, opts)

Create an expense type

Creates a new expense type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ExpenseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
expense_type_create_dto = OpenapiClient::ExpenseTypeCreateDto.new # ExpenseTypeCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create an expense type
  result = api_instance.create_expense_type(tenant_id, expense_type_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseTypesApi->create_expense_type: #{e}"
end
```

#### Using the create_expense_type_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_expense_type_with_http_info(tenant_id, expense_type_create_dto, opts)

```ruby
begin
  # Create an expense type
  data, status_code, headers = api_instance.create_expense_type_with_http_info(tenant_id, expense_type_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseTypesApi->create_expense_type_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **expense_type_create_dto** | [**ExpenseTypeCreateDto**](ExpenseTypeCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_expense_type

> <EmptyEnvelope> delete_expense_type(tenant_id, expense_type_id, opts)

Delete an expense type

Deletes an expense type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ExpenseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
expense_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an expense type
  result = api_instance.delete_expense_type(tenant_id, expense_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseTypesApi->delete_expense_type: #{e}"
end
```

#### Using the delete_expense_type_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_expense_type_with_http_info(tenant_id, expense_type_id, opts)

```ruby
begin
  # Delete an expense type
  data, status_code, headers = api_instance.delete_expense_type_with_http_info(tenant_id, expense_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseTypesApi->delete_expense_type_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **expense_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_expense_type

> <ExpenseTypeDtoEnvelope> get_expense_type(tenant_id, expense_type_id, opts)

Get an expense type by id

Retrieves an expense type by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ExpenseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
expense_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get an expense type by id
  result = api_instance.get_expense_type(tenant_id, expense_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseTypesApi->get_expense_type: #{e}"
end
```

#### Using the get_expense_type_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExpenseTypeDtoEnvelope>, Integer, Hash)> get_expense_type_with_http_info(tenant_id, expense_type_id, opts)

```ruby
begin
  # Get an expense type by id
  data, status_code, headers = api_instance.get_expense_type_with_http_info(tenant_id, expense_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExpenseTypeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseTypesApi->get_expense_type_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **expense_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ExpenseTypeDtoEnvelope**](ExpenseTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_expense_types

> <ExpenseTypeDtoListEnvelope> get_expense_types(tenant_id, opts)

Get all expense types for a tenant

Retrieves all expense types for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ExpenseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all expense types for a tenant
  result = api_instance.get_expense_types(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseTypesApi->get_expense_types: #{e}"
end
```

#### Using the get_expense_types_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExpenseTypeDtoListEnvelope>, Integer, Hash)> get_expense_types_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all expense types for a tenant
  data, status_code, headers = api_instance.get_expense_types_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExpenseTypeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseTypesApi->get_expense_types_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ExpenseTypeDtoListEnvelope**](ExpenseTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_expense_types_count

> <Int32Envelope> get_expense_types_count(tenant_id, opts)

Get the count of expense types for a tenant

Retrieves the count of expense types for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ExpenseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of expense types for a tenant
  result = api_instance.get_expense_types_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseTypesApi->get_expense_types_count: #{e}"
end
```

#### Using the get_expense_types_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_expense_types_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of expense types for a tenant
  data, status_code, headers = api_instance.get_expense_types_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseTypesApi->get_expense_types_count_with_http_info: #{e}"
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


## patch_expense_type

> <EmptyEnvelope> patch_expense_type(tenant_id, expense_type_id, opts)

Patch an expense type

Partially updates an existing expense type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ExpenseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
expense_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch an expense type
  result = api_instance.patch_expense_type(tenant_id, expense_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseTypesApi->patch_expense_type: #{e}"
end
```

#### Using the patch_expense_type_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_expense_type_with_http_info(tenant_id, expense_type_id, opts)

```ruby
begin
  # Patch an expense type
  data, status_code, headers = api_instance.patch_expense_type_with_http_info(tenant_id, expense_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseTypesApi->patch_expense_type_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **expense_type_id** | **String** |  |  |
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


## update_expense_type

> <EmptyEnvelope> update_expense_type(tenant_id, expense_type_id, expense_type_update_dto, opts)

Update an expense type

Updates an existing expense type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ExpenseTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
expense_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
expense_type_update_dto = OpenapiClient::ExpenseTypeUpdateDto.new # ExpenseTypeUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update an expense type
  result = api_instance.update_expense_type(tenant_id, expense_type_id, expense_type_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseTypesApi->update_expense_type: #{e}"
end
```

#### Using the update_expense_type_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_expense_type_with_http_info(tenant_id, expense_type_id, expense_type_update_dto, opts)

```ruby
begin
  # Update an expense type
  data, status_code, headers = api_instance.update_expense_type_with_http_info(tenant_id, expense_type_id, expense_type_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseTypesApi->update_expense_type_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **expense_type_id** | **String** |  |  |
| **expense_type_update_dto** | [**ExpenseTypeUpdateDto**](ExpenseTypeUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

