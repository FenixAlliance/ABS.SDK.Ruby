# OpenapiClient::JournalsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**aggregate_journal_entry_credits_async**](JournalsApi.md#aggregate_journal_entry_credits_async) | **GET** /api/v2/AccountingService/Journals/{journalId}/Entries/Aggregate/Credits | Aggregate journal entry credits |
| [**aggregate_journal_entry_debits_async**](JournalsApi.md#aggregate_journal_entry_debits_async) | **GET** /api/v2/AccountingService/Journals/{journalId}/Entries/Aggregate/Debits | Aggregate journal entry debits |
| [**assign_journal_to_book_async**](JournalsApi.md#assign_journal_to_book_async) | **POST** /api/v2/AccountingService/Journals/{journalId}/AssignToBook | Bind a journal to a financial book |
| [**count_journals_async**](JournalsApi.md#count_journals_async) | **GET** /api/v2/AccountingService/Journals/Count | Count journals |
| [**create_journal_async**](JournalsApi.md#create_journal_async) | **POST** /api/v2/AccountingService/Journals | Create journal |
| [**create_journal_entry_async**](JournalsApi.md#create_journal_entry_async) | **POST** /api/v2/AccountingService/Journals/{journalId}/Entries | Create journal entry |
| [**delete_journal_async**](JournalsApi.md#delete_journal_async) | **DELETE** /api/v2/AccountingService/Journals/{journalId} | Delete journal |
| [**delete_journal_entry_async**](JournalsApi.md#delete_journal_entry_async) | **DELETE** /api/v2/AccountingService/Journals/{journalId}/Entries/{entryId} | Delete journal entry |
| [**get_journal_details_async**](JournalsApi.md#get_journal_details_async) | **GET** /api/v2/AccountingService/Journals/{journalId} | Get journal by ID |
| [**get_journal_entries_async**](JournalsApi.md#get_journal_entries_async) | **GET** /api/v2/AccountingService/Journals/{journalId}/Entries | Get journal entries |
| [**get_journal_entries_count_async**](JournalsApi.md#get_journal_entries_count_async) | **GET** /api/v2/AccountingService/Journals/{journalId}/Entries/Count | Count journal entries |
| [**get_journal_entry_details_async**](JournalsApi.md#get_journal_entry_details_async) | **GET** /api/v2/AccountingService/Journals/{journalId}/Entries/{entryId} | Get journal entry by ID |
| [**get_journals_async**](JournalsApi.md#get_journals_async) | **GET** /api/v2/AccountingService/Journals | Get all journals |
| [**patch_journal_async**](JournalsApi.md#patch_journal_async) | **PATCH** /api/v2/AccountingService/Journals/{journalId} | Patch a journal |
| [**patch_journal_entry_async**](JournalsApi.md#patch_journal_entry_async) | **PATCH** /api/v2/AccountingService/Journals/{journalId}/Entries/{entryId} | Patch a journal entry |
| [**post_journal_entry_async**](JournalsApi.md#post_journal_entry_async) | **POST** /api/v2/AccountingService/Journals/{journalId}/Entries/{entryId}/Post | Post a draft journal entry |
| [**reverse_journal_entry_async**](JournalsApi.md#reverse_journal_entry_async) | **POST** /api/v2/AccountingService/Journals/{journalId}/Entries/{entryId}/Reverse | Reverse a posted journal entry |
| [**update_journal_async**](JournalsApi.md#update_journal_async) | **PUT** /api/v2/AccountingService/Journals/{journalId} | Update journal |
| [**update_journal_entry_async**](JournalsApi.md#update_journal_entry_async) | **PUT** /api/v2/AccountingService/Journals/{journalId}/Entries/{entryId} | Update journal entry |


## aggregate_journal_entry_credits_async

> <MoneyEnvelope> aggregate_journal_entry_credits_async(tenant_id, journal_id, opts)

Aggregate journal entry credits

Returns the sum of all credit amounts for entries in the specified journal, normalized to the target currency.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  currency_id: 'currency_id_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  journal_entry_dto_collection_query_parameters: OpenapiClient::JournalEntryDtoCollectionQueryParameters.new # JournalEntryDtoCollectionQueryParameters | 
}

begin
  # Aggregate journal entry credits
  result = api_instance.aggregate_journal_entry_credits_async(tenant_id, journal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->aggregate_journal_entry_credits_async: #{e}"
end
```

#### Using the aggregate_journal_entry_credits_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MoneyEnvelope>, Integer, Hash)> aggregate_journal_entry_credits_async_with_http_info(tenant_id, journal_id, opts)

```ruby
begin
  # Aggregate journal entry credits
  data, status_code, headers = api_instance.aggregate_journal_entry_credits_async_with_http_info(tenant_id, journal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MoneyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->aggregate_journal_entry_credits_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_id** | **String** |  |  |
| **currency_id** | **String** |  | [optional][default to &#39;USD.USA&#39;] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **journal_entry_dto_collection_query_parameters** | [**JournalEntryDtoCollectionQueryParameters**](JournalEntryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## aggregate_journal_entry_debits_async

> <MoneyEnvelope> aggregate_journal_entry_debits_async(tenant_id, journal_id, opts)

Aggregate journal entry debits

Returns the sum of all debit amounts for entries in the specified journal, normalized to the target currency.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  currency_id: 'currency_id_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  journal_entry_dto_collection_query_parameters: OpenapiClient::JournalEntryDtoCollectionQueryParameters.new # JournalEntryDtoCollectionQueryParameters | 
}

begin
  # Aggregate journal entry debits
  result = api_instance.aggregate_journal_entry_debits_async(tenant_id, journal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->aggregate_journal_entry_debits_async: #{e}"
end
```

#### Using the aggregate_journal_entry_debits_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MoneyEnvelope>, Integer, Hash)> aggregate_journal_entry_debits_async_with_http_info(tenant_id, journal_id, opts)

```ruby
begin
  # Aggregate journal entry debits
  data, status_code, headers = api_instance.aggregate_journal_entry_debits_async_with_http_info(tenant_id, journal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MoneyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->aggregate_journal_entry_debits_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_id** | **String** |  |  |
| **currency_id** | **String** |  | [optional][default to &#39;USD.USA&#39;] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **journal_entry_dto_collection_query_parameters** | [**JournalEntryDtoCollectionQueryParameters**](JournalEntryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## assign_journal_to_book_async

> <EmptyEnvelope> assign_journal_to_book_async(tenant_id, journal_id, opts)

Bind a journal to a financial book

Establishes the one-way Journal↔FinancialBook binding (finish-line #5): binds an unbound journal to the supplied book and sets its book-scoped code, enforcing (Tenant, Book, Code) uniqueness. Binding an unbound journal or re-affirming the same book succeeds; a duplicate code in the book is rejected (400), and re-homing an already-bound journal to a DIFFERENT book is rejected by the aggregate. Requires the journals_update permission.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  assign_journal_to_book_request: OpenapiClient::AssignJournalToBookRequest.new({financial_book_id: 'financial_book_id_example', code: 'code_example'}) # AssignJournalToBookRequest | 
}

begin
  # Bind a journal to a financial book
  result = api_instance.assign_journal_to_book_async(tenant_id, journal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->assign_journal_to_book_async: #{e}"
end
```

#### Using the assign_journal_to_book_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> assign_journal_to_book_async_with_http_info(tenant_id, journal_id, opts)

```ruby
begin
  # Bind a journal to a financial book
  data, status_code, headers = api_instance.assign_journal_to_book_async_with_http_info(tenant_id, journal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->assign_journal_to_book_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **assign_journal_to_book_request** | [**AssignJournalToBookRequest**](AssignJournalToBookRequest.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## count_journals_async

> <Int32Envelope> count_journals_async(tenant_id, opts)

Count journals

Returns the count of journals for the tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  journal_dto_collection_query_parameters: OpenapiClient::JournalDtoCollectionQueryParameters.new # JournalDtoCollectionQueryParameters | 
}

begin
  # Count journals
  result = api_instance.count_journals_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->count_journals_async: #{e}"
end
```

#### Using the count_journals_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_journals_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count journals
  data, status_code, headers = api_instance.count_journals_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->count_journals_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **journal_dto_collection_query_parameters** | [**JournalDtoCollectionQueryParameters**](JournalDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_journal_async

> <EmptyEnvelope> create_journal_async(tenant_id, opts)

Create journal

Creates a new journal for the tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  journal_create_dto: OpenapiClient::JournalCreateDto.new({name: 'name_example'}) # JournalCreateDto | 
}

begin
  # Create journal
  result = api_instance.create_journal_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->create_journal_async: #{e}"
end
```

#### Using the create_journal_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_journal_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create journal
  data, status_code, headers = api_instance.create_journal_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->create_journal_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **journal_create_dto** | [**JournalCreateDto**](JournalCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_journal_entry_async

> <EmptyEnvelope> create_journal_entry_async(tenant_id, journal_id, opts)

Create journal entry

Creates a new journal entry for a given journal.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  journal_entry_create_dto: OpenapiClient::JournalEntryCreateDto.new({journal_id: 'journal_id_example', fiscal_period_id: 'fiscal_period_id_example', transaction_currency_id: 'transaction_currency_id_example', description: 'description_example'}) # JournalEntryCreateDto | 
}

begin
  # Create journal entry
  result = api_instance.create_journal_entry_async(tenant_id, journal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->create_journal_entry_async: #{e}"
end
```

#### Using the create_journal_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_journal_entry_async_with_http_info(tenant_id, journal_id, opts)

```ruby
begin
  # Create journal entry
  data, status_code, headers = api_instance.create_journal_entry_async_with_http_info(tenant_id, journal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->create_journal_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **journal_entry_create_dto** | [**JournalEntryCreateDto**](JournalEntryCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_journal_async

> <EmptyEnvelope> delete_journal_async(tenant_id, journal_id, opts)

Delete journal

Deletes a journal by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete journal
  result = api_instance.delete_journal_async(tenant_id, journal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->delete_journal_async: #{e}"
end
```

#### Using the delete_journal_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_journal_async_with_http_info(tenant_id, journal_id, opts)

```ruby
begin
  # Delete journal
  data, status_code, headers = api_instance.delete_journal_async_with_http_info(tenant_id, journal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->delete_journal_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_journal_entry_async

> <EmptyEnvelope> delete_journal_entry_async(tenant_id, journal_id, entry_id, opts)

Delete journal entry

Deletes a specific journal entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete journal entry
  result = api_instance.delete_journal_entry_async(tenant_id, journal_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->delete_journal_entry_async: #{e}"
end
```

#### Using the delete_journal_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_journal_entry_async_with_http_info(tenant_id, journal_id, entry_id, opts)

```ruby
begin
  # Delete journal entry
  data, status_code, headers = api_instance.delete_journal_entry_async_with_http_info(tenant_id, journal_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->delete_journal_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_id** | **String** |  |  |
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


## get_journal_details_async

> <JournalDtoEnvelope> get_journal_details_async(tenant_id, journal_id, opts)

Get journal by ID

Retrieves the details of a journal.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get journal by ID
  result = api_instance.get_journal_details_async(tenant_id, journal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->get_journal_details_async: #{e}"
end
```

#### Using the get_journal_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JournalDtoEnvelope>, Integer, Hash)> get_journal_details_async_with_http_info(tenant_id, journal_id, opts)

```ruby
begin
  # Get journal by ID
  data, status_code, headers = api_instance.get_journal_details_async_with_http_info(tenant_id, journal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JournalDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->get_journal_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**JournalDtoEnvelope**](JournalDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_journal_entries_async

> <JournalEntryDtoIReadOnlyListEnvelope> get_journal_entries_async(tenant_id, journal_id, opts)

Get journal entries

Gets entries for the specified journal.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  journal_entry_dto_collection_query_parameters: OpenapiClient::JournalEntryDtoCollectionQueryParameters.new # JournalEntryDtoCollectionQueryParameters | 
}

begin
  # Get journal entries
  result = api_instance.get_journal_entries_async(tenant_id, journal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->get_journal_entries_async: #{e}"
end
```

#### Using the get_journal_entries_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JournalEntryDtoIReadOnlyListEnvelope>, Integer, Hash)> get_journal_entries_async_with_http_info(tenant_id, journal_id, opts)

```ruby
begin
  # Get journal entries
  data, status_code, headers = api_instance.get_journal_entries_async_with_http_info(tenant_id, journal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JournalEntryDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->get_journal_entries_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **journal_entry_dto_collection_query_parameters** | [**JournalEntryDtoCollectionQueryParameters**](JournalEntryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**JournalEntryDtoIReadOnlyListEnvelope**](JournalEntryDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_journal_entries_count_async

> <Int32Envelope> get_journal_entries_count_async(tenant_id, journal_id, opts)

Count journal entries

Returns the number of entries in the specified journal.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  journal_entry_dto_collection_query_parameters: OpenapiClient::JournalEntryDtoCollectionQueryParameters.new # JournalEntryDtoCollectionQueryParameters | 
}

begin
  # Count journal entries
  result = api_instance.get_journal_entries_count_async(tenant_id, journal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->get_journal_entries_count_async: #{e}"
end
```

#### Using the get_journal_entries_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_journal_entries_count_async_with_http_info(tenant_id, journal_id, opts)

```ruby
begin
  # Count journal entries
  data, status_code, headers = api_instance.get_journal_entries_count_async_with_http_info(tenant_id, journal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->get_journal_entries_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **journal_entry_dto_collection_query_parameters** | [**JournalEntryDtoCollectionQueryParameters**](JournalEntryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_journal_entry_details_async

> <JournalEntryDtoEnvelope> get_journal_entry_details_async(tenant_id, journal_id, entry_id, opts)

Get journal entry by ID

Retrieves a single journal entry WITH its hydrated posting lines — each line's account, direction, description and currency facets (transaction / functional / account / USD).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get journal entry by ID
  result = api_instance.get_journal_entry_details_async(tenant_id, journal_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->get_journal_entry_details_async: #{e}"
end
```

#### Using the get_journal_entry_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JournalEntryDtoEnvelope>, Integer, Hash)> get_journal_entry_details_async_with_http_info(tenant_id, journal_id, entry_id, opts)

```ruby
begin
  # Get journal entry by ID
  data, status_code, headers = api_instance.get_journal_entry_details_async_with_http_info(tenant_id, journal_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JournalEntryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->get_journal_entry_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_id** | **String** |  |  |
| **entry_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**JournalEntryDtoEnvelope**](JournalEntryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_journals_async

> <JournalDtoIReadOnlyListEnvelope> get_journals_async(tenant_id, opts)

Get all journals

Retrieves all journals for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  journal_dto_collection_query_parameters: OpenapiClient::JournalDtoCollectionQueryParameters.new # JournalDtoCollectionQueryParameters | 
}

begin
  # Get all journals
  result = api_instance.get_journals_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->get_journals_async: #{e}"
end
```

#### Using the get_journals_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JournalDtoIReadOnlyListEnvelope>, Integer, Hash)> get_journals_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all journals
  data, status_code, headers = api_instance.get_journals_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JournalDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->get_journals_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **journal_dto_collection_query_parameters** | [**JournalDtoCollectionQueryParameters**](JournalDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**JournalDtoIReadOnlyListEnvelope**](JournalDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_journal_async

> <EmptyEnvelope> patch_journal_async(tenant_id, journal_id, opts)

Patch a journal

Partially updates a journal.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a journal
  result = api_instance.patch_journal_async(tenant_id, journal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->patch_journal_async: #{e}"
end
```

#### Using the patch_journal_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_journal_async_with_http_info(tenant_id, journal_id, opts)

```ruby
begin
  # Patch a journal
  data, status_code, headers = api_instance.patch_journal_async_with_http_info(tenant_id, journal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->patch_journal_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_id** | **String** |  |  |
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


## patch_journal_entry_async

> <EmptyEnvelope> patch_journal_entry_async(tenant_id, journal_id, entry_id, opts)

Patch a journal entry

Partially updates a journal entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a journal entry
  result = api_instance.patch_journal_entry_async(tenant_id, journal_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->patch_journal_entry_async: #{e}"
end
```

#### Using the patch_journal_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_journal_entry_async_with_http_info(tenant_id, journal_id, entry_id, opts)

```ruby
begin
  # Patch a journal entry
  data, status_code, headers = api_instance.patch_journal_entry_async_with_http_info(tenant_id, journal_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->patch_journal_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_id** | **String** |  |  |
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


## post_journal_entry_async

> <EmptyEnvelope> post_journal_entry_async(tenant_id, journal_id, entry_id, opts)

Post a draft journal entry

Posts a DRAFT journal entry into its own open fiscal period. Enforces the balanced-entry invariant and the open-period gate, then seals the entry (immutable — correct via reversal, never edit/delete). An unbalanced draft or a closed period is rejected. Requires the journals_post permission.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Post a draft journal entry
  result = api_instance.post_journal_entry_async(tenant_id, journal_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->post_journal_entry_async: #{e}"
end
```

#### Using the post_journal_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> post_journal_entry_async_with_http_info(tenant_id, journal_id, entry_id, opts)

```ruby
begin
  # Post a draft journal entry
  data, status_code, headers = api_instance.post_journal_entry_async_with_http_info(tenant_id, journal_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->post_journal_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_id** | **String** |  |  |
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


## reverse_journal_entry_async

> <EmptyEnvelope> reverse_journal_entry_async(tenant_id, journal_id, entry_id, opts)

Reverse a posted journal entry

Reverses a POSTED journal entry by writing a balanced compensating counter-entry into the supplied open fiscal period and marking the original Reversed — one atomic operation (append-only audit trail). Requires the journals_reverse permission.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  reverse_journal_entry_request: OpenapiClient::ReverseJournalEntryRequest.new({reversal_period_id: 'reversal_period_id_example'}) # ReverseJournalEntryRequest | 
}

begin
  # Reverse a posted journal entry
  result = api_instance.reverse_journal_entry_async(tenant_id, journal_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->reverse_journal_entry_async: #{e}"
end
```

#### Using the reverse_journal_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> reverse_journal_entry_async_with_http_info(tenant_id, journal_id, entry_id, opts)

```ruby
begin
  # Reverse a posted journal entry
  data, status_code, headers = api_instance.reverse_journal_entry_async_with_http_info(tenant_id, journal_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->reverse_journal_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_id** | **String** |  |  |
| **entry_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **reverse_journal_entry_request** | [**ReverseJournalEntryRequest**](ReverseJournalEntryRequest.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_journal_async

> <EmptyEnvelope> update_journal_async(tenant_id, journal_id, opts)

Update journal

Updates an existing journal.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  journal_update_dto: OpenapiClient::JournalUpdateDto.new # JournalUpdateDto | 
}

begin
  # Update journal
  result = api_instance.update_journal_async(tenant_id, journal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->update_journal_async: #{e}"
end
```

#### Using the update_journal_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_journal_async_with_http_info(tenant_id, journal_id, opts)

```ruby
begin
  # Update journal
  data, status_code, headers = api_instance.update_journal_async_with_http_info(tenant_id, journal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->update_journal_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **journal_update_dto** | [**JournalUpdateDto**](JournalUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_journal_entry_async

> <EmptyEnvelope> update_journal_entry_async(tenant_id, journal_id, entry_id, opts)

Update journal entry

Updates a specific journal entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JournalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
journal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  journal_entry_update_dto: OpenapiClient::JournalEntryUpdateDto.new({fiscal_period_id: 'fiscal_period_id_example', transaction_currency_id: 'transaction_currency_id_example', description: 'description_example'}) # JournalEntryUpdateDto | 
}

begin
  # Update journal entry
  result = api_instance.update_journal_entry_async(tenant_id, journal_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->update_journal_entry_async: #{e}"
end
```

#### Using the update_journal_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_journal_entry_async_with_http_info(tenant_id, journal_id, entry_id, opts)

```ruby
begin
  # Update journal entry
  data, status_code, headers = api_instance.update_journal_entry_async_with_http_info(tenant_id, journal_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JournalsApi->update_journal_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **journal_id** | **String** |  |  |
| **entry_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **journal_entry_update_dto** | [**JournalEntryUpdateDto**](JournalEntryUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

