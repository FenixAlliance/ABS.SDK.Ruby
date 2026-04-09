# OpenapiClient::JournalsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_journals_async**](JournalsApi.md#count_journals_async) | **GET** /api/v2/AccountingService/Journals/Count | Count journals |
| [**create_journal_async**](JournalsApi.md#create_journal_async) | **POST** /api/v2/AccountingService/Journals | Create journal |
| [**create_journal_entry_async**](JournalsApi.md#create_journal_entry_async) | **POST** /api/v2/AccountingService/Journals/{journalId}/Entries | Create journal entry |
| [**delete_journal_async**](JournalsApi.md#delete_journal_async) | **DELETE** /api/v2/AccountingService/Journals/{journalId} | Delete journal |
| [**delete_journal_entry_async**](JournalsApi.md#delete_journal_entry_async) | **DELETE** /api/v2/AccountingService/Journals/{journalId}/Entries/{entryId} | Delete journal entry |
| [**get_journal_details_async**](JournalsApi.md#get_journal_details_async) | **GET** /api/v2/AccountingService/Journals/{journalId} | Get journal by ID |
| [**get_journal_entries_async**](JournalsApi.md#get_journal_entries_async) | **GET** /api/v2/AccountingService/Journals/{journalId}/Entries | Get journal entries |
| [**get_journal_entries_count_async**](JournalsApi.md#get_journal_entries_count_async) | **GET** /api/v2/AccountingService/Journals/{journalId}/Entries/Count | Count journal entries |
| [**get_journals_async**](JournalsApi.md#get_journals_async) | **GET** /api/v2/AccountingService/Journals | Get all journals |
| [**update_journal_async**](JournalsApi.md#update_journal_async) | **PUT** /api/v2/AccountingService/Journals/{journalId} | Update journal |
| [**update_journal_entry_async**](JournalsApi.md#update_journal_entry_async) | **PUT** /api/v2/AccountingService/Journals/{journalId}/Entries/{entryId} | Update journal entry |


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
  x_api_version: 'x_api_version_example' # String | 
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

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
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
  journal_entry_create_dto: OpenapiClient::JournalEntryCreateDto.new({description: 'description_example', date: Time.now, journal_id: 'journal_id_example', currency_id: 'currency_id_example', debit_account_id: 'debit_account_id_example', credit_account_id: 'credit_account_id_example'}) # JournalEntryCreateDto | 
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
  x_api_version: 'x_api_version_example' # String | 
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

### Return type

[**JournalEntryDtoIReadOnlyListEnvelope**](JournalEntryDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
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
  x_api_version: 'x_api_version_example' # String | 
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

### Return type

[**Int32Envelope**](Int32Envelope.md)

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
  x_api_version: 'x_api_version_example' # String | 
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

### Return type

[**JournalDtoIReadOnlyListEnvelope**](JournalDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
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
  journal_entry_update_dto: OpenapiClient::JournalEntryUpdateDto.new({description: 'description_example', date: Time.now, journal_id: 'journal_id_example', currency_id: 'currency_id_example', debit_account_id: 'debit_account_id_example', credit_account_id: 'credit_account_id_example'}) # JournalEntryUpdateDto | 
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

