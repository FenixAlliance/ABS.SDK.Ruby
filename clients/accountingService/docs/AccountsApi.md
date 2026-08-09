# OpenapiClient::AccountsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**aggregate_accounts_balance_async**](AccountsApi.md#aggregate_accounts_balance_async) | **GET** /api/v2/AccountingService/Accounts/Aggregate/Balance | Aggregate accounts balance |
| [**balance_account_async**](AccountsApi.md#balance_account_async) | **POST** /api/v2/AccountingService/Accounts/{accountId}/Balance | Balance account |
| [**balance_root_account_async**](AccountsApi.md#balance_root_account_async) | **POST** /api/v2/AccountingService/Accounts/Root/Balance | Balance root account |
| [**create_account_async**](AccountsApi.md#create_account_async) | **POST** /api/v2/AccountingService/Accounts | Get root accounts |
| [**create_account_credit_async**](AccountsApi.md#create_account_credit_async) | **POST** /api/v2/AccountingService/Accounts/{accountId}/Credits | Create account credit |
| [**create_account_debit_async**](AccountsApi.md#create_account_debit_async) | **POST** /api/v2/AccountingService/Accounts/{accountId}/Debits | Create account debit |
| [**create_account_entry_async**](AccountsApi.md#create_account_entry_async) | **POST** /api/v2/AccountingService/Accounts/{accountId}/Entries | Create account entry |
| [**create_account_relation_async**](AccountsApi.md#create_account_relation_async) | **POST** /api/v2/AccountingService/Accounts/Relations | Create account relation |
| [**create_account_type_async**](AccountsApi.md#create_account_type_async) | **POST** /api/v2/AccountingService/Accounts/Types | Create account type |
| [**delete_account_async**](AccountsApi.md#delete_account_async) | **DELETE** /api/v2/AccountingService/Accounts/{accountId} | Delete an account |
| [**delete_account_entry_async**](AccountsApi.md#delete_account_entry_async) | **DELETE** /api/v2/AccountingService/Accounts/{accountId}/Entries/{entryId} | Delete account entry |
| [**delete_account_relation_async**](AccountsApi.md#delete_account_relation_async) | **DELETE** /api/v2/AccountingService/Accounts/Relations/{accountRelationId} | Delete account relation |
| [**delete_account_type_async**](AccountsApi.md#delete_account_type_async) | **DELETE** /api/v2/AccountingService/Accounts/Types/{accountTypeId} | Delete account type |
| [**get_account_aggregate_async**](AccountsApi.md#get_account_aggregate_async) | **POST** /api/v2/AccountingService/Accounts/Aggregate | Get account aggregate |
| [**get_account_credits_async**](AccountsApi.md#get_account_credits_async) | **GET** /api/v2/AccountingService/Accounts/{accountId}/Credits | Get account credits |
| [**get_account_credits_count_async**](AccountsApi.md#get_account_credits_count_async) | **GET** /api/v2/AccountingService/Accounts/{accountId}/Credits/Count | Get account credits count |
| [**get_account_debits_async**](AccountsApi.md#get_account_debits_async) | **GET** /api/v2/AccountingService/Accounts/{accountId}/Debits | Get account debits |
| [**get_account_debits_count_async**](AccountsApi.md#get_account_debits_count_async) | **GET** /api/v2/AccountingService/Accounts/{accountId}/Debits/Count | Get account debits count |
| [**get_account_details_async**](AccountsApi.md#get_account_details_async) | **GET** /api/v2/AccountingService/Accounts/{accountId} | Get account details |
| [**get_account_entries_async**](AccountsApi.md#get_account_entries_async) | **GET** /api/v2/AccountingService/Accounts/{accountId}/Entries | Get account entries |
| [**get_account_entry_async**](AccountsApi.md#get_account_entry_async) | **GET** /api/v2/AccountingService/Accounts/{accountId}/Entries/{entryId} | Get account entry |
| [**get_account_relations_async**](AccountsApi.md#get_account_relations_async) | **GET** /api/v2/AccountingService/Accounts/Relations | Get account relations |
| [**get_account_relations_count_async**](AccountsApi.md#get_account_relations_count_async) | **GET** /api/v2/AccountingService/Accounts/Relations/Count | Get account relations count |
| [**get_account_type_by_id_async**](AccountsApi.md#get_account_type_by_id_async) | **GET** /api/v2/AccountingService/Accounts/Types/{accountTypeId} | Get account type by ID |
| [**get_account_types_async**](AccountsApi.md#get_account_types_async) | **GET** /api/v2/AccountingService/Accounts/Types | Get account types |
| [**get_account_types_count_async**](AccountsApi.md#get_account_types_count_async) | **GET** /api/v2/AccountingService/Accounts/Types/Count | Get account types count |
| [**get_accounts_async**](AccountsApi.md#get_accounts_async) | **GET** /api/v2/AccountingService/Accounts | Creates a new account |
| [**get_accounts_count_async**](AccountsApi.md#get_accounts_count_async) | **GET** /api/v2/AccountingService/Accounts/Count | Get the number of accounts |
| [**get_charts_of_accounts_async**](AccountsApi.md#get_charts_of_accounts_async) | **GET** /api/v2/AccountingService/Accounts/ChartsOfAccounts | Get charts of accounts |
| [**get_child_accounts_async**](AccountsApi.md#get_child_accounts_async) | **GET** /api/v2/AccountingService/Accounts/{accountId}/Children | Get child accounts |
| [**get_credit_account_entries_async**](AccountsApi.md#get_credit_account_entries_async) | **GET** /api/v2/AccountingService/Accounts/{accountId}/Entries/Credit | Get credit account entries |
| [**get_debit_account_entries_async**](AccountsApi.md#get_debit_account_entries_async) | **GET** /api/v2/AccountingService/Accounts/{accountId}/Entries/Debit | Get debit account entries |
| [**get_root_accounts_async**](AccountsApi.md#get_root_accounts_async) | **GET** /api/v2/AccountingService/Accounts/Root | Get root accounts |
| [**patch_account_async**](AccountsApi.md#patch_account_async) | **PATCH** /api/v2/AccountingService/Accounts/{accountId} | Patch an account |
| [**patch_account_entry_async**](AccountsApi.md#patch_account_entry_async) | **PATCH** /api/v2/AccountingService/Accounts/{accountId}/Entries/{entryId} | Patch account entry |
| [**patch_account_relation_async**](AccountsApi.md#patch_account_relation_async) | **PATCH** /api/v2/AccountingService/Accounts/Relations/{accountRelationId} | Patch account relation |
| [**patch_account_type_async**](AccountsApi.md#patch_account_type_async) | **PATCH** /api/v2/AccountingService/Accounts/Types/{accountTypeId} | Patch account type |
| [**seed_chart_of_accounts_async**](AccountsApi.md#seed_chart_of_accounts_async) | **POST** /api/v2/AccountingService/Accounts/ChartsOfAccounts/Seed | Seed chart of accounts |
| [**update_account_async**](AccountsApi.md#update_account_async) | **PUT** /api/v2/AccountingService/Accounts/{accountId} | Update an account |
| [**update_account_entry_async**](AccountsApi.md#update_account_entry_async) | **PUT** /api/v2/AccountingService/Accounts/{accountId}/Entries/{entryId} | Update account entry |
| [**update_account_relation_async**](AccountsApi.md#update_account_relation_async) | **PUT** /api/v2/AccountingService/Accounts/Relations/{accountRelationId} | Update account relation |
| [**update_account_type_async**](AccountsApi.md#update_account_type_async) | **PUT** /api/v2/AccountingService/Accounts/Types/{accountTypeId} | Update account type |


## aggregate_accounts_balance_async

> <MoneyEnvelope> aggregate_accounts_balance_async(tenant_id, opts)

Aggregate accounts balance

Returns the sum of all account balances matching OData filters, normalized to the target currency using stored USD values.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  currency_id: 'currency_id_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  account_dto_collection_query_parameters: OpenapiClient::AccountDtoCollectionQueryParameters.new # AccountDtoCollectionQueryParameters | 
}

begin
  # Aggregate accounts balance
  result = api_instance.aggregate_accounts_balance_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->aggregate_accounts_balance_async: #{e}"
end
```

#### Using the aggregate_accounts_balance_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MoneyEnvelope>, Integer, Hash)> aggregate_accounts_balance_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Aggregate accounts balance
  data, status_code, headers = api_instance.aggregate_accounts_balance_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MoneyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->aggregate_accounts_balance_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **currency_id** | **String** |  | [optional][default to &#39;USD.USA&#39;] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **account_dto_collection_query_parameters** | [**AccountDtoCollectionQueryParameters**](AccountDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## balance_account_async

> <AccountDtoEnvelope> balance_account_async(tenant_id, account_id, opts)

Balance account

Balance account.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Balance account
  result = api_instance.balance_account_async(tenant_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->balance_account_async: #{e}"
end
```

#### Using the balance_account_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountDtoEnvelope>, Integer, Hash)> balance_account_async_with_http_info(tenant_id, account_id, opts)

```ruby
begin
  # Balance account
  data, status_code, headers = api_instance.balance_account_async_with_http_info(tenant_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->balance_account_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**AccountDtoEnvelope**](AccountDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## balance_root_account_async

> <AccountDtoListEnvelope> balance_root_account_async(tenant_id, opts)

Balance root account

Balance root account.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Balance root account
  result = api_instance.balance_root_account_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->balance_root_account_async: #{e}"
end
```

#### Using the balance_root_account_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountDtoListEnvelope>, Integer, Hash)> balance_root_account_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Balance root account
  data, status_code, headers = api_instance.balance_root_account_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->balance_root_account_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**AccountDtoListEnvelope**](AccountDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_account_async

> <AccountDtoListEnvelope> create_account_async(tenant_id, opts)

Get root accounts

Get root accounts.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  account_create_dto: OpenapiClient::AccountCreateDto.new({name: 'name_example', currency_id: 'currency_id_example', account_category: 'Assets'}) # AccountCreateDto | 
}

begin
  # Get root accounts
  result = api_instance.create_account_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->create_account_async: #{e}"
end
```

#### Using the create_account_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountDtoListEnvelope>, Integer, Hash)> create_account_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get root accounts
  data, status_code, headers = api_instance.create_account_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->create_account_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **account_create_dto** | [**AccountCreateDto**](AccountCreateDto.md) |  | [optional] |

### Return type

[**AccountDtoListEnvelope**](AccountDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_account_credit_async

> <AccountingEntryDtoListEnvelope> create_account_credit_async(tenant_id, account_id, opts)

Create account credit

Create account credit.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  accounting_entry_create_dto: OpenapiClient::AccountingEntryCreateDto.new({journal_entry_id: 'journal_entry_id_example', account_id: 'account_id_example', direction: 'Debit', transaction_currency_id: 'transaction_currency_id_example', description: 'description_example'}) # AccountingEntryCreateDto | 
}

begin
  # Create account credit
  result = api_instance.create_account_credit_async(tenant_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->create_account_credit_async: #{e}"
end
```

#### Using the create_account_credit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountingEntryDtoListEnvelope>, Integer, Hash)> create_account_credit_async_with_http_info(tenant_id, account_id, opts)

```ruby
begin
  # Create account credit
  data, status_code, headers = api_instance.create_account_credit_async_with_http_info(tenant_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountingEntryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->create_account_credit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **accounting_entry_create_dto** | [**AccountingEntryCreateDto**](AccountingEntryCreateDto.md) |  | [optional] |

### Return type

[**AccountingEntryDtoListEnvelope**](AccountingEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_account_debit_async

> <AccountingEntryDtoListEnvelope> create_account_debit_async(tenant_id, account_id, opts)

Create account debit

Create account debit.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  accounting_entry_create_dto: OpenapiClient::AccountingEntryCreateDto.new({journal_entry_id: 'journal_entry_id_example', account_id: 'account_id_example', direction: 'Debit', transaction_currency_id: 'transaction_currency_id_example', description: 'description_example'}) # AccountingEntryCreateDto | 
}

begin
  # Create account debit
  result = api_instance.create_account_debit_async(tenant_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->create_account_debit_async: #{e}"
end
```

#### Using the create_account_debit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountingEntryDtoListEnvelope>, Integer, Hash)> create_account_debit_async_with_http_info(tenant_id, account_id, opts)

```ruby
begin
  # Create account debit
  data, status_code, headers = api_instance.create_account_debit_async_with_http_info(tenant_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountingEntryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->create_account_debit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **accounting_entry_create_dto** | [**AccountingEntryCreateDto**](AccountingEntryCreateDto.md) |  | [optional] |

### Return type

[**AccountingEntryDtoListEnvelope**](AccountingEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_account_entry_async

> <AccountingEntryDtoEnvelope> create_account_entry_async(tenant_id, account_id, opts)

Create account entry

Create account entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  accounting_entry_create_dto: OpenapiClient::AccountingEntryCreateDto.new({journal_entry_id: 'journal_entry_id_example', account_id: 'account_id_example', direction: 'Debit', transaction_currency_id: 'transaction_currency_id_example', description: 'description_example'}) # AccountingEntryCreateDto | 
}

begin
  # Create account entry
  result = api_instance.create_account_entry_async(tenant_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->create_account_entry_async: #{e}"
end
```

#### Using the create_account_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountingEntryDtoEnvelope>, Integer, Hash)> create_account_entry_async_with_http_info(tenant_id, account_id, opts)

```ruby
begin
  # Create account entry
  data, status_code, headers = api_instance.create_account_entry_async_with_http_info(tenant_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountingEntryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->create_account_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **accounting_entry_create_dto** | [**AccountingEntryCreateDto**](AccountingEntryCreateDto.md) |  | [optional] |

### Return type

[**AccountingEntryDtoEnvelope**](AccountingEntryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_account_relation_async

> <EmptyEnvelope> create_account_relation_async(tenant_id, account_id, opts)

Create account relation

Create account relation.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  account_relation_create_dto: OpenapiClient::AccountRelationCreateDto.new # AccountRelationCreateDto | 
}

begin
  # Create account relation
  result = api_instance.create_account_relation_async(tenant_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->create_account_relation_async: #{e}"
end
```

#### Using the create_account_relation_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_account_relation_async_with_http_info(tenant_id, account_id, opts)

```ruby
begin
  # Create account relation
  data, status_code, headers = api_instance.create_account_relation_async_with_http_info(tenant_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->create_account_relation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **account_relation_create_dto** | [**AccountRelationCreateDto**](AccountRelationCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_account_type_async

> <EmptyEnvelope> create_account_type_async(tenant_id, opts)

Create account type

Create account type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  account_type_create_dto: OpenapiClient::AccountTypeCreateDto.new # AccountTypeCreateDto | 
}

begin
  # Create account type
  result = api_instance.create_account_type_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->create_account_type_async: #{e}"
end
```

#### Using the create_account_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_account_type_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create account type
  data, status_code, headers = api_instance.create_account_type_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->create_account_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **account_type_create_dto** | [**AccountTypeCreateDto**](AccountTypeCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_account_async

> <EmptyEnvelope> delete_account_async(tenant_id, account_id, opts)

Delete an account

Delete an account.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an account
  result = api_instance.delete_account_async(tenant_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->delete_account_async: #{e}"
end
```

#### Using the delete_account_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_account_async_with_http_info(tenant_id, account_id, opts)

```ruby
begin
  # Delete an account
  data, status_code, headers = api_instance.delete_account_async_with_http_info(tenant_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->delete_account_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_account_entry_async

> <EmptyEnvelope> delete_account_entry_async(tenant_id, account_id, entry_id, opts)

Delete account entry

Delete account entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete account entry
  result = api_instance.delete_account_entry_async(tenant_id, account_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->delete_account_entry_async: #{e}"
end
```

#### Using the delete_account_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_account_entry_async_with_http_info(tenant_id, account_id, entry_id, opts)

```ruby
begin
  # Delete account entry
  data, status_code, headers = api_instance.delete_account_entry_async_with_http_info(tenant_id, account_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->delete_account_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **entry_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_account_relation_async

> <EmptyEnvelope> delete_account_relation_async(tenant_id, account_relation_id, account_id, opts)

Delete account relation

Delete account relation.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_relation_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete account relation
  result = api_instance.delete_account_relation_async(tenant_id, account_relation_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->delete_account_relation_async: #{e}"
end
```

#### Using the delete_account_relation_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_account_relation_async_with_http_info(tenant_id, account_relation_id, account_id, opts)

```ruby
begin
  # Delete account relation
  data, status_code, headers = api_instance.delete_account_relation_async_with_http_info(tenant_id, account_relation_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->delete_account_relation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_relation_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_account_type_async

> <EmptyEnvelope> delete_account_type_async(tenant_id, account_type_id, opts)

Delete account type

Delete account type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete account type
  result = api_instance.delete_account_type_async(tenant_id, account_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->delete_account_type_async: #{e}"
end
```

#### Using the delete_account_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_account_type_async_with_http_info(tenant_id, account_type_id, opts)

```ruby
begin
  # Delete account type
  data, status_code, headers = api_instance.delete_account_type_async_with_http_info(tenant_id, account_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->delete_account_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_account_aggregate_async

> <AccountingEntryDtoListEnvelope> get_account_aggregate_async(tenant_id, opts)

Get account aggregate

Get account aggregate.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  currency_id: 'currency_id_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  account_dto: [OpenapiClient::AccountDto.new] # Array<AccountDto> | 
}

begin
  # Get account aggregate
  result = api_instance.get_account_aggregate_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_aggregate_async: #{e}"
end
```

#### Using the get_account_aggregate_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountingEntryDtoListEnvelope>, Integer, Hash)> get_account_aggregate_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get account aggregate
  data, status_code, headers = api_instance.get_account_aggregate_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountingEntryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_aggregate_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **currency_id** | **String** |  | [optional][default to &#39;USD.USA&#39;] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **account_dto** | [**Array&lt;AccountDto&gt;**](AccountDto.md) |  | [optional] |

### Return type

[**AccountingEntryDtoListEnvelope**](AccountingEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_account_credits_async

> <AccountingEntryDtoListEnvelope> get_account_credits_async(tenant_id, account_id, opts)

Get account credits

Get account credits.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  accounting_entry_dto_collection_query_parameters: OpenapiClient::AccountingEntryDtoCollectionQueryParameters.new # AccountingEntryDtoCollectionQueryParameters | 
}

begin
  # Get account credits
  result = api_instance.get_account_credits_async(tenant_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_credits_async: #{e}"
end
```

#### Using the get_account_credits_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountingEntryDtoListEnvelope>, Integer, Hash)> get_account_credits_async_with_http_info(tenant_id, account_id, opts)

```ruby
begin
  # Get account credits
  data, status_code, headers = api_instance.get_account_credits_async_with_http_info(tenant_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountingEntryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_credits_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **accounting_entry_dto_collection_query_parameters** | [**AccountingEntryDtoCollectionQueryParameters**](AccountingEntryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AccountingEntryDtoListEnvelope**](AccountingEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_account_credits_count_async

> <Int32Envelope> get_account_credits_count_async(tenant_id, account_id, opts)

Get account credits count

Get account credits count.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  accounting_entry_dto_collection_query_parameters: OpenapiClient::AccountingEntryDtoCollectionQueryParameters.new # AccountingEntryDtoCollectionQueryParameters | 
}

begin
  # Get account credits count
  result = api_instance.get_account_credits_count_async(tenant_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_credits_count_async: #{e}"
end
```

#### Using the get_account_credits_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_account_credits_count_async_with_http_info(tenant_id, account_id, opts)

```ruby
begin
  # Get account credits count
  data, status_code, headers = api_instance.get_account_credits_count_async_with_http_info(tenant_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_credits_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **accounting_entry_dto_collection_query_parameters** | [**AccountingEntryDtoCollectionQueryParameters**](AccountingEntryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_account_debits_async

> <AccountingEntryDtoListEnvelope> get_account_debits_async(tenant_id, account_id, opts)

Get account debits

Get account debits.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  accounting_entry_dto_collection_query_parameters: OpenapiClient::AccountingEntryDtoCollectionQueryParameters.new # AccountingEntryDtoCollectionQueryParameters | 
}

begin
  # Get account debits
  result = api_instance.get_account_debits_async(tenant_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_debits_async: #{e}"
end
```

#### Using the get_account_debits_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountingEntryDtoListEnvelope>, Integer, Hash)> get_account_debits_async_with_http_info(tenant_id, account_id, opts)

```ruby
begin
  # Get account debits
  data, status_code, headers = api_instance.get_account_debits_async_with_http_info(tenant_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountingEntryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_debits_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **accounting_entry_dto_collection_query_parameters** | [**AccountingEntryDtoCollectionQueryParameters**](AccountingEntryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AccountingEntryDtoListEnvelope**](AccountingEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_account_debits_count_async

> <Int32Envelope> get_account_debits_count_async(tenant_id, account_id, opts)

Get account debits count

Get account debits count.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  accounting_entry_dto_collection_query_parameters: OpenapiClient::AccountingEntryDtoCollectionQueryParameters.new # AccountingEntryDtoCollectionQueryParameters | 
}

begin
  # Get account debits count
  result = api_instance.get_account_debits_count_async(tenant_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_debits_count_async: #{e}"
end
```

#### Using the get_account_debits_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_account_debits_count_async_with_http_info(tenant_id, account_id, opts)

```ruby
begin
  # Get account debits count
  data, status_code, headers = api_instance.get_account_debits_count_async_with_http_info(tenant_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_debits_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **accounting_entry_dto_collection_query_parameters** | [**AccountingEntryDtoCollectionQueryParameters**](AccountingEntryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_account_details_async

> <AccountDtoEnvelope> get_account_details_async(tenant_id, account_id, opts)

Get account details

Get account details.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get account details
  result = api_instance.get_account_details_async(tenant_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_details_async: #{e}"
end
```

#### Using the get_account_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountDtoEnvelope>, Integer, Hash)> get_account_details_async_with_http_info(tenant_id, account_id, opts)

```ruby
begin
  # Get account details
  data, status_code, headers = api_instance.get_account_details_async_with_http_info(tenant_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**AccountDtoEnvelope**](AccountDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_account_entries_async

> <AccountingEntryDtoListEnvelope> get_account_entries_async(tenant_id, account_id, opts)

Get account entries

Get account entries.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  accounting_entry_dto_collection_query_parameters: OpenapiClient::AccountingEntryDtoCollectionQueryParameters.new # AccountingEntryDtoCollectionQueryParameters | 
}

begin
  # Get account entries
  result = api_instance.get_account_entries_async(tenant_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_entries_async: #{e}"
end
```

#### Using the get_account_entries_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountingEntryDtoListEnvelope>, Integer, Hash)> get_account_entries_async_with_http_info(tenant_id, account_id, opts)

```ruby
begin
  # Get account entries
  data, status_code, headers = api_instance.get_account_entries_async_with_http_info(tenant_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountingEntryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_entries_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **accounting_entry_dto_collection_query_parameters** | [**AccountingEntryDtoCollectionQueryParameters**](AccountingEntryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AccountingEntryDtoListEnvelope**](AccountingEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_account_entry_async

> <AccountingEntryDtoEnvelope> get_account_entry_async(tenant_id, account_id, entry_id, opts)

Get account entry

Get account entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get account entry
  result = api_instance.get_account_entry_async(tenant_id, account_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_entry_async: #{e}"
end
```

#### Using the get_account_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountingEntryDtoEnvelope>, Integer, Hash)> get_account_entry_async_with_http_info(tenant_id, account_id, entry_id, opts)

```ruby
begin
  # Get account entry
  data, status_code, headers = api_instance.get_account_entry_async_with_http_info(tenant_id, account_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountingEntryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **entry_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**AccountingEntryDtoEnvelope**](AccountingEntryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_account_relations_async

> <AccountRelationDtoListEnvelope> get_account_relations_async(tenant_id, account_id, opts)

Get account relations

Get account relations.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  account_relation_dto_collection_query_parameters: OpenapiClient::AccountRelationDtoCollectionQueryParameters.new # AccountRelationDtoCollectionQueryParameters | 
}

begin
  # Get account relations
  result = api_instance.get_account_relations_async(tenant_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_relations_async: #{e}"
end
```

#### Using the get_account_relations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountRelationDtoListEnvelope>, Integer, Hash)> get_account_relations_async_with_http_info(tenant_id, account_id, opts)

```ruby
begin
  # Get account relations
  data, status_code, headers = api_instance.get_account_relations_async_with_http_info(tenant_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountRelationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_relations_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **account_relation_dto_collection_query_parameters** | [**AccountRelationDtoCollectionQueryParameters**](AccountRelationDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AccountRelationDtoListEnvelope**](AccountRelationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_account_relations_count_async

> <Int32Envelope> get_account_relations_count_async(tenant_id, account_id, opts)

Get account relations count

Get account relations count.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  account_relation_dto_collection_query_parameters: OpenapiClient::AccountRelationDtoCollectionQueryParameters.new # AccountRelationDtoCollectionQueryParameters | 
}

begin
  # Get account relations count
  result = api_instance.get_account_relations_count_async(tenant_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_relations_count_async: #{e}"
end
```

#### Using the get_account_relations_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_account_relations_count_async_with_http_info(tenant_id, account_id, opts)

```ruby
begin
  # Get account relations count
  data, status_code, headers = api_instance.get_account_relations_count_async_with_http_info(tenant_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_relations_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **account_relation_dto_collection_query_parameters** | [**AccountRelationDtoCollectionQueryParameters**](AccountRelationDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_account_type_by_id_async

> <AccountTypeDtoEnvelope> get_account_type_by_id_async(tenant_id, account_type_id, opts)

Get account type by ID

Get account type by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get account type by ID
  result = api_instance.get_account_type_by_id_async(tenant_id, account_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_type_by_id_async: #{e}"
end
```

#### Using the get_account_type_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountTypeDtoEnvelope>, Integer, Hash)> get_account_type_by_id_async_with_http_info(tenant_id, account_type_id, opts)

```ruby
begin
  # Get account type by ID
  data, status_code, headers = api_instance.get_account_type_by_id_async_with_http_info(tenant_id, account_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountTypeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_type_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**AccountTypeDtoEnvelope**](AccountTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_account_types_async

> <AccountTypeDtoListEnvelope> get_account_types_async(tenant_id, opts)

Get account types

Get account types.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  account_type_dto_collection_query_parameters: OpenapiClient::AccountTypeDtoCollectionQueryParameters.new # AccountTypeDtoCollectionQueryParameters | 
}

begin
  # Get account types
  result = api_instance.get_account_types_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_types_async: #{e}"
end
```

#### Using the get_account_types_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountTypeDtoListEnvelope>, Integer, Hash)> get_account_types_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get account types
  data, status_code, headers = api_instance.get_account_types_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountTypeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_types_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **account_type_dto_collection_query_parameters** | [**AccountTypeDtoCollectionQueryParameters**](AccountTypeDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AccountTypeDtoListEnvelope**](AccountTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_account_types_count_async

> <Int32Envelope> get_account_types_count_async(tenant_id, opts)

Get account types count

Get account types count.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  account_type_dto_collection_query_parameters: OpenapiClient::AccountTypeDtoCollectionQueryParameters.new # AccountTypeDtoCollectionQueryParameters | 
}

begin
  # Get account types count
  result = api_instance.get_account_types_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_types_count_async: #{e}"
end
```

#### Using the get_account_types_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_account_types_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get account types count
  data, status_code, headers = api_instance.get_account_types_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_account_types_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **account_type_dto_collection_query_parameters** | [**AccountTypeDtoCollectionQueryParameters**](AccountTypeDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_accounts_async

> <AccountDtoListEnvelope> get_accounts_async(tenant_id, opts)

Creates a new account

Creates a new account.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  account_dto_collection_query_parameters: OpenapiClient::AccountDtoCollectionQueryParameters.new # AccountDtoCollectionQueryParameters | 
}

begin
  # Creates a new account
  result = api_instance.get_accounts_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_accounts_async: #{e}"
end
```

#### Using the get_accounts_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountDtoListEnvelope>, Integer, Hash)> get_accounts_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new account
  data, status_code, headers = api_instance.get_accounts_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_accounts_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **account_dto_collection_query_parameters** | [**AccountDtoCollectionQueryParameters**](AccountDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AccountDtoListEnvelope**](AccountDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_accounts_count_async

> <Int32Envelope> get_accounts_count_async(tenant_id, opts)

Get the number of accounts

Get the number of accounts.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  account_dto_collection_query_parameters: OpenapiClient::AccountDtoCollectionQueryParameters.new # AccountDtoCollectionQueryParameters | 
}

begin
  # Get the number of accounts
  result = api_instance.get_accounts_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_accounts_count_async: #{e}"
end
```

#### Using the get_accounts_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_accounts_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the number of accounts
  data, status_code, headers = api_instance.get_accounts_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_accounts_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **account_dto_collection_query_parameters** | [**AccountDtoCollectionQueryParameters**](AccountDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_charts_of_accounts_async

> <ChartOfAccountsListEnvelope> get_charts_of_accounts_async(opts)

Get charts of accounts

Get available charts of accounts.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get charts of accounts
  result = api_instance.get_charts_of_accounts_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_charts_of_accounts_async: #{e}"
end
```

#### Using the get_charts_of_accounts_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ChartOfAccountsListEnvelope>, Integer, Hash)> get_charts_of_accounts_async_with_http_info(opts)

```ruby
begin
  # Get charts of accounts
  data, status_code, headers = api_instance.get_charts_of_accounts_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ChartOfAccountsListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_charts_of_accounts_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ChartOfAccountsListEnvelope**](ChartOfAccountsListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_child_accounts_async

> <AccountDtoListEnvelope> get_child_accounts_async(tenant_id, account_id, opts)

Get child accounts

Get child accounts.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get child accounts
  result = api_instance.get_child_accounts_async(tenant_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_child_accounts_async: #{e}"
end
```

#### Using the get_child_accounts_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountDtoListEnvelope>, Integer, Hash)> get_child_accounts_async_with_http_info(tenant_id, account_id, opts)

```ruby
begin
  # Get child accounts
  data, status_code, headers = api_instance.get_child_accounts_async_with_http_info(tenant_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_child_accounts_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**AccountDtoListEnvelope**](AccountDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_credit_account_entries_async

> <AccountingEntryDtoListEnvelope> get_credit_account_entries_async(tenant_id, account_id, opts)

Get credit account entries

Get credit account entries.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  accounting_entry_dto_collection_query_parameters: OpenapiClient::AccountingEntryDtoCollectionQueryParameters.new # AccountingEntryDtoCollectionQueryParameters | 
}

begin
  # Get credit account entries
  result = api_instance.get_credit_account_entries_async(tenant_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_credit_account_entries_async: #{e}"
end
```

#### Using the get_credit_account_entries_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountingEntryDtoListEnvelope>, Integer, Hash)> get_credit_account_entries_async_with_http_info(tenant_id, account_id, opts)

```ruby
begin
  # Get credit account entries
  data, status_code, headers = api_instance.get_credit_account_entries_async_with_http_info(tenant_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountingEntryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_credit_account_entries_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **accounting_entry_dto_collection_query_parameters** | [**AccountingEntryDtoCollectionQueryParameters**](AccountingEntryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AccountingEntryDtoListEnvelope**](AccountingEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_debit_account_entries_async

> <AccountingEntryDtoListEnvelope> get_debit_account_entries_async(tenant_id, account_id, opts)

Get debit account entries

Get debit account entries.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  accounting_entry_dto_collection_query_parameters: OpenapiClient::AccountingEntryDtoCollectionQueryParameters.new # AccountingEntryDtoCollectionQueryParameters | 
}

begin
  # Get debit account entries
  result = api_instance.get_debit_account_entries_async(tenant_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_debit_account_entries_async: #{e}"
end
```

#### Using the get_debit_account_entries_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountingEntryDtoListEnvelope>, Integer, Hash)> get_debit_account_entries_async_with_http_info(tenant_id, account_id, opts)

```ruby
begin
  # Get debit account entries
  data, status_code, headers = api_instance.get_debit_account_entries_async_with_http_info(tenant_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountingEntryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_debit_account_entries_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **accounting_entry_dto_collection_query_parameters** | [**AccountingEntryDtoCollectionQueryParameters**](AccountingEntryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AccountingEntryDtoListEnvelope**](AccountingEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_root_accounts_async

> <AccountDtoListEnvelope> get_root_accounts_async(tenant_id, opts)

Get root accounts

Get root accounts.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  account_dto_collection_query_parameters: OpenapiClient::AccountDtoCollectionQueryParameters.new # AccountDtoCollectionQueryParameters | 
}

begin
  # Get root accounts
  result = api_instance.get_root_accounts_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_root_accounts_async: #{e}"
end
```

#### Using the get_root_accounts_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountDtoListEnvelope>, Integer, Hash)> get_root_accounts_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get root accounts
  data, status_code, headers = api_instance.get_root_accounts_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->get_root_accounts_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **account_dto_collection_query_parameters** | [**AccountDtoCollectionQueryParameters**](AccountDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AccountDtoListEnvelope**](AccountDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_account_async

> <EmptyEnvelope> patch_account_async(tenant_id, account_id, opts)

Patch an account

Patch an account.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch an account
  result = api_instance.patch_account_async(tenant_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->patch_account_async: #{e}"
end
```

#### Using the patch_account_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_account_async_with_http_info(tenant_id, account_id, opts)

```ruby
begin
  # Patch an account
  data, status_code, headers = api_instance.patch_account_async_with_http_info(tenant_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->patch_account_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
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


## patch_account_entry_async

> <EmptyEnvelope> patch_account_entry_async(tenant_id, account_id, entry_id, opts)

Patch account entry

Patch account entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch account entry
  result = api_instance.patch_account_entry_async(tenant_id, account_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->patch_account_entry_async: #{e}"
end
```

#### Using the patch_account_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_account_entry_async_with_http_info(tenant_id, account_id, entry_id, opts)

```ruby
begin
  # Patch account entry
  data, status_code, headers = api_instance.patch_account_entry_async_with_http_info(tenant_id, account_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->patch_account_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **entry_id** | **String** |  |  |
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


## patch_account_relation_async

> <EmptyEnvelope> patch_account_relation_async(tenant_id, account_relation_id, account_id, opts)

Patch account relation

Patch account relation.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_relation_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch account relation
  result = api_instance.patch_account_relation_async(tenant_id, account_relation_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->patch_account_relation_async: #{e}"
end
```

#### Using the patch_account_relation_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_account_relation_async_with_http_info(tenant_id, account_relation_id, account_id, opts)

```ruby
begin
  # Patch account relation
  data, status_code, headers = api_instance.patch_account_relation_async_with_http_info(tenant_id, account_relation_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->patch_account_relation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_relation_id** | **String** |  |  |
| **account_id** | **String** |  |  |
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


## patch_account_type_async

> <EmptyEnvelope> patch_account_type_async(tenant_id, account_type_id, opts)

Patch account type

Patch account type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch account type
  result = api_instance.patch_account_type_async(tenant_id, account_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->patch_account_type_async: #{e}"
end
```

#### Using the patch_account_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_account_type_async_with_http_info(tenant_id, account_type_id, opts)

```ruby
begin
  # Patch account type
  data, status_code, headers = api_instance.patch_account_type_async_with_http_info(tenant_id, account_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->patch_account_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_type_id** | **String** |  |  |
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


## seed_chart_of_accounts_async

> <EmptyEnvelope> seed_chart_of_accounts_async(tenant_id, opts)

Seed chart of accounts

Seed a chart of accounts from a file URL.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  seed_chart_of_accounts_request: OpenapiClient::SeedChartOfAccountsRequest.new # SeedChartOfAccountsRequest | 
}

begin
  # Seed chart of accounts
  result = api_instance.seed_chart_of_accounts_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->seed_chart_of_accounts_async: #{e}"
end
```

#### Using the seed_chart_of_accounts_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> seed_chart_of_accounts_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Seed chart of accounts
  data, status_code, headers = api_instance.seed_chart_of_accounts_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->seed_chart_of_accounts_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **seed_chart_of_accounts_request** | [**SeedChartOfAccountsRequest**](SeedChartOfAccountsRequest.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_account_async

> <AccountDtoEnvelope> update_account_async(tenant_id, account_id, opts)

Update an account

Update an account.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  account_update_dto: OpenapiClient::AccountUpdateDto.new({name: 'name_example', currency_id: 'currency_id_example'}) # AccountUpdateDto | 
}

begin
  # Update an account
  result = api_instance.update_account_async(tenant_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->update_account_async: #{e}"
end
```

#### Using the update_account_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccountDtoEnvelope>, Integer, Hash)> update_account_async_with_http_info(tenant_id, account_id, opts)

```ruby
begin
  # Update an account
  data, status_code, headers = api_instance.update_account_async_with_http_info(tenant_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccountDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->update_account_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **account_update_dto** | [**AccountUpdateDto**](AccountUpdateDto.md) |  | [optional] |

### Return type

[**AccountDtoEnvelope**](AccountDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_account_entry_async

> <EmptyEnvelope> update_account_entry_async(tenant_id, account_id, entry_id, opts)

Update account entry

Update account entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  accounting_entry_update_dto: OpenapiClient::AccountingEntryUpdateDto.new # AccountingEntryUpdateDto | 
}

begin
  # Update account entry
  result = api_instance.update_account_entry_async(tenant_id, account_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->update_account_entry_async: #{e}"
end
```

#### Using the update_account_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_account_entry_async_with_http_info(tenant_id, account_id, entry_id, opts)

```ruby
begin
  # Update account entry
  data, status_code, headers = api_instance.update_account_entry_async_with_http_info(tenant_id, account_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->update_account_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **entry_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **accounting_entry_update_dto** | [**AccountingEntryUpdateDto**](AccountingEntryUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_account_relation_async

> <EmptyEnvelope> update_account_relation_async(tenant_id, account_relation_id, account_id, opts)

Update account relation

Update account relation.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_relation_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  account_relation_update_dto: OpenapiClient::AccountRelationUpdateDto.new # AccountRelationUpdateDto | 
}

begin
  # Update account relation
  result = api_instance.update_account_relation_async(tenant_id, account_relation_id, account_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->update_account_relation_async: #{e}"
end
```

#### Using the update_account_relation_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_account_relation_async_with_http_info(tenant_id, account_relation_id, account_id, opts)

```ruby
begin
  # Update account relation
  data, status_code, headers = api_instance.update_account_relation_async_with_http_info(tenant_id, account_relation_id, account_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->update_account_relation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_relation_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **account_relation_update_dto** | [**AccountRelationUpdateDto**](AccountRelationUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_account_type_async

> <EmptyEnvelope> update_account_type_async(tenant_id, account_type_id, opts)

Update account type

Update account type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AccountsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
account_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  account_type_update_dto: OpenapiClient::AccountTypeUpdateDto.new # AccountTypeUpdateDto | 
}

begin
  # Update account type
  result = api_instance.update_account_type_async(tenant_id, account_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->update_account_type_async: #{e}"
end
```

#### Using the update_account_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_account_type_async_with_http_info(tenant_id, account_type_id, opts)

```ruby
begin
  # Update account type
  data, status_code, headers = api_instance.update_account_type_async_with_http_info(tenant_id, account_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AccountsApi->update_account_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **account_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **account_type_update_dto** | [**AccountTypeUpdateDto**](AccountTypeUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

