# OpenapiClient::FinancialBooksApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_financial_book_async**](FinancialBooksApi.md#create_financial_book_async) | **POST** /api/v2/AccountingService/FinancialBooks | Creates a new financial book |
| [**delete_financial_book_async**](FinancialBooksApi.md#delete_financial_book_async) | **DELETE** /api/v2/AccountingService/FinancialBooks/{financialBookId} | Deletes an existing financial book |
| [**get_financial_book_details_async**](FinancialBooksApi.md#get_financial_book_details_async) | **GET** /api/v2/AccountingService/FinancialBooks/{financialBookId} | Gets the details of a specific financial book |
| [**get_financial_books_async**](FinancialBooksApi.md#get_financial_books_async) | **GET** /api/v2/AccountingService/FinancialBooks | Get all financial books for a tenant |
| [**get_financial_books_count_async**](FinancialBooksApi.md#get_financial_books_count_async) | **GET** /api/v2/AccountingService/FinancialBooks/Count | Get the count of financial books |
| [**patch_financial_book_async**](FinancialBooksApi.md#patch_financial_book_async) | **PATCH** /api/v2/AccountingService/FinancialBooks/{financialBookId} | Patch a financial book |
| [**update_financial_book_async**](FinancialBooksApi.md#update_financial_book_async) | **PUT** /api/v2/AccountingService/FinancialBooks/{financialBookId} | Updates an existing financial book |


## create_financial_book_async

> <EmptyEnvelope> create_financial_book_async(tenant_id, financial_book_create_dto, opts)

Creates a new financial book

Creates a new financial book.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FinancialBooksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
financial_book_create_dto = OpenapiClient::FinancialBookCreateDto.new({name: 'name_example'}) # FinancialBookCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Creates a new financial book
  result = api_instance.create_financial_book_async(tenant_id, financial_book_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FinancialBooksApi->create_financial_book_async: #{e}"
end
```

#### Using the create_financial_book_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_financial_book_async_with_http_info(tenant_id, financial_book_create_dto, opts)

```ruby
begin
  # Creates a new financial book
  data, status_code, headers = api_instance.create_financial_book_async_with_http_info(tenant_id, financial_book_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FinancialBooksApi->create_financial_book_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **financial_book_create_dto** | [**FinancialBookCreateDto**](FinancialBookCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_financial_book_async

> <EmptyEnvelope> delete_financial_book_async(tenant_id, financial_book_id, opts)

Deletes an existing financial book

Deletes an existing financial book.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FinancialBooksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
financial_book_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes an existing financial book
  result = api_instance.delete_financial_book_async(tenant_id, financial_book_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FinancialBooksApi->delete_financial_book_async: #{e}"
end
```

#### Using the delete_financial_book_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_financial_book_async_with_http_info(tenant_id, financial_book_id, opts)

```ruby
begin
  # Deletes an existing financial book
  data, status_code, headers = api_instance.delete_financial_book_async_with_http_info(tenant_id, financial_book_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FinancialBooksApi->delete_financial_book_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **financial_book_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_financial_book_details_async

> <FinancialBookDtoEnvelope> get_financial_book_details_async(tenant_id, financial_book_id, opts)

Gets the details of a specific financial book

Gets the details of a specific financial book.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FinancialBooksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
financial_book_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the details of a specific financial book
  result = api_instance.get_financial_book_details_async(tenant_id, financial_book_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FinancialBooksApi->get_financial_book_details_async: #{e}"
end
```

#### Using the get_financial_book_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FinancialBookDtoEnvelope>, Integer, Hash)> get_financial_book_details_async_with_http_info(tenant_id, financial_book_id, opts)

```ruby
begin
  # Gets the details of a specific financial book
  data, status_code, headers = api_instance.get_financial_book_details_async_with_http_info(tenant_id, financial_book_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FinancialBookDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FinancialBooksApi->get_financial_book_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **financial_book_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**FinancialBookDtoEnvelope**](FinancialBookDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_financial_books_async

> <FinancialBookDtoListEnvelope> get_financial_books_async(tenant_id, opts)

Get all financial books for a tenant

Retrieves all financial books for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FinancialBooksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  financial_book_dto_collection_query_parameters: OpenapiClient::FinancialBookDtoCollectionQueryParameters.new # FinancialBookDtoCollectionQueryParameters | 
}

begin
  # Get all financial books for a tenant
  result = api_instance.get_financial_books_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FinancialBooksApi->get_financial_books_async: #{e}"
end
```

#### Using the get_financial_books_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FinancialBookDtoListEnvelope>, Integer, Hash)> get_financial_books_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all financial books for a tenant
  data, status_code, headers = api_instance.get_financial_books_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FinancialBookDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FinancialBooksApi->get_financial_books_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **financial_book_dto_collection_query_parameters** | [**FinancialBookDtoCollectionQueryParameters**](FinancialBookDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**FinancialBookDtoListEnvelope**](FinancialBookDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_financial_books_count_async

> <Int32Envelope> get_financial_books_count_async(tenant_id, opts)

Get the count of financial books

Get the count of financial books.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FinancialBooksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  financial_book_dto_collection_query_parameters: OpenapiClient::FinancialBookDtoCollectionQueryParameters.new # FinancialBookDtoCollectionQueryParameters | 
}

begin
  # Get the count of financial books
  result = api_instance.get_financial_books_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FinancialBooksApi->get_financial_books_count_async: #{e}"
end
```

#### Using the get_financial_books_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_financial_books_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of financial books
  data, status_code, headers = api_instance.get_financial_books_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FinancialBooksApi->get_financial_books_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **financial_book_dto_collection_query_parameters** | [**FinancialBookDtoCollectionQueryParameters**](FinancialBookDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_financial_book_async

> <EmptyEnvelope> patch_financial_book_async(tenant_id, financial_book_id, opts)

Patch a financial book

Partially updates a financial book.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FinancialBooksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
financial_book_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a financial book
  result = api_instance.patch_financial_book_async(tenant_id, financial_book_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FinancialBooksApi->patch_financial_book_async: #{e}"
end
```

#### Using the patch_financial_book_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_financial_book_async_with_http_info(tenant_id, financial_book_id, opts)

```ruby
begin
  # Patch a financial book
  data, status_code, headers = api_instance.patch_financial_book_async_with_http_info(tenant_id, financial_book_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FinancialBooksApi->patch_financial_book_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **financial_book_id** | **String** |  |  |
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


## update_financial_book_async

> <EmptyEnvelope> update_financial_book_async(tenant_id, financial_book_id, financial_book_update_dto, opts)

Updates an existing financial book

Updates an existing financial book.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FinancialBooksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
financial_book_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
financial_book_update_dto = OpenapiClient::FinancialBookUpdateDto.new # FinancialBookUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Updates an existing financial book
  result = api_instance.update_financial_book_async(tenant_id, financial_book_id, financial_book_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FinancialBooksApi->update_financial_book_async: #{e}"
end
```

#### Using the update_financial_book_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_financial_book_async_with_http_info(tenant_id, financial_book_id, financial_book_update_dto, opts)

```ruby
begin
  # Updates an existing financial book
  data, status_code, headers = api_instance.update_financial_book_async_with_http_info(tenant_id, financial_book_id, financial_book_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FinancialBooksApi->update_financial_book_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **financial_book_id** | **String** |  |  |
| **financial_book_update_dto** | [**FinancialBookUpdateDto**](FinancialBookUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

