# OpenapiClient::MarketingListsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_marketing_list_async**](MarketingListsApi.md#create_marketing_list_async) | **POST** /api/v2/MarketingService/MarketingLists | Create a marketing list |
| [**delete_marketing_list_async**](MarketingListsApi.md#delete_marketing_list_async) | **DELETE** /api/v2/MarketingService/MarketingLists/{marketinglistId} | Delete a marketing list |
| [**get_marketing_list_details_async**](MarketingListsApi.md#get_marketing_list_details_async) | **GET** /api/v2/MarketingService/MarketingLists/{marketinglistId} | Get marketing list by ID |
| [**get_marketing_list_o_data_async**](MarketingListsApi.md#get_marketing_list_o_data_async) | **GET** /api/v2/MarketingService/MarketingLists | Get marketing lists |
| [**get_marketing_lists_count_async**](MarketingListsApi.md#get_marketing_lists_count_async) | **GET** /api/v2/MarketingService/MarketingLists/Count | Get marketing lists count |
| [**update_marketing_list_async**](MarketingListsApi.md#update_marketing_list_async) | **PUT** /api/v2/MarketingService/MarketingLists/{marketinglistId} | Update a marketing list |


## create_marketing_list_async

> <EmptyEnvelope> create_marketing_list_async(tenant_id, marketing_list_create_dto, opts)

Create a marketing list

Creates a new marketing list for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
marketing_list_create_dto = OpenapiClient::MarketingListCreateDto.new # MarketingListCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a marketing list
  result = api_instance.create_marketing_list_async(tenant_id, marketing_list_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingListsApi->create_marketing_list_async: #{e}"
end
```

#### Using the create_marketing_list_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_marketing_list_async_with_http_info(tenant_id, marketing_list_create_dto, opts)

```ruby
begin
  # Create a marketing list
  data, status_code, headers = api_instance.create_marketing_list_async_with_http_info(tenant_id, marketing_list_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingListsApi->create_marketing_list_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **marketing_list_create_dto** | [**MarketingListCreateDto**](MarketingListCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_marketing_list_async

> <EmptyEnvelope> delete_marketing_list_async(tenant_id, marketinglist_id, opts)

Delete a marketing list

Deletes a marketing list by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
marketinglist_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a marketing list
  result = api_instance.delete_marketing_list_async(tenant_id, marketinglist_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingListsApi->delete_marketing_list_async: #{e}"
end
```

#### Using the delete_marketing_list_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_marketing_list_async_with_http_info(tenant_id, marketinglist_id, opts)

```ruby
begin
  # Delete a marketing list
  data, status_code, headers = api_instance.delete_marketing_list_async_with_http_info(tenant_id, marketinglist_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingListsApi->delete_marketing_list_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **marketinglist_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_marketing_list_details_async

> <MarketingListDtoEnvelope> get_marketing_list_details_async(tenant_id, marketinglist_id, opts)

Get marketing list by ID

Retrieves the details of a specific marketing list by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
marketinglist_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get marketing list by ID
  result = api_instance.get_marketing_list_details_async(tenant_id, marketinglist_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingListsApi->get_marketing_list_details_async: #{e}"
end
```

#### Using the get_marketing_list_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MarketingListDtoEnvelope>, Integer, Hash)> get_marketing_list_details_async_with_http_info(tenant_id, marketinglist_id, opts)

```ruby
begin
  # Get marketing list by ID
  data, status_code, headers = api_instance.get_marketing_list_details_async_with_http_info(tenant_id, marketinglist_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MarketingListDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingListsApi->get_marketing_list_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **marketinglist_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MarketingListDtoEnvelope**](MarketingListDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_marketing_list_o_data_async

> <MarketingListDtoListEnvelope> get_marketing_list_o_data_async(tenant_id, opts)

Get marketing lists

Retrieves a collection of marketing lists for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get marketing lists
  result = api_instance.get_marketing_list_o_data_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingListsApi->get_marketing_list_o_data_async: #{e}"
end
```

#### Using the get_marketing_list_o_data_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MarketingListDtoListEnvelope>, Integer, Hash)> get_marketing_list_o_data_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get marketing lists
  data, status_code, headers = api_instance.get_marketing_list_o_data_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MarketingListDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingListsApi->get_marketing_list_o_data_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MarketingListDtoListEnvelope**](MarketingListDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_marketing_lists_count_async

> <Int32Envelope> get_marketing_lists_count_async(tenant_id, opts)

Get marketing lists count

Returns the count of marketing lists for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get marketing lists count
  result = api_instance.get_marketing_lists_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingListsApi->get_marketing_lists_count_async: #{e}"
end
```

#### Using the get_marketing_lists_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_marketing_lists_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get marketing lists count
  data, status_code, headers = api_instance.get_marketing_lists_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingListsApi->get_marketing_lists_count_async_with_http_info: #{e}"
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


## update_marketing_list_async

> <EmptyEnvelope> update_marketing_list_async(tenant_id, marketinglist_id, marketing_list_update_dto, opts)

Update a marketing list

Updates an existing marketing list by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
marketinglist_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
marketing_list_update_dto = OpenapiClient::MarketingListUpdateDto.new # MarketingListUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update a marketing list
  result = api_instance.update_marketing_list_async(tenant_id, marketinglist_id, marketing_list_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingListsApi->update_marketing_list_async: #{e}"
end
```

#### Using the update_marketing_list_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_marketing_list_async_with_http_info(tenant_id, marketinglist_id, marketing_list_update_dto, opts)

```ruby
begin
  # Update a marketing list
  data, status_code, headers = api_instance.update_marketing_list_async_with_http_info(tenant_id, marketinglist_id, marketing_list_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingListsApi->update_marketing_list_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **marketinglist_id** | **String** |  |  |
| **marketing_list_update_dto** | [**MarketingListUpdateDto**](MarketingListUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

