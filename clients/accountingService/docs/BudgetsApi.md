# OpenapiClient::BudgetsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_budget_account_entry_async**](BudgetsApi.md#create_budget_account_entry_async) | **POST** /api/v2/AccountingService/Budgets/{budgetId}/AccountEntries | Creates a budget account entry |
| [**create_budget_async**](BudgetsApi.md#create_budget_async) | **POST** /api/v2/AccountingService/Budgets | Creates a budget |
| [**delete_budget_account_entry_async**](BudgetsApi.md#delete_budget_account_entry_async) | **DELETE** /api/v2/AccountingService/Budgets/{budgetId}/AccountEntries/{entryId} | Deletes a budget account entry |
| [**delete_budget_async**](BudgetsApi.md#delete_budget_async) | **DELETE** /api/v2/AccountingService/Budgets/{budgetId} | Deletes a budget |
| [**get_budget_account_entries_collection_async**](BudgetsApi.md#get_budget_account_entries_collection_async) | **GET** /api/v2/AccountingService/Budgets/{budgetId}/AccountEntries | Gets all budget account entries |
| [**get_budget_account_entry_async**](BudgetsApi.md#get_budget_account_entry_async) | **GET** /api/v2/AccountingService/Budgets/{budgetId}/AccountEntries/{entryId} | Gets a budget account entry by id |
| [**get_budget_details_async**](BudgetsApi.md#get_budget_details_async) | **GET** /api/v2/AccountingService/Budgets/{budgetId} | Gets a budget by id |
| [**get_budgets_async**](BudgetsApi.md#get_budgets_async) | **GET** /api/v2/AccountingService/Budgets | Gets all budgets |
| [**get_budgets_count_async**](BudgetsApi.md#get_budgets_count_async) | **GET** /api/v2/AccountingService/Budgets/Count | Get the count of budgets |
| [**patch_budget_account_entry_async**](BudgetsApi.md#patch_budget_account_entry_async) | **PATCH** /api/v2/AccountingService/Budgets/{budgetId}/AccountEntries/{entryId} | Patches a budget account entry |
| [**patch_budget_async**](BudgetsApi.md#patch_budget_async) | **PATCH** /api/v2/AccountingService/Budgets/{budgetId} | Patches a budget |
| [**update_budget_account_entry_async**](BudgetsApi.md#update_budget_account_entry_async) | **PUT** /api/v2/AccountingService/Budgets/{budgetId}/AccountEntries/{entryId} | Updates a budget account entry |
| [**update_budget_async**](BudgetsApi.md#update_budget_async) | **PUT** /api/v2/AccountingService/Budgets/{budgetId} | Updates a budget |


## create_budget_account_entry_async

> <EmptyEnvelope> create_budget_account_entry_async(tenant_id, budget_id, budget_account_entry_create_dto, opts)

Creates a budget account entry

Create a budget account entry

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BudgetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
budget_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
budget_account_entry_create_dto = OpenapiClient::BudgetAccountEntryCreateDto.new({description: 'description_example', currency_id: 'currency_id_example'}) # BudgetAccountEntryCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Creates a budget account entry
  result = api_instance.create_budget_account_entry_async(tenant_id, budget_id, budget_account_entry_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->create_budget_account_entry_async: #{e}"
end
```

#### Using the create_budget_account_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_budget_account_entry_async_with_http_info(tenant_id, budget_id, budget_account_entry_create_dto, opts)

```ruby
begin
  # Creates a budget account entry
  data, status_code, headers = api_instance.create_budget_account_entry_async_with_http_info(tenant_id, budget_id, budget_account_entry_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->create_budget_account_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **budget_id** | **String** |  |  |
| **budget_account_entry_create_dto** | [**BudgetAccountEntryCreateDto**](BudgetAccountEntryCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_budget_async

> <EmptyEnvelope> create_budget_async(tenant_id, budget_create_dto, opts)

Creates a budget

Create a budget

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BudgetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
budget_create_dto = OpenapiClient::BudgetCreateDto.new # BudgetCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Creates a budget
  result = api_instance.create_budget_async(tenant_id, budget_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->create_budget_async: #{e}"
end
```

#### Using the create_budget_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_budget_async_with_http_info(tenant_id, budget_create_dto, opts)

```ruby
begin
  # Creates a budget
  data, status_code, headers = api_instance.create_budget_async_with_http_info(tenant_id, budget_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->create_budget_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **budget_create_dto** | [**BudgetCreateDto**](BudgetCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_budget_account_entry_async

> <EmptyEnvelope> delete_budget_account_entry_async(tenant_id, budget_id, entry_id, opts)

Deletes a budget account entry

Delete a budget account entry

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BudgetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
budget_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes a budget account entry
  result = api_instance.delete_budget_account_entry_async(tenant_id, budget_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->delete_budget_account_entry_async: #{e}"
end
```

#### Using the delete_budget_account_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_budget_account_entry_async_with_http_info(tenant_id, budget_id, entry_id, opts)

```ruby
begin
  # Deletes a budget account entry
  data, status_code, headers = api_instance.delete_budget_account_entry_async_with_http_info(tenant_id, budget_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->delete_budget_account_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **budget_id** | **String** |  |  |
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


## delete_budget_async

> <EmptyEnvelope> delete_budget_async(tenant_id, budget_id, opts)

Deletes a budget

Delete a budget

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BudgetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
budget_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes a budget
  result = api_instance.delete_budget_async(tenant_id, budget_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->delete_budget_async: #{e}"
end
```

#### Using the delete_budget_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_budget_async_with_http_info(tenant_id, budget_id, opts)

```ruby
begin
  # Deletes a budget
  data, status_code, headers = api_instance.delete_budget_async_with_http_info(tenant_id, budget_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->delete_budget_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **budget_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_budget_account_entries_collection_async

> <BudgetAccountEntryDtoIReadOnlyListEnvelope> get_budget_account_entries_collection_async(tenant_id, budget_id, opts)

Gets all budget account entries

Get all budget account entries

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BudgetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
budget_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets all budget account entries
  result = api_instance.get_budget_account_entries_collection_async(tenant_id, budget_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->get_budget_account_entries_collection_async: #{e}"
end
```

#### Using the get_budget_account_entries_collection_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BudgetAccountEntryDtoIReadOnlyListEnvelope>, Integer, Hash)> get_budget_account_entries_collection_async_with_http_info(tenant_id, budget_id, opts)

```ruby
begin
  # Gets all budget account entries
  data, status_code, headers = api_instance.get_budget_account_entries_collection_async_with_http_info(tenant_id, budget_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BudgetAccountEntryDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->get_budget_account_entries_collection_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **budget_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BudgetAccountEntryDtoIReadOnlyListEnvelope**](BudgetAccountEntryDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_budget_account_entry_async

> <BudgetAccountEntryDtoEnvelope> get_budget_account_entry_async(tenant_id, budget_id, entry_id, opts)

Gets a budget account entry by id

Get a budget account entry by id

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BudgetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
budget_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets a budget account entry by id
  result = api_instance.get_budget_account_entry_async(tenant_id, budget_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->get_budget_account_entry_async: #{e}"
end
```

#### Using the get_budget_account_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BudgetAccountEntryDtoEnvelope>, Integer, Hash)> get_budget_account_entry_async_with_http_info(tenant_id, budget_id, entry_id, opts)

```ruby
begin
  # Gets a budget account entry by id
  data, status_code, headers = api_instance.get_budget_account_entry_async_with_http_info(tenant_id, budget_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BudgetAccountEntryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->get_budget_account_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **budget_id** | **String** |  |  |
| **entry_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BudgetAccountEntryDtoEnvelope**](BudgetAccountEntryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_budget_details_async

> <BudgetDtoEnvelope> get_budget_details_async(tenant_id, budget_id, opts)

Gets a budget by id

Get a budget by id

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BudgetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
budget_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets a budget by id
  result = api_instance.get_budget_details_async(tenant_id, budget_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->get_budget_details_async: #{e}"
end
```

#### Using the get_budget_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BudgetDtoEnvelope>, Integer, Hash)> get_budget_details_async_with_http_info(tenant_id, budget_id, opts)

```ruby
begin
  # Gets a budget by id
  data, status_code, headers = api_instance.get_budget_details_async_with_http_info(tenant_id, budget_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BudgetDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->get_budget_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **budget_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BudgetDtoEnvelope**](BudgetDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_budgets_async

> <BudgetDtoIReadOnlyListEnvelope> get_budgets_async(tenant_id, opts)

Gets all budgets

Get all budgets

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BudgetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets all budgets
  result = api_instance.get_budgets_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->get_budgets_async: #{e}"
end
```

#### Using the get_budgets_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BudgetDtoIReadOnlyListEnvelope>, Integer, Hash)> get_budgets_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets all budgets
  data, status_code, headers = api_instance.get_budgets_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BudgetDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->get_budgets_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BudgetDtoIReadOnlyListEnvelope**](BudgetDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_budgets_count_async

> <Int32Envelope> get_budgets_count_async(tenant_id, opts)

Get the count of budgets

Get the count of budgets.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BudgetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of budgets
  result = api_instance.get_budgets_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->get_budgets_count_async: #{e}"
end
```

#### Using the get_budgets_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_budgets_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of budgets
  data, status_code, headers = api_instance.get_budgets_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->get_budgets_count_async_with_http_info: #{e}"
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


## patch_budget_account_entry_async

> <EmptyEnvelope> patch_budget_account_entry_async(tenant_id, budget_id, entry_id, opts)

Patches a budget account entry

Partially update a budget account entry using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BudgetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
budget_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patches a budget account entry
  result = api_instance.patch_budget_account_entry_async(tenant_id, budget_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->patch_budget_account_entry_async: #{e}"
end
```

#### Using the patch_budget_account_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_budget_account_entry_async_with_http_info(tenant_id, budget_id, entry_id, opts)

```ruby
begin
  # Patches a budget account entry
  data, status_code, headers = api_instance.patch_budget_account_entry_async_with_http_info(tenant_id, budget_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->patch_budget_account_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **budget_id** | **String** |  |  |
| **entry_id** | **String** |  |  |
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


## patch_budget_async

> <EmptyEnvelope> patch_budget_async(tenant_id, budget_id, opts)

Patches a budget

Partially update a budget using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BudgetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
budget_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patches a budget
  result = api_instance.patch_budget_async(tenant_id, budget_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->patch_budget_async: #{e}"
end
```

#### Using the patch_budget_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_budget_async_with_http_info(tenant_id, budget_id, opts)

```ruby
begin
  # Patches a budget
  data, status_code, headers = api_instance.patch_budget_async_with_http_info(tenant_id, budget_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->patch_budget_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **budget_id** | **String** |  |  |
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


## update_budget_account_entry_async

> <EmptyEnvelope> update_budget_account_entry_async(tenant_id, budget_id, entry_id, budget_account_entry_update_dto, opts)

Updates a budget account entry

Update a budget account entry

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BudgetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
budget_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
budget_account_entry_update_dto = OpenapiClient::BudgetAccountEntryUpdateDto.new # BudgetAccountEntryUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Updates a budget account entry
  result = api_instance.update_budget_account_entry_async(tenant_id, budget_id, entry_id, budget_account_entry_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->update_budget_account_entry_async: #{e}"
end
```

#### Using the update_budget_account_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_budget_account_entry_async_with_http_info(tenant_id, budget_id, entry_id, budget_account_entry_update_dto, opts)

```ruby
begin
  # Updates a budget account entry
  data, status_code, headers = api_instance.update_budget_account_entry_async_with_http_info(tenant_id, budget_id, entry_id, budget_account_entry_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->update_budget_account_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **budget_id** | **String** |  |  |
| **entry_id** | **String** |  |  |
| **budget_account_entry_update_dto** | [**BudgetAccountEntryUpdateDto**](BudgetAccountEntryUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_budget_async

> <EmptyEnvelope> update_budget_async(tenant_id, budget_id, budget_update_dto, opts)

Updates a budget

Update a budget

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BudgetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
budget_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
budget_update_dto = OpenapiClient::BudgetUpdateDto.new # BudgetUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Updates a budget
  result = api_instance.update_budget_async(tenant_id, budget_id, budget_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->update_budget_async: #{e}"
end
```

#### Using the update_budget_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_budget_async_with_http_info(tenant_id, budget_id, budget_update_dto, opts)

```ruby
begin
  # Updates a budget
  data, status_code, headers = api_instance.update_budget_async_with_http_info(tenant_id, budget_id, budget_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BudgetsApi->update_budget_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **budget_id** | **String** |  |  |
| **budget_update_dto** | [**BudgetUpdateDto**](BudgetUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

