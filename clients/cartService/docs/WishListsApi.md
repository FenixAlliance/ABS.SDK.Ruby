# OpenapiClient::WishListsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**add_product_to_wish_list**](WishListsApi.md#add_product_to_wish_list) | **POST** /api/v2/CartService/WishLists/Records | Add a product to a wish list |
| [**create_wish_list**](WishListsApi.md#create_wish_list) | **POST** /api/v2/CartService/WishLists | Create a wish list |
| [**delete_wish_list**](WishListsApi.md#delete_wish_list) | **DELETE** /api/v2/CartService/WishLists/{wishListId} | Delete a wish list |
| [**delete_wish_list_record**](WishListsApi.md#delete_wish_list_record) | **DELETE** /api/v2/CartService/WishLists/Records/{recordId} | Delete a wish list record |
| [**get_cart_wish_list_details_async**](WishListsApi.md#get_cart_wish_list_details_async) | **GET** /api/v2/CartService/WishLists/{wishListId}/Details | Get wish list details |
| [**get_cart_wish_list_items_async**](WishListsApi.md#get_cart_wish_list_items_async) | **GET** /api/v2/CartService/WishLists/{wishListId}/Records | Get wish list item records |
| [**get_wish_list_async**](WishListsApi.md#get_wish_list_async) | **GET** /api/v2/CartService/WishLists/{cartId} | Get wish lists for a cart |
| [**is_product_in_wish_lists**](WishListsApi.md#is_product_in_wish_lists) | **GET** /api/v2/CartService/WishLists/Contains | Check if a product is in any wish list |
| [**update_product_to_wish_list**](WishListsApi.md#update_product_to_wish_list) | **PUT** /api/v2/CartService/WishLists/{wishListId} | Update a wish list |
| [**wish_list_exists**](WishListsApi.md#wish_list_exists) | **GET** /api/v2/CartService/WishLists/Exists | Check if a wish list exists |
| [**wish_list_exists_head_async**](WishListsApi.md#wish_list_exists_head_async) | **HEAD** /api/v2/CartService/WishLists/Exists | Check if a wish list exists (HEAD) |


## add_product_to_wish_list

> <EmptyEnvelope> add_product_to_wish_list(opts)

Add a product to a wish list

Adds the specified product to the given wish list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WishListsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  product_to_wish_list_request: OpenapiClient::ProductToWishListRequest.new # ProductToWishListRequest | 
}

begin
  # Add a product to a wish list
  result = api_instance.add_product_to_wish_list(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->add_product_to_wish_list: #{e}"
end
```

#### Using the add_product_to_wish_list_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> add_product_to_wish_list_with_http_info(opts)

```ruby
begin
  # Add a product to a wish list
  data, status_code, headers = api_instance.add_product_to_wish_list_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->add_product_to_wish_list_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **product_to_wish_list_request** | [**ProductToWishListRequest**](ProductToWishListRequest.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_wish_list

> <EmptyEnvelope> create_wish_list(opts)

Create a wish list

Creates a new wish list from the provided request data.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WishListsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  new_wish_list_request: OpenapiClient::NewWishListRequest.new # NewWishListRequest | 
}

begin
  # Create a wish list
  result = api_instance.create_wish_list(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->create_wish_list: #{e}"
end
```

#### Using the create_wish_list_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_wish_list_with_http_info(opts)

```ruby
begin
  # Create a wish list
  data, status_code, headers = api_instance.create_wish_list_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->create_wish_list_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **new_wish_list_request** | [**NewWishListRequest**](NewWishListRequest.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_wish_list

> <EmptyEnvelope> delete_wish_list(wish_list_id, opts)

Delete a wish list

Deletes the specified wish list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WishListsApi.new
wish_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a wish list
  result = api_instance.delete_wish_list(wish_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->delete_wish_list: #{e}"
end
```

#### Using the delete_wish_list_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_wish_list_with_http_info(wish_list_id, opts)

```ruby
begin
  # Delete a wish list
  data, status_code, headers = api_instance.delete_wish_list_with_http_info(wish_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->delete_wish_list_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wish_list_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_wish_list_record

> delete_wish_list_record(record_id, opts)

Delete a wish list record

Removes a specific item record from a wish list by its record ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WishListsApi.new
record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a wish list record
  api_instance.delete_wish_list_record(record_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->delete_wish_list_record: #{e}"
end
```

#### Using the delete_wish_list_record_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_wish_list_record_with_http_info(record_id, opts)

```ruby
begin
  # Delete a wish list record
  data, status_code, headers = api_instance.delete_wish_list_record_with_http_info(record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->delete_wish_list_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **record_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## get_cart_wish_list_details_async

> <WishListDto> get_cart_wish_list_details_async(wish_list_id, opts)

Get wish list details

Retrieves the full details of the specified wish list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WishListsApi.new
wish_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get wish list details
  result = api_instance.get_cart_wish_list_details_async(wish_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->get_cart_wish_list_details_async: #{e}"
end
```

#### Using the get_cart_wish_list_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WishListDto>, Integer, Hash)> get_cart_wish_list_details_async_with_http_info(wish_list_id, opts)

```ruby
begin
  # Get wish list details
  data, status_code, headers = api_instance.get_cart_wish_list_details_async_with_http_info(wish_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WishListDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->get_cart_wish_list_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wish_list_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WishListDto**](WishListDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cart_wish_list_items_async

> <Array<WishListItemRecordDto>> get_cart_wish_list_items_async(wish_list_id, opts)

Get wish list item records

Retrieves all item records in the specified wish list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WishListsApi.new
wish_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get wish list item records
  result = api_instance.get_cart_wish_list_items_async(wish_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->get_cart_wish_list_items_async: #{e}"
end
```

#### Using the get_cart_wish_list_items_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<WishListItemRecordDto>>, Integer, Hash)> get_cart_wish_list_items_async_with_http_info(wish_list_id, opts)

```ruby
begin
  # Get wish list item records
  data, status_code, headers = api_instance.get_cart_wish_list_items_async_with_http_info(wish_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<WishListItemRecordDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->get_cart_wish_list_items_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wish_list_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;WishListItemRecordDto&gt;**](WishListItemRecordDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_wish_list_async

> <Array<WishListDto>> get_wish_list_async(cart_id, opts)

Get wish lists for a cart

Retrieves all wish lists associated with the specified cart.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WishListsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get wish lists for a cart
  result = api_instance.get_wish_list_async(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->get_wish_list_async: #{e}"
end
```

#### Using the get_wish_list_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<WishListDto>>, Integer, Hash)> get_wish_list_async_with_http_info(cart_id, opts)

```ruby
begin
  # Get wish lists for a cart
  data, status_code, headers = api_instance.get_wish_list_async_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<WishListDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->get_wish_list_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;WishListDto&gt;**](WishListDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## is_product_in_wish_lists

> <BooleanEnvelope> is_product_in_wish_lists(opts)

Check if a product is in any wish list

Returns a boolean indicating whether the specified product exists in any wish list of the given cart.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WishListsApi.new
opts = {
  cart_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  product_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Check if a product is in any wish list
  result = api_instance.is_product_in_wish_lists(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->is_product_in_wish_lists: #{e}"
end
```

#### Using the is_product_in_wish_lists_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BooleanEnvelope>, Integer, Hash)> is_product_in_wish_lists_with_http_info(opts)

```ruby
begin
  # Check if a product is in any wish list
  data, status_code, headers = api_instance.is_product_in_wish_lists_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BooleanEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->is_product_in_wish_lists_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  | [optional] |
| **product_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_product_to_wish_list

> <EmptyEnvelope> update_product_to_wish_list(wish_list_id, opts)

Update a wish list

Updates the specified wish list with the provided data.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WishListsApi.new
wish_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  wish_list_update_dto: OpenapiClient::WishListUpdateDto.new({title: 'title_example'}) # WishListUpdateDto | 
}

begin
  # Update a wish list
  result = api_instance.update_product_to_wish_list(wish_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->update_product_to_wish_list: #{e}"
end
```

#### Using the update_product_to_wish_list_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_product_to_wish_list_with_http_info(wish_list_id, opts)

```ruby
begin
  # Update a wish list
  data, status_code, headers = api_instance.update_product_to_wish_list_with_http_info(wish_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->update_product_to_wish_list_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wish_list_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **wish_list_update_dto** | [**WishListUpdateDto**](WishListUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## wish_list_exists

> <BooleanEnvelope> wish_list_exists(opts)

Check if a wish list exists

Returns a boolean indicating whether the specified wish list exists.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WishListsApi.new
opts = {
  wish_list_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Check if a wish list exists
  result = api_instance.wish_list_exists(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->wish_list_exists: #{e}"
end
```

#### Using the wish_list_exists_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BooleanEnvelope>, Integer, Hash)> wish_list_exists_with_http_info(opts)

```ruby
begin
  # Check if a wish list exists
  data, status_code, headers = api_instance.wish_list_exists_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BooleanEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->wish_list_exists_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wish_list_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## wish_list_exists_head_async

> <EmptyEnvelope> wish_list_exists_head_async(opts)

Check if a wish list exists (HEAD)

HEAD request to check whether the specified wish list exists without returning a response body.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WishListsApi.new
opts = {
  wish_list_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Check if a wish list exists (HEAD)
  result = api_instance.wish_list_exists_head_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->wish_list_exists_head_async: #{e}"
end
```

#### Using the wish_list_exists_head_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> wish_list_exists_head_async_with_http_info(opts)

```ruby
begin
  # Check if a wish list exists (HEAD)
  data, status_code, headers = api_instance.wish_list_exists_head_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WishListsApi->wish_list_exists_head_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wish_list_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

