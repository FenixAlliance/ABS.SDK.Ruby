# OpenapiClient::TransactionsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_transaction**](TransactionsApi.md#create_transaction) | **POST** /api/v2/AccountingService/Transactions | Create a transaction |
| [**create_transaction_category**](TransactionsApi.md#create_transaction_category) | **POST** /api/v2/AccountingService/Transactions/Categories | Create a transaction category |
| [**delete_transaction**](TransactionsApi.md#delete_transaction) | **DELETE** /api/v2/AccountingService/Transactions/{transactionId} | Delete a transaction |
| [**delete_transaction_category**](TransactionsApi.md#delete_transaction_category) | **DELETE** /api/v2/AccountingService/Transactions/Categories/{categoryId} | Delete a transaction category |
| [**get_transaction**](TransactionsApi.md#get_transaction) | **GET** /api/v2/AccountingService/Transactions/{transactionId} | Get transaction by ID |
| [**get_transaction_categories**](TransactionsApi.md#get_transaction_categories) | **GET** /api/v2/AccountingService/Transactions/Categories | Get all transaction categories |
| [**get_transaction_categories_count**](TransactionsApi.md#get_transaction_categories_count) | **GET** /api/v2/AccountingService/Transactions/Categories/Count | Get transaction categories count |
| [**get_transaction_category**](TransactionsApi.md#get_transaction_category) | **GET** /api/v2/AccountingService/Transactions/Categories/{categoryId} | Get transaction category by ID |
| [**get_transactions**](TransactionsApi.md#get_transactions) | **GET** /api/v2/AccountingService/Transactions | Get all transactions for a tenant |
| [**get_transactions_count**](TransactionsApi.md#get_transactions_count) | **GET** /api/v2/AccountingService/Transactions/Count | Get transactions count |
| [**patch_transaction**](TransactionsApi.md#patch_transaction) | **PATCH** /api/v2/AccountingService/Transactions/{transactionId} | Patch a transaction |
| [**patch_transaction_category**](TransactionsApi.md#patch_transaction_category) | **PATCH** /api/v2/AccountingService/Transactions/Categories/{categoryId} | Patch a transaction category |
| [**update_transaction**](TransactionsApi.md#update_transaction) | **PUT** /api/v2/AccountingService/Transactions/{transactionId} | Update a transaction |
| [**update_transaction_category**](TransactionsApi.md#update_transaction_category) | **PUT** /api/v2/AccountingService/Transactions/Categories/{categoryId} | Update a transaction category |


## create_transaction

> <TransactionDtoEnvelope> create_transaction(tenant_id, opts)

Create a transaction

Creates a new transaction for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TransactionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  transaction_create_dto: OpenapiClient::TransactionCreateDto.new # TransactionCreateDto | 
}

begin
  # Create a transaction
  result = api_instance.create_transaction(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->create_transaction: #{e}"
end
```

#### Using the create_transaction_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TransactionDtoEnvelope>, Integer, Hash)> create_transaction_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a transaction
  data, status_code, headers = api_instance.create_transaction_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TransactionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->create_transaction_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **transaction_create_dto** | [**TransactionCreateDto**](TransactionCreateDto.md) |  | [optional] |

### Return type

[**TransactionDtoEnvelope**](TransactionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_transaction_category

> <TransactionCategoryDtoEnvelope> create_transaction_category(tenant_id, opts)

Create a transaction category

Creates a new transaction category for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TransactionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  transaction_category_create_dto: OpenapiClient::TransactionCategoryCreateDto.new # TransactionCategoryCreateDto | 
}

begin
  # Create a transaction category
  result = api_instance.create_transaction_category(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->create_transaction_category: #{e}"
end
```

#### Using the create_transaction_category_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TransactionCategoryDtoEnvelope>, Integer, Hash)> create_transaction_category_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a transaction category
  data, status_code, headers = api_instance.create_transaction_category_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TransactionCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->create_transaction_category_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **transaction_category_create_dto** | [**TransactionCategoryCreateDto**](TransactionCategoryCreateDto.md) |  | [optional] |

### Return type

[**TransactionCategoryDtoEnvelope**](TransactionCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_transaction

> <TransactionDtoEnvelope> delete_transaction(tenant_id, transaction_id, opts)

Delete a transaction

Deletes a transaction by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TransactionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transaction_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a transaction
  result = api_instance.delete_transaction(tenant_id, transaction_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->delete_transaction: #{e}"
end
```

#### Using the delete_transaction_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TransactionDtoEnvelope>, Integer, Hash)> delete_transaction_with_http_info(tenant_id, transaction_id, opts)

```ruby
begin
  # Delete a transaction
  data, status_code, headers = api_instance.delete_transaction_with_http_info(tenant_id, transaction_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TransactionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->delete_transaction_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **transaction_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TransactionDtoEnvelope**](TransactionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_transaction_category

> <TransactionCategoryDtoEnvelope> delete_transaction_category(tenant_id, category_id, opts)

Delete a transaction category

Deletes a transaction category by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TransactionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a transaction category
  result = api_instance.delete_transaction_category(tenant_id, category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->delete_transaction_category: #{e}"
end
```

#### Using the delete_transaction_category_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TransactionCategoryDtoEnvelope>, Integer, Hash)> delete_transaction_category_with_http_info(tenant_id, category_id, opts)

```ruby
begin
  # Delete a transaction category
  data, status_code, headers = api_instance.delete_transaction_category_with_http_info(tenant_id, category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TransactionCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->delete_transaction_category_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TransactionCategoryDtoEnvelope**](TransactionCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_transaction

> <TransactionDtoEnvelope> get_transaction(tenant_id, transaction_id, opts)

Get transaction by ID

Retrieves a specific transaction by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TransactionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transaction_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get transaction by ID
  result = api_instance.get_transaction(tenant_id, transaction_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->get_transaction: #{e}"
end
```

#### Using the get_transaction_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TransactionDtoEnvelope>, Integer, Hash)> get_transaction_with_http_info(tenant_id, transaction_id, opts)

```ruby
begin
  # Get transaction by ID
  data, status_code, headers = api_instance.get_transaction_with_http_info(tenant_id, transaction_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TransactionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->get_transaction_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **transaction_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TransactionDtoEnvelope**](TransactionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_transaction_categories

> <TransactionCategoryDtoListEnvelope> get_transaction_categories(tenant_id, opts)

Get all transaction categories

Retrieves all transaction categories for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TransactionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  transaction_category_dto_collection_query_parameters: OpenapiClient::TransactionCategoryDtoCollectionQueryParameters.new # TransactionCategoryDtoCollectionQueryParameters | 
}

begin
  # Get all transaction categories
  result = api_instance.get_transaction_categories(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->get_transaction_categories: #{e}"
end
```

#### Using the get_transaction_categories_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TransactionCategoryDtoListEnvelope>, Integer, Hash)> get_transaction_categories_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all transaction categories
  data, status_code, headers = api_instance.get_transaction_categories_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TransactionCategoryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->get_transaction_categories_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **transaction_category_dto_collection_query_parameters** | [**TransactionCategoryDtoCollectionQueryParameters**](TransactionCategoryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**TransactionCategoryDtoListEnvelope**](TransactionCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_transaction_categories_count

> <Int32Envelope> get_transaction_categories_count(tenant_id, opts)

Get transaction categories count

Returns total number of transaction categories for the tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TransactionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  transaction_category_dto_collection_query_parameters: OpenapiClient::TransactionCategoryDtoCollectionQueryParameters.new # TransactionCategoryDtoCollectionQueryParameters | 
}

begin
  # Get transaction categories count
  result = api_instance.get_transaction_categories_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->get_transaction_categories_count: #{e}"
end
```

#### Using the get_transaction_categories_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_transaction_categories_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get transaction categories count
  data, status_code, headers = api_instance.get_transaction_categories_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->get_transaction_categories_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **transaction_category_dto_collection_query_parameters** | [**TransactionCategoryDtoCollectionQueryParameters**](TransactionCategoryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_transaction_category

> <TransactionCategoryDtoEnvelope> get_transaction_category(tenant_id, category_id, opts)

Get transaction category by ID

Retrieves a specific transaction category by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TransactionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get transaction category by ID
  result = api_instance.get_transaction_category(tenant_id, category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->get_transaction_category: #{e}"
end
```

#### Using the get_transaction_category_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TransactionCategoryDtoEnvelope>, Integer, Hash)> get_transaction_category_with_http_info(tenant_id, category_id, opts)

```ruby
begin
  # Get transaction category by ID
  data, status_code, headers = api_instance.get_transaction_category_with_http_info(tenant_id, category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TransactionCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->get_transaction_category_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TransactionCategoryDtoEnvelope**](TransactionCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_transactions

> <TransactionDtoListEnvelope> get_transactions(tenant_id, opts)

Get all transactions for a tenant

Retrieves all transactions for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TransactionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  transaction_dto_collection_query_parameters: OpenapiClient::TransactionDtoCollectionQueryParameters.new # TransactionDtoCollectionQueryParameters | 
}

begin
  # Get all transactions for a tenant
  result = api_instance.get_transactions(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->get_transactions: #{e}"
end
```

#### Using the get_transactions_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TransactionDtoListEnvelope>, Integer, Hash)> get_transactions_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all transactions for a tenant
  data, status_code, headers = api_instance.get_transactions_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TransactionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->get_transactions_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **transaction_dto_collection_query_parameters** | [**TransactionDtoCollectionQueryParameters**](TransactionDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**TransactionDtoListEnvelope**](TransactionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_transactions_count

> <Int32Envelope> get_transactions_count(tenant_id, opts)

Get transactions count

Returns total number of transactions for the tenant with OData filter support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TransactionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  transaction_dto_collection_query_parameters: OpenapiClient::TransactionDtoCollectionQueryParameters.new # TransactionDtoCollectionQueryParameters | 
}

begin
  # Get transactions count
  result = api_instance.get_transactions_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->get_transactions_count: #{e}"
end
```

#### Using the get_transactions_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_transactions_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get transactions count
  data, status_code, headers = api_instance.get_transactions_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->get_transactions_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **transaction_dto_collection_query_parameters** | [**TransactionDtoCollectionQueryParameters**](TransactionDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_transaction

> <EmptyEnvelope> patch_transaction(tenant_id, transaction_id, opts)

Patch a transaction

Partially updates an existing transaction identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TransactionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transaction_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a transaction
  result = api_instance.patch_transaction(tenant_id, transaction_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->patch_transaction: #{e}"
end
```

#### Using the patch_transaction_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_transaction_with_http_info(tenant_id, transaction_id, opts)

```ruby
begin
  # Patch a transaction
  data, status_code, headers = api_instance.patch_transaction_with_http_info(tenant_id, transaction_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->patch_transaction_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **transaction_id** | **String** |  |  |
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


## patch_transaction_category

> <EmptyEnvelope> patch_transaction_category(tenant_id, category_id, opts)

Patch a transaction category

Partially updates an existing transaction category identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TransactionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a transaction category
  result = api_instance.patch_transaction_category(tenant_id, category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->patch_transaction_category: #{e}"
end
```

#### Using the patch_transaction_category_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_transaction_category_with_http_info(tenant_id, category_id, opts)

```ruby
begin
  # Patch a transaction category
  data, status_code, headers = api_instance.patch_transaction_category_with_http_info(tenant_id, category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->patch_transaction_category_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **category_id** | **String** |  |  |
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


## update_transaction

> <TransactionDtoEnvelope> update_transaction(tenant_id, transaction_id, opts)

Update a transaction

Updates an existing transaction with the provided data.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TransactionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transaction_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  transaction_update_dto: OpenapiClient::TransactionUpdateDto.new # TransactionUpdateDto | 
}

begin
  # Update a transaction
  result = api_instance.update_transaction(tenant_id, transaction_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->update_transaction: #{e}"
end
```

#### Using the update_transaction_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TransactionDtoEnvelope>, Integer, Hash)> update_transaction_with_http_info(tenant_id, transaction_id, opts)

```ruby
begin
  # Update a transaction
  data, status_code, headers = api_instance.update_transaction_with_http_info(tenant_id, transaction_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TransactionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->update_transaction_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **transaction_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **transaction_update_dto** | [**TransactionUpdateDto**](TransactionUpdateDto.md) |  | [optional] |

### Return type

[**TransactionDtoEnvelope**](TransactionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_transaction_category

> <TransactionCategoryDtoEnvelope> update_transaction_category(tenant_id, category_id, opts)

Update a transaction category

Updates an existing transaction category with the provided data.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TransactionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  transaction_category_update_dto: OpenapiClient::TransactionCategoryUpdateDto.new # TransactionCategoryUpdateDto | 
}

begin
  # Update a transaction category
  result = api_instance.update_transaction_category(tenant_id, category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->update_transaction_category: #{e}"
end
```

#### Using the update_transaction_category_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TransactionCategoryDtoEnvelope>, Integer, Hash)> update_transaction_category_with_http_info(tenant_id, category_id, opts)

```ruby
begin
  # Update a transaction category
  data, status_code, headers = api_instance.update_transaction_category_with_http_info(tenant_id, category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TransactionCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TransactionsApi->update_transaction_category_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **transaction_category_update_dto** | [**TransactionCategoryUpdateDto**](TransactionCategoryUpdateDto.md) |  | [optional] |

### Return type

[**TransactionCategoryDtoEnvelope**](TransactionCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

