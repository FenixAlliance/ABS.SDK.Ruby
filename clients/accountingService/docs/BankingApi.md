# OpenapiClient::BankingApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_bank**](BankingApi.md#create_bank) | **POST** /api/v2/AccountingService/Banking | Creates a new bank |
| [**create_bank_account**](BankingApi.md#create_bank_account) | **POST** /api/v2/AccountingService/Banking/{bankId}/Accounts | Creates a new bank account |
| [**create_bank_guarantee**](BankingApi.md#create_bank_guarantee) | **POST** /api/v2/AccountingService/Banking/{bankId}/Guarantees | Creates a new bank guarantee |
| [**create_bank_transaction**](BankingApi.md#create_bank_transaction) | **POST** /api/v2/AccountingService/Banking/{bankId}/Transactions | Creates a new bank transaction |
| [**delete_bank**](BankingApi.md#delete_bank) | **DELETE** /api/v2/AccountingService/Banking/{bankId} | Deletes a bank |
| [**delete_bank_account**](BankingApi.md#delete_bank_account) | **DELETE** /api/v2/AccountingService/Banking/{bankId}/Accounts/{accountId} | Deletes a bank account |
| [**delete_bank_guarantee**](BankingApi.md#delete_bank_guarantee) | **DELETE** /api/v2/AccountingService/Banking/{bankId}/Guarantees/{guaranteeId} | Deletes a bank guarantee |
| [**delete_bank_transaction**](BankingApi.md#delete_bank_transaction) | **DELETE** /api/v2/AccountingService/Banking/{bankId}/Transactions/{transactionId} | Deletes a bank transaction |
| [**get_bank**](BankingApi.md#get_bank) | **GET** /api/v2/AccountingService/Banking/{bankId} | Gets the current tenant bank |
| [**get_bank_account**](BankingApi.md#get_bank_account) | **GET** /api/v2/AccountingService/Banking/{bankId}/Accounts/{accountId} | Gets the current tenant bank account |
| [**get_bank_accounts**](BankingApi.md#get_bank_accounts) | **GET** /api/v2/AccountingService/Banking/{bankId}/Accounts | Gets the current tenant bank accounts |
| [**get_bank_accounts_count**](BankingApi.md#get_bank_accounts_count) | **GET** /api/v2/AccountingService/Banking/{bankId}/Accounts/Count | Gets the current tenant bank accounts count |
| [**get_bank_guarantee**](BankingApi.md#get_bank_guarantee) | **GET** /api/v2/AccountingService/Banking/{bankId}/Guarantees/{guaranteeId} | Gets the current tenant bank guarantee |
| [**get_bank_guarantees**](BankingApi.md#get_bank_guarantees) | **GET** /api/v2/AccountingService/Banking/{bankId}/Guarantees | Gets the current tenant bank guarantees |
| [**get_bank_guarantees_count**](BankingApi.md#get_bank_guarantees_count) | **GET** /api/v2/AccountingService/Banking/{bankId}/Guarantees/Count | Gets the current tenant bank guarantees count |
| [**get_bank_transaction**](BankingApi.md#get_bank_transaction) | **GET** /api/v2/AccountingService/Banking/{bankId}/Transactions/{transactionId} | Gets the current tenant bank transaction |
| [**get_bank_transactions**](BankingApi.md#get_bank_transactions) | **GET** /api/v2/AccountingService/Banking/{bankId}/Transactions | Gets the current tenant bank transactions |
| [**get_bank_transactions_count**](BankingApi.md#get_bank_transactions_count) | **GET** /api/v2/AccountingService/Banking/{bankId}/Transactions/Count | Gets the current tenant bank transactions count |
| [**get_banks**](BankingApi.md#get_banks) | **GET** /api/v2/AccountingService/Banking | Gets the current tenant banks |
| [**get_banks_count**](BankingApi.md#get_banks_count) | **GET** /api/v2/AccountingService/Banking/Count | Gets the current tenant banks count |
| [**patch_bank**](BankingApi.md#patch_bank) | **PATCH** /api/v2/AccountingService/Banking/{bankId} | Patches a bank |
| [**patch_bank_account**](BankingApi.md#patch_bank_account) | **PATCH** /api/v2/AccountingService/Banking/{bankId}/Accounts/{accountId} | Patches a bank account |
| [**patch_bank_guarantee**](BankingApi.md#patch_bank_guarantee) | **PATCH** /api/v2/AccountingService/Banking/{bankId}/Guarantees/{guaranteeId} | Patches a bank guarantee |
| [**patch_bank_transaction**](BankingApi.md#patch_bank_transaction) | **PATCH** /api/v2/AccountingService/Banking/{bankId}/Transactions/{transactionId} | Patches a bank transaction |
| [**update_bank**](BankingApi.md#update_bank) | **PUT** /api/v2/AccountingService/Banking/{bankId} | Updates a bank |
| [**update_bank_account**](BankingApi.md#update_bank_account) | **PUT** /api/v2/AccountingService/Banking/{bankId}/Accounts/{accountId} | Updates a bank account |
| [**update_bank_guarantee**](BankingApi.md#update_bank_guarantee) | **PUT** /api/v2/AccountingService/Banking/{bankId}/Guarantees/{guaranteeId} | Updates a bank guarantee |
| [**update_bank_transaction**](BankingApi.md#update_bank_transaction) | **PUT** /api/v2/AccountingService/Banking/{bankId}/Transactions/{transactionId} | Updates a bank transaction |


## create_bank

> <BankDtoEnvelope> create_bank(tenant_id, opts)

Creates a new bank

Create a new bank.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  bank_create_dto: OpenapiClient::BankCreateDto.new # BankCreateDto | 
}

begin
  # Creates a new bank
  result = api_instance.create_bank(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->create_bank: #{e}"
end
```

#### Using the create_bank_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BankDtoEnvelope>, Integer, Hash)> create_bank_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new bank
  data, status_code, headers = api_instance.create_bank_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BankDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->create_bank_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **bank_create_dto** | [**BankCreateDto**](BankCreateDto.md) |  | [optional] |

### Return type

[**BankDtoEnvelope**](BankDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_bank_account

> <BankAccountDtoEnvelope> create_bank_account(tenant_id, bank_id, opts)

Creates a new bank account

Create a new bank account.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  bank_account_create_dto: OpenapiClient::BankAccountCreateDto.new # BankAccountCreateDto | 
}

begin
  # Creates a new bank account
  result = api_instance.create_bank_account(tenant_id, bank_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->create_bank_account: #{e}"
end
```

#### Using the create_bank_account_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BankAccountDtoEnvelope>, Integer, Hash)> create_bank_account_with_http_info(tenant_id, bank_id, opts)

```ruby
begin
  # Creates a new bank account
  data, status_code, headers = api_instance.create_bank_account_with_http_info(tenant_id, bank_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BankAccountDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->create_bank_account_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **bank_account_create_dto** | [**BankAccountCreateDto**](BankAccountCreateDto.md) |  | [optional] |

### Return type

[**BankAccountDtoEnvelope**](BankAccountDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_bank_guarantee

> <BankGuaranteeDtoEnvelope> create_bank_guarantee(tenant_id, bank_id, opts)

Creates a new bank guarantee

Create a new bank guarantee.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  bank_guarantee_create_dto: OpenapiClient::BankGuaranteeCreateDto.new # BankGuaranteeCreateDto | 
}

begin
  # Creates a new bank guarantee
  result = api_instance.create_bank_guarantee(tenant_id, bank_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->create_bank_guarantee: #{e}"
end
```

#### Using the create_bank_guarantee_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BankGuaranteeDtoEnvelope>, Integer, Hash)> create_bank_guarantee_with_http_info(tenant_id, bank_id, opts)

```ruby
begin
  # Creates a new bank guarantee
  data, status_code, headers = api_instance.create_bank_guarantee_with_http_info(tenant_id, bank_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BankGuaranteeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->create_bank_guarantee_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **bank_guarantee_create_dto** | [**BankGuaranteeCreateDto**](BankGuaranteeCreateDto.md) |  | [optional] |

### Return type

[**BankGuaranteeDtoEnvelope**](BankGuaranteeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_bank_transaction

> <BankTransactionDtoEnvelope> create_bank_transaction(tenant_id, bank_id, opts)

Creates a new bank transaction

Create a new bank transaction.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  bank_transaction_create_dto: OpenapiClient::BankTransactionCreateDto.new # BankTransactionCreateDto | 
}

begin
  # Creates a new bank transaction
  result = api_instance.create_bank_transaction(tenant_id, bank_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->create_bank_transaction: #{e}"
end
```

#### Using the create_bank_transaction_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BankTransactionDtoEnvelope>, Integer, Hash)> create_bank_transaction_with_http_info(tenant_id, bank_id, opts)

```ruby
begin
  # Creates a new bank transaction
  data, status_code, headers = api_instance.create_bank_transaction_with_http_info(tenant_id, bank_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BankTransactionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->create_bank_transaction_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **bank_transaction_create_dto** | [**BankTransactionCreateDto**](BankTransactionCreateDto.md) |  | [optional] |

### Return type

[**BankTransactionDtoEnvelope**](BankTransactionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_bank

> delete_bank(tenant_id, bank_id, opts)

Deletes a bank

Delete a bank.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes a bank
  api_instance.delete_bank(tenant_id, bank_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->delete_bank: #{e}"
end
```

#### Using the delete_bank_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_bank_with_http_info(tenant_id, bank_id, opts)

```ruby
begin
  # Deletes a bank
  data, status_code, headers = api_instance.delete_bank_with_http_info(tenant_id, bank_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->delete_bank_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_bank_account

> delete_bank_account(tenant_id, bank_id, account_id, opts)

Deletes a bank account

Delete a bank account.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes a bank account
  api_instance.delete_bank_account(tenant_id, bank_id, account_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->delete_bank_account: #{e}"
end
```

#### Using the delete_bank_account_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_bank_account_with_http_info(tenant_id, bank_id, account_id, opts)

```ruby
begin
  # Deletes a bank account
  data, status_code, headers = api_instance.delete_bank_account_with_http_info(tenant_id, bank_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->delete_bank_account_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_bank_guarantee

> delete_bank_guarantee(tenant_id, bank_id, guarantee_id, opts)

Deletes a bank guarantee

Delete a bank guarantee.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
guarantee_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes a bank guarantee
  api_instance.delete_bank_guarantee(tenant_id, bank_id, guarantee_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->delete_bank_guarantee: #{e}"
end
```

#### Using the delete_bank_guarantee_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_bank_guarantee_with_http_info(tenant_id, bank_id, guarantee_id, opts)

```ruby
begin
  # Deletes a bank guarantee
  data, status_code, headers = api_instance.delete_bank_guarantee_with_http_info(tenant_id, bank_id, guarantee_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->delete_bank_guarantee_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **guarantee_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_bank_transaction

> delete_bank_transaction(tenant_id, bank_id, transaction_id, opts)

Deletes a bank transaction

Delete a bank transaction.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transaction_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes a bank transaction
  api_instance.delete_bank_transaction(tenant_id, bank_id, transaction_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->delete_bank_transaction: #{e}"
end
```

#### Using the delete_bank_transaction_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_bank_transaction_with_http_info(tenant_id, bank_id, transaction_id, opts)

```ruby
begin
  # Deletes a bank transaction
  data, status_code, headers = api_instance.delete_bank_transaction_with_http_info(tenant_id, bank_id, transaction_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->delete_bank_transaction_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **transaction_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_bank

> <BankDtoEnvelope> get_bank(tenant_id, bank_id, opts)

Gets the current tenant bank

Get the currently acting tenant bank.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant bank
  result = api_instance.get_bank(tenant_id, bank_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank: #{e}"
end
```

#### Using the get_bank_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BankDtoEnvelope>, Integer, Hash)> get_bank_with_http_info(tenant_id, bank_id, opts)

```ruby
begin
  # Gets the current tenant bank
  data, status_code, headers = api_instance.get_bank_with_http_info(tenant_id, bank_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BankDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BankDtoEnvelope**](BankDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_bank_account

> <BankAccountDtoEnvelope> get_bank_account(tenant_id, bank_id, account_id, opts)

Gets the current tenant bank account

Get the currently acting tenant bank account.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant bank account
  result = api_instance.get_bank_account(tenant_id, bank_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank_account: #{e}"
end
```

#### Using the get_bank_account_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BankAccountDtoEnvelope>, Integer, Hash)> get_bank_account_with_http_info(tenant_id, bank_id, account_id, opts)

```ruby
begin
  # Gets the current tenant bank account
  data, status_code, headers = api_instance.get_bank_account_with_http_info(tenant_id, bank_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BankAccountDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank_account_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BankAccountDtoEnvelope**](BankAccountDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_bank_accounts

> <BankAccountDtoListEnvelope> get_bank_accounts(tenant_id, bank_id, opts)

Gets the current tenant bank accounts

Get the currently acting tenant bank accounts.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant bank accounts
  result = api_instance.get_bank_accounts(tenant_id, bank_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank_accounts: #{e}"
end
```

#### Using the get_bank_accounts_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BankAccountDtoListEnvelope>, Integer, Hash)> get_bank_accounts_with_http_info(tenant_id, bank_id, opts)

```ruby
begin
  # Gets the current tenant bank accounts
  data, status_code, headers = api_instance.get_bank_accounts_with_http_info(tenant_id, bank_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BankAccountDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank_accounts_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BankAccountDtoListEnvelope**](BankAccountDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_bank_accounts_count

> <Int32Envelope> get_bank_accounts_count(tenant_id, bank_id, opts)

Gets the current tenant bank accounts count

Get the currently acting tenant bank accounts count.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant bank accounts count
  result = api_instance.get_bank_accounts_count(tenant_id, bank_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank_accounts_count: #{e}"
end
```

#### Using the get_bank_accounts_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_bank_accounts_count_with_http_info(tenant_id, bank_id, opts)

```ruby
begin
  # Gets the current tenant bank accounts count
  data, status_code, headers = api_instance.get_bank_accounts_count_with_http_info(tenant_id, bank_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank_accounts_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_bank_guarantee

> <BankGuaranteeDtoEnvelope> get_bank_guarantee(tenant_id, bank_id, guarantee_id, opts)

Gets the current tenant bank guarantee

Get the currently acting tenant bank guarantee.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
guarantee_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant bank guarantee
  result = api_instance.get_bank_guarantee(tenant_id, bank_id, guarantee_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank_guarantee: #{e}"
end
```

#### Using the get_bank_guarantee_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BankGuaranteeDtoEnvelope>, Integer, Hash)> get_bank_guarantee_with_http_info(tenant_id, bank_id, guarantee_id, opts)

```ruby
begin
  # Gets the current tenant bank guarantee
  data, status_code, headers = api_instance.get_bank_guarantee_with_http_info(tenant_id, bank_id, guarantee_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BankGuaranteeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank_guarantee_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **guarantee_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BankGuaranteeDtoEnvelope**](BankGuaranteeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_bank_guarantees

> <BankGuaranteeDtoListEnvelope> get_bank_guarantees(tenant_id, bank_id, opts)

Gets the current tenant bank guarantees

Get the currently acting tenant bank guarantees.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant bank guarantees
  result = api_instance.get_bank_guarantees(tenant_id, bank_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank_guarantees: #{e}"
end
```

#### Using the get_bank_guarantees_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BankGuaranteeDtoListEnvelope>, Integer, Hash)> get_bank_guarantees_with_http_info(tenant_id, bank_id, opts)

```ruby
begin
  # Gets the current tenant bank guarantees
  data, status_code, headers = api_instance.get_bank_guarantees_with_http_info(tenant_id, bank_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BankGuaranteeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank_guarantees_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BankGuaranteeDtoListEnvelope**](BankGuaranteeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_bank_guarantees_count

> <Int32Envelope> get_bank_guarantees_count(tenant_id, bank_id, opts)

Gets the current tenant bank guarantees count

Get the currently acting tenant bank guarantees count.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant bank guarantees count
  result = api_instance.get_bank_guarantees_count(tenant_id, bank_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank_guarantees_count: #{e}"
end
```

#### Using the get_bank_guarantees_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_bank_guarantees_count_with_http_info(tenant_id, bank_id, opts)

```ruby
begin
  # Gets the current tenant bank guarantees count
  data, status_code, headers = api_instance.get_bank_guarantees_count_with_http_info(tenant_id, bank_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank_guarantees_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_bank_transaction

> <BankTransactionDtoEnvelope> get_bank_transaction(tenant_id, bank_id, transaction_id, opts)

Gets the current tenant bank transaction

Get the currently acting tenant bank transaction.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transaction_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant bank transaction
  result = api_instance.get_bank_transaction(tenant_id, bank_id, transaction_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank_transaction: #{e}"
end
```

#### Using the get_bank_transaction_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BankTransactionDtoEnvelope>, Integer, Hash)> get_bank_transaction_with_http_info(tenant_id, bank_id, transaction_id, opts)

```ruby
begin
  # Gets the current tenant bank transaction
  data, status_code, headers = api_instance.get_bank_transaction_with_http_info(tenant_id, bank_id, transaction_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BankTransactionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank_transaction_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **transaction_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BankTransactionDtoEnvelope**](BankTransactionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_bank_transactions

> <BankTransactionDtoListEnvelope> get_bank_transactions(tenant_id, bank_id, opts)

Gets the current tenant bank transactions

Get the currently acting tenant bank transactions.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant bank transactions
  result = api_instance.get_bank_transactions(tenant_id, bank_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank_transactions: #{e}"
end
```

#### Using the get_bank_transactions_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BankTransactionDtoListEnvelope>, Integer, Hash)> get_bank_transactions_with_http_info(tenant_id, bank_id, opts)

```ruby
begin
  # Gets the current tenant bank transactions
  data, status_code, headers = api_instance.get_bank_transactions_with_http_info(tenant_id, bank_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BankTransactionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank_transactions_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BankTransactionDtoListEnvelope**](BankTransactionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_bank_transactions_count

> <Int32Envelope> get_bank_transactions_count(tenant_id, bank_id, opts)

Gets the current tenant bank transactions count

Get the currently acting tenant bank transactions count.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant bank transactions count
  result = api_instance.get_bank_transactions_count(tenant_id, bank_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank_transactions_count: #{e}"
end
```

#### Using the get_bank_transactions_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_bank_transactions_count_with_http_info(tenant_id, bank_id, opts)

```ruby
begin
  # Gets the current tenant bank transactions count
  data, status_code, headers = api_instance.get_bank_transactions_count_with_http_info(tenant_id, bank_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_bank_transactions_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_banks

> <BankDtoListEnvelope> get_banks(tenant_id, opts)

Gets the current tenant banks

Get the currently acting tenant banks.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant banks
  result = api_instance.get_banks(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_banks: #{e}"
end
```

#### Using the get_banks_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BankDtoListEnvelope>, Integer, Hash)> get_banks_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets the current tenant banks
  data, status_code, headers = api_instance.get_banks_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BankDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_banks_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BankDtoListEnvelope**](BankDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_banks_count

> <Int32Envelope> get_banks_count(tenant_id, opts)

Gets the current tenant banks count

Get the currently acting tenant banks count.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant banks count
  result = api_instance.get_banks_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_banks_count: #{e}"
end
```

#### Using the get_banks_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_banks_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets the current tenant banks count
  data, status_code, headers = api_instance.get_banks_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->get_banks_count_with_http_info: #{e}"
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


## patch_bank

> <EmptyEnvelope> patch_bank(tenant_id, bank_id, opts)

Patches a bank

Partially update a bank using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patches a bank
  result = api_instance.patch_bank(tenant_id, bank_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->patch_bank: #{e}"
end
```

#### Using the patch_bank_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_bank_with_http_info(tenant_id, bank_id, opts)

```ruby
begin
  # Patches a bank
  data, status_code, headers = api_instance.patch_bank_with_http_info(tenant_id, bank_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->patch_bank_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
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


## patch_bank_account

> <EmptyEnvelope> patch_bank_account(tenant_id, bank_id, account_id, opts)

Patches a bank account

Partially update a bank account using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patches a bank account
  result = api_instance.patch_bank_account(tenant_id, bank_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->patch_bank_account: #{e}"
end
```

#### Using the patch_bank_account_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_bank_account_with_http_info(tenant_id, bank_id, account_id, opts)

```ruby
begin
  # Patches a bank account
  data, status_code, headers = api_instance.patch_bank_account_with_http_info(tenant_id, bank_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->patch_bank_account_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **account_id** | **String** |  |  |
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


## patch_bank_guarantee

> <EmptyEnvelope> patch_bank_guarantee(tenant_id, bank_id, guarantee_id, opts)

Patches a bank guarantee

Partially update a bank guarantee using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
guarantee_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patches a bank guarantee
  result = api_instance.patch_bank_guarantee(tenant_id, bank_id, guarantee_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->patch_bank_guarantee: #{e}"
end
```

#### Using the patch_bank_guarantee_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_bank_guarantee_with_http_info(tenant_id, bank_id, guarantee_id, opts)

```ruby
begin
  # Patches a bank guarantee
  data, status_code, headers = api_instance.patch_bank_guarantee_with_http_info(tenant_id, bank_id, guarantee_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->patch_bank_guarantee_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **guarantee_id** | **String** |  |  |
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


## patch_bank_transaction

> <EmptyEnvelope> patch_bank_transaction(tenant_id, bank_id, transaction_id, opts)

Patches a bank transaction

Partially update a bank transaction using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transaction_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patches a bank transaction
  result = api_instance.patch_bank_transaction(tenant_id, bank_id, transaction_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->patch_bank_transaction: #{e}"
end
```

#### Using the patch_bank_transaction_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_bank_transaction_with_http_info(tenant_id, bank_id, transaction_id, opts)

```ruby
begin
  # Patches a bank transaction
  data, status_code, headers = api_instance.patch_bank_transaction_with_http_info(tenant_id, bank_id, transaction_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->patch_bank_transaction_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **transaction_id** | **String** |  |  |
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


## update_bank

> <BankDtoEnvelope> update_bank(tenant_id, bank_id, opts)

Updates a bank

Update a bank.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  bank_update_dto: OpenapiClient::BankUpdateDto.new # BankUpdateDto | 
}

begin
  # Updates a bank
  result = api_instance.update_bank(tenant_id, bank_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->update_bank: #{e}"
end
```

#### Using the update_bank_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BankDtoEnvelope>, Integer, Hash)> update_bank_with_http_info(tenant_id, bank_id, opts)

```ruby
begin
  # Updates a bank
  data, status_code, headers = api_instance.update_bank_with_http_info(tenant_id, bank_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BankDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->update_bank_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **bank_update_dto** | [**BankUpdateDto**](BankUpdateDto.md) |  | [optional] |

### Return type

[**BankDtoEnvelope**](BankDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_bank_account

> <BankAccountDtoEnvelope> update_bank_account(tenant_id, bank_id, account_id, opts)

Updates a bank account

Update a bank account.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  bank_account_update_dto: OpenapiClient::BankAccountUpdateDto.new # BankAccountUpdateDto | 
}

begin
  # Updates a bank account
  result = api_instance.update_bank_account(tenant_id, bank_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->update_bank_account: #{e}"
end
```

#### Using the update_bank_account_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BankAccountDtoEnvelope>, Integer, Hash)> update_bank_account_with_http_info(tenant_id, bank_id, account_id, opts)

```ruby
begin
  # Updates a bank account
  data, status_code, headers = api_instance.update_bank_account_with_http_info(tenant_id, bank_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BankAccountDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->update_bank_account_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **bank_account_update_dto** | [**BankAccountUpdateDto**](BankAccountUpdateDto.md) |  | [optional] |

### Return type

[**BankAccountDtoEnvelope**](BankAccountDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_bank_guarantee

> <BankGuaranteeDtoEnvelope> update_bank_guarantee(tenant_id, bank_id, guarantee_id, opts)

Updates a bank guarantee

Update a bank guarantee.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
guarantee_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  bank_guarantee_update_dto: OpenapiClient::BankGuaranteeUpdateDto.new # BankGuaranteeUpdateDto | 
}

begin
  # Updates a bank guarantee
  result = api_instance.update_bank_guarantee(tenant_id, bank_id, guarantee_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->update_bank_guarantee: #{e}"
end
```

#### Using the update_bank_guarantee_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BankGuaranteeDtoEnvelope>, Integer, Hash)> update_bank_guarantee_with_http_info(tenant_id, bank_id, guarantee_id, opts)

```ruby
begin
  # Updates a bank guarantee
  data, status_code, headers = api_instance.update_bank_guarantee_with_http_info(tenant_id, bank_id, guarantee_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BankGuaranteeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->update_bank_guarantee_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **guarantee_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **bank_guarantee_update_dto** | [**BankGuaranteeUpdateDto**](BankGuaranteeUpdateDto.md) |  | [optional] |

### Return type

[**BankGuaranteeDtoEnvelope**](BankGuaranteeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_bank_transaction

> <BankTransactionDtoEnvelope> update_bank_transaction(tenant_id, bank_id, transaction_id, opts)

Updates a bank transaction

Update a bank transaction.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
bank_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transaction_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  bank_transaction_update_dto: OpenapiClient::BankTransactionUpdateDto.new # BankTransactionUpdateDto | 
}

begin
  # Updates a bank transaction
  result = api_instance.update_bank_transaction(tenant_id, bank_id, transaction_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->update_bank_transaction: #{e}"
end
```

#### Using the update_bank_transaction_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BankTransactionDtoEnvelope>, Integer, Hash)> update_bank_transaction_with_http_info(tenant_id, bank_id, transaction_id, opts)

```ruby
begin
  # Updates a bank transaction
  data, status_code, headers = api_instance.update_bank_transaction_with_http_info(tenant_id, bank_id, transaction_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BankTransactionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankingApi->update_bank_transaction_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **bank_id** | **String** |  |  |
| **transaction_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **bank_transaction_update_dto** | [**BankTransactionUpdateDto**](BankTransactionUpdateDto.md) |  | [optional] |

### Return type

[**BankTransactionDtoEnvelope**](BankTransactionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

