# OpenapiClient::DiscountListsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_discount_list**](DiscountListsApi.md#create_discount_list) | **POST** /api/v2/PricingService/DiscountLists | Creates a new discount list |
| [**create_discount_list_entry**](DiscountListsApi.md#create_discount_list_entry) | **POST** /api/v2/PricingService/DiscountLists/{discountListId}/Discounts | Creates a discount list entry |
| [**delete_discount_list**](DiscountListsApi.md#delete_discount_list) | **DELETE** /api/v2/PricingService/DiscountLists/{discountListId} | Deletes a discount list |
| [**delete_discount_list_entry**](DiscountListsApi.md#delete_discount_list_entry) | **DELETE** /api/v2/PricingService/DiscountLists/{discountListId}/Discounts/{discountListEntryId} | Deletes a discount list entry |
| [**get_discount_list**](DiscountListsApi.md#get_discount_list) | **GET** /api/v2/PricingService/DiscountLists/{discountListId} | Gets a discount list by ID |
| [**get_discount_list_entries**](DiscountListsApi.md#get_discount_list_entries) | **GET** /api/v2/PricingService/DiscountLists/{discountListId}/Discounts | Retrieves discounts in a discount list |
| [**get_discount_list_entries_count**](DiscountListsApi.md#get_discount_list_entries_count) | **GET** /api/v2/PricingService/DiscountLists/{discountListId}/Discounts/Count | Counts discounts in a discount list |
| [**get_discount_list_entry**](DiscountListsApi.md#get_discount_list_entry) | **GET** /api/v2/PricingService/DiscountLists/{discountListId}/Discounts/{discountListEntryId} | Gets a discount list entry by ID |
| [**get_discount_lists**](DiscountListsApi.md#get_discount_lists) | **GET** /api/v2/PricingService/DiscountLists | Retrieves all discount lists |
| [**get_discount_lists_count**](DiscountListsApi.md#get_discount_lists_count) | **GET** /api/v2/PricingService/DiscountLists/Count | Counts discount lists |
| [**patch_discount_list**](DiscountListsApi.md#patch_discount_list) | **PATCH** /api/v2/PricingService/DiscountLists/{discountListId} | Patches a discount list |
| [**patch_discount_list_entry**](DiscountListsApi.md#patch_discount_list_entry) | **PATCH** /api/v2/PricingService/DiscountLists/{discountListId}/Discounts/{discountListEntryId} | Patches a discount list entry |
| [**update_discount_list**](DiscountListsApi.md#update_discount_list) | **PUT** /api/v2/PricingService/DiscountLists/{discountListId} | Updates a discount list |
| [**update_discount_list_entry**](DiscountListsApi.md#update_discount_list_entry) | **PUT** /api/v2/PricingService/DiscountLists/{discountListId}/Discounts/{discountListEntryId} | Updates a discount list entry |


## create_discount_list

> <EmptyEnvelope> create_discount_list(tenant_id, opts)

Creates a new discount list

Creates a new discount list for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DiscountListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  discount_list_create_dto: OpenapiClient::DiscountListCreateDto.new # DiscountListCreateDto | 
}

begin
  # Creates a new discount list
  result = api_instance.create_discount_list(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->create_discount_list: #{e}"
end
```

#### Using the create_discount_list_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_discount_list_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new discount list
  data, status_code, headers = api_instance.create_discount_list_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->create_discount_list_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **discount_list_create_dto** | [**DiscountListCreateDto**](DiscountListCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_discount_list_entry

> <EmptyEnvelope> create_discount_list_entry(tenant_id, discount_list_id, opts)

Creates a discount list entry

Creates a new discount entry in the specified discount list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DiscountListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
discount_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  discount_create_dto: OpenapiClient::DiscountCreateDto.new # DiscountCreateDto | 
}

begin
  # Creates a discount list entry
  result = api_instance.create_discount_list_entry(tenant_id, discount_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->create_discount_list_entry: #{e}"
end
```

#### Using the create_discount_list_entry_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_discount_list_entry_with_http_info(tenant_id, discount_list_id, opts)

```ruby
begin
  # Creates a discount list entry
  data, status_code, headers = api_instance.create_discount_list_entry_with_http_info(tenant_id, discount_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->create_discount_list_entry_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **discount_list_id** | **String** |  |  |
| **discount_create_dto** | [**DiscountCreateDto**](DiscountCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_discount_list

> <EmptyEnvelope> delete_discount_list(tenant_id, discount_list_id)

Deletes a discount list

Deletes the specified discount list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DiscountListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
discount_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes a discount list
  result = api_instance.delete_discount_list(tenant_id, discount_list_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->delete_discount_list: #{e}"
end
```

#### Using the delete_discount_list_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_discount_list_with_http_info(tenant_id, discount_list_id)

```ruby
begin
  # Deletes a discount list
  data, status_code, headers = api_instance.delete_discount_list_with_http_info(tenant_id, discount_list_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->delete_discount_list_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **discount_list_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_discount_list_entry

> <EmptyEnvelope> delete_discount_list_entry(tenant_id, discount_list_id, discount_list_entry_id)

Deletes a discount list entry

Deletes the specified discount entry from a discount list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DiscountListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
discount_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
discount_list_entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes a discount list entry
  result = api_instance.delete_discount_list_entry(tenant_id, discount_list_id, discount_list_entry_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->delete_discount_list_entry: #{e}"
end
```

#### Using the delete_discount_list_entry_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_discount_list_entry_with_http_info(tenant_id, discount_list_id, discount_list_entry_id)

```ruby
begin
  # Deletes a discount list entry
  data, status_code, headers = api_instance.delete_discount_list_entry_with_http_info(tenant_id, discount_list_id, discount_list_entry_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->delete_discount_list_entry_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **discount_list_id** | **String** |  |  |
| **discount_list_entry_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_discount_list

> <DiscountListDtoEnvelope> get_discount_list(tenant_id, discount_list_id)

Gets a discount list by ID

Retrieves the details of a discount list using its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DiscountListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
discount_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a discount list by ID
  result = api_instance.get_discount_list(tenant_id, discount_list_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->get_discount_list: #{e}"
end
```

#### Using the get_discount_list_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<DiscountListDtoEnvelope>, Integer, Hash)> get_discount_list_with_http_info(tenant_id, discount_list_id)

```ruby
begin
  # Gets a discount list by ID
  data, status_code, headers = api_instance.get_discount_list_with_http_info(tenant_id, discount_list_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <DiscountListDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->get_discount_list_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **discount_list_id** | **String** |  |  |

### Return type

[**DiscountListDtoEnvelope**](DiscountListDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_discount_list_entries

> <DiscountDtoListEnvelope> get_discount_list_entries(tenant_id, discount_list_id, opts)

Retrieves discounts in a discount list

Gets all discount entries for a specific discount list with OData support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DiscountListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
discount_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  discount_dto_collection_query_parameters: OpenapiClient::DiscountDtoCollectionQueryParameters.new # DiscountDtoCollectionQueryParameters | 
}

begin
  # Retrieves discounts in a discount list
  result = api_instance.get_discount_list_entries(tenant_id, discount_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->get_discount_list_entries: #{e}"
end
```

#### Using the get_discount_list_entries_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<DiscountDtoListEnvelope>, Integer, Hash)> get_discount_list_entries_with_http_info(tenant_id, discount_list_id, opts)

```ruby
begin
  # Retrieves discounts in a discount list
  data, status_code, headers = api_instance.get_discount_list_entries_with_http_info(tenant_id, discount_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <DiscountDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->get_discount_list_entries_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **discount_list_id** | **String** |  |  |
| **discount_dto_collection_query_parameters** | [**DiscountDtoCollectionQueryParameters**](DiscountDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**DiscountDtoListEnvelope**](DiscountDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_discount_list_entries_count

> <Int32Envelope> get_discount_list_entries_count(tenant_id, discount_list_id, opts)

Counts discounts in a discount list

Gets the count of discount entries for a specific discount list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DiscountListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
discount_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  discount_dto_collection_query_parameters: OpenapiClient::DiscountDtoCollectionQueryParameters.new # DiscountDtoCollectionQueryParameters | 
}

begin
  # Counts discounts in a discount list
  result = api_instance.get_discount_list_entries_count(tenant_id, discount_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->get_discount_list_entries_count: #{e}"
end
```

#### Using the get_discount_list_entries_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_discount_list_entries_count_with_http_info(tenant_id, discount_list_id, opts)

```ruby
begin
  # Counts discounts in a discount list
  data, status_code, headers = api_instance.get_discount_list_entries_count_with_http_info(tenant_id, discount_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->get_discount_list_entries_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **discount_list_id** | **String** |  |  |
| **discount_dto_collection_query_parameters** | [**DiscountDtoCollectionQueryParameters**](DiscountDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_discount_list_entry

> <DiscountDtoEnvelope> get_discount_list_entry(tenant_id, discount_list_id, discount_list_entry_id)

Gets a discount list entry by ID

Retrieves a specific discount entry from a discount list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DiscountListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
discount_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
discount_list_entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a discount list entry by ID
  result = api_instance.get_discount_list_entry(tenant_id, discount_list_id, discount_list_entry_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->get_discount_list_entry: #{e}"
end
```

#### Using the get_discount_list_entry_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<DiscountDtoEnvelope>, Integer, Hash)> get_discount_list_entry_with_http_info(tenant_id, discount_list_id, discount_list_entry_id)

```ruby
begin
  # Gets a discount list entry by ID
  data, status_code, headers = api_instance.get_discount_list_entry_with_http_info(tenant_id, discount_list_id, discount_list_entry_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <DiscountDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->get_discount_list_entry_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **discount_list_id** | **String** |  |  |
| **discount_list_entry_id** | **String** |  |  |

### Return type

[**DiscountDtoEnvelope**](DiscountDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_discount_lists

> <DiscountListDtoListEnvelope> get_discount_lists(tenant_id, opts)

Retrieves all discount lists

Gets all discount lists for the current tenant with OData support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DiscountListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  discount_list_dto_collection_query_parameters: OpenapiClient::DiscountListDtoCollectionQueryParameters.new # DiscountListDtoCollectionQueryParameters | 
}

begin
  # Retrieves all discount lists
  result = api_instance.get_discount_lists(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->get_discount_lists: #{e}"
end
```

#### Using the get_discount_lists_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<DiscountListDtoListEnvelope>, Integer, Hash)> get_discount_lists_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieves all discount lists
  data, status_code, headers = api_instance.get_discount_lists_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <DiscountListDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->get_discount_lists_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **discount_list_dto_collection_query_parameters** | [**DiscountListDtoCollectionQueryParameters**](DiscountListDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**DiscountListDtoListEnvelope**](DiscountListDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_discount_lists_count

> <Int32Envelope> get_discount_lists_count(tenant_id, opts)

Counts discount lists

Gets the count of discount lists for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DiscountListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  discount_list_dto_collection_query_parameters: OpenapiClient::DiscountListDtoCollectionQueryParameters.new # DiscountListDtoCollectionQueryParameters | 
}

begin
  # Counts discount lists
  result = api_instance.get_discount_lists_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->get_discount_lists_count: #{e}"
end
```

#### Using the get_discount_lists_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_discount_lists_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Counts discount lists
  data, status_code, headers = api_instance.get_discount_lists_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->get_discount_lists_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **discount_list_dto_collection_query_parameters** | [**DiscountListDtoCollectionQueryParameters**](DiscountListDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_discount_list

> <EmptyEnvelope> patch_discount_list(tenant_id, discount_list_id, opts)

Patches a discount list

Partially updates the specified discount list using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DiscountListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
discount_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patches a discount list
  result = api_instance.patch_discount_list(tenant_id, discount_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->patch_discount_list: #{e}"
end
```

#### Using the patch_discount_list_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_discount_list_with_http_info(tenant_id, discount_list_id, opts)

```ruby
begin
  # Patches a discount list
  data, status_code, headers = api_instance.patch_discount_list_with_http_info(tenant_id, discount_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->patch_discount_list_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **discount_list_id** | **String** |  |  |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_discount_list_entry

> <EmptyEnvelope> patch_discount_list_entry(tenant_id, discount_list_id, discount_list_entry_id, opts)

Patches a discount list entry

Partially updates the specified discount entry using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DiscountListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
discount_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
discount_list_entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patches a discount list entry
  result = api_instance.patch_discount_list_entry(tenant_id, discount_list_id, discount_list_entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->patch_discount_list_entry: #{e}"
end
```

#### Using the patch_discount_list_entry_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_discount_list_entry_with_http_info(tenant_id, discount_list_id, discount_list_entry_id, opts)

```ruby
begin
  # Patches a discount list entry
  data, status_code, headers = api_instance.patch_discount_list_entry_with_http_info(tenant_id, discount_list_id, discount_list_entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->patch_discount_list_entry_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **discount_list_id** | **String** |  |  |
| **discount_list_entry_id** | **String** |  |  |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_discount_list

> <EmptyEnvelope> update_discount_list(tenant_id, discount_list_id, opts)

Updates a discount list

Updates the specified discount list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DiscountListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
discount_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  discount_list_update_dto: OpenapiClient::DiscountListUpdateDto.new # DiscountListUpdateDto | 
}

begin
  # Updates a discount list
  result = api_instance.update_discount_list(tenant_id, discount_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->update_discount_list: #{e}"
end
```

#### Using the update_discount_list_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_discount_list_with_http_info(tenant_id, discount_list_id, opts)

```ruby
begin
  # Updates a discount list
  data, status_code, headers = api_instance.update_discount_list_with_http_info(tenant_id, discount_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->update_discount_list_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **discount_list_id** | **String** |  |  |
| **discount_list_update_dto** | [**DiscountListUpdateDto**](DiscountListUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_discount_list_entry

> <EmptyEnvelope> update_discount_list_entry(tenant_id, discount_list_id, discount_list_entry_id, opts)

Updates a discount list entry

Updates the specified discount entry in a discount list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DiscountListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
discount_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
discount_list_entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  discount_update_dto: OpenapiClient::DiscountUpdateDto.new # DiscountUpdateDto | 
}

begin
  # Updates a discount list entry
  result = api_instance.update_discount_list_entry(tenant_id, discount_list_id, discount_list_entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->update_discount_list_entry: #{e}"
end
```

#### Using the update_discount_list_entry_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_discount_list_entry_with_http_info(tenant_id, discount_list_id, discount_list_entry_id, opts)

```ruby
begin
  # Updates a discount list entry
  data, status_code, headers = api_instance.update_discount_list_entry_with_http_info(tenant_id, discount_list_id, discount_list_entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DiscountListsApi->update_discount_list_entry_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **discount_list_id** | **String** |  |  |
| **discount_list_entry_id** | **String** |  |  |
| **discount_update_dto** | [**DiscountUpdateDto**](DiscountUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

