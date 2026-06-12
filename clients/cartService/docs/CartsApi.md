# OpenapiClient::CartsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**add_item_to_cart_async**](CartsApi.md#add_item_to_cart_async) | **POST** /api/v2/CartService/Carts/{cartId}/Items/{itemId} | Add an Item to a cart |
| [**add_item_to_cart_compare_table**](CartsApi.md#add_item_to_cart_compare_table) | **POST** /api/v2/CartService/Carts/{cartId}/Compare/{itemId} | Add an item to the compare table |
| [**add_item_to_wish_list**](CartsApi.md#add_item_to_wish_list) | **POST** /api/v2/CartService/Carts/{cartId}/WishLists/{wishListId}/Records | Add a record to a wish list |
| [**cart_wish_list_exists_head**](CartsApi.md#cart_wish_list_exists_head) | **HEAD** /api/v2/CartService/Carts/{cartId}/WishLists/{wishListId}/Exists | Assesses if a WishList exists |
| [**clear_cart_records**](CartsApi.md#clear_cart_records) | **DELETE** /api/v2/CartService/Carts/{cartId}/Items | Clear all items from a cart |
| [**create_wish_list_async**](CartsApi.md#create_wish_list_async) | **POST** /api/v2/CartService/Carts/{cartId}/WishLists | Create a new wish list |
| [**decrease_cart_item_quantity**](CartsApi.md#decrease_cart_item_quantity) | **PUT** /api/v2/CartService/Carts/{cartId}/Items/{itemId}/Decrease | Decrease an Item in a cart |
| [**decrease_cart_line_async**](CartsApi.md#decrease_cart_line_async) | **PUT** /api/v2/CartService/Carts/{cartId}/Lines/{lineId}/Decrease | Decrease the quantity of a cart line |
| [**delete_cart_wish_list**](CartsApi.md#delete_cart_wish_list) | **DELETE** /api/v2/CartService/Carts/{cartId}/WishLists/{wishListId} | Delete a wish list |
| [**delete_cart_wish_list_record**](CartsApi.md#delete_cart_wish_list_record) | **DELETE** /api/v2/CartService/Carts/{cartId}/WishLists/{wishListId}/Records/{recordId} | Remove a record from a wish list |
| [**get_acting_cart**](CartsApi.md#get_acting_cart) | **GET** /api/v2/CartService/Carts/ActingCart | Get the acting cart |
| [**get_cart_by_id_async**](CartsApi.md#get_cart_by_id_async) | **GET** /api/v2/CartService/Carts/{cartId} | Get all business owned contacts |
| [**get_cart_compare_record**](CartsApi.md#get_cart_compare_record) | **GET** /api/v2/CartService/Carts/{cartId}/Compare/{itemId} | Get an item from the compare table |
| [**get_cart_compare_records**](CartsApi.md#get_cart_compare_records) | **GET** /api/v2/CartService/Carts/{cartId}/Compare | Get all items in the compare table |
| [**get_cart_country_async**](CartsApi.md#get_cart_country_async) | **GET** /api/v2/CartService/Carts/{cartId}/Country | Get the country of a cart |
| [**get_cart_currency_async**](CartsApi.md#get_cart_currency_async) | **GET** /api/v2/CartService/Carts/{cartId}/Currency | Get the currency of a cart |
| [**get_cart_items**](CartsApi.md#get_cart_items) | **GET** /api/v2/CartService/Carts/{cartId}/Items | Get all cart lines |
| [**get_cart_line_async**](CartsApi.md#get_cart_line_async) | **GET** /api/v2/CartService/Carts/{cartId}/Lines/{lineId} | Get a cart line by ID |
| [**get_cart_lines_async**](CartsApi.md#get_cart_lines_async) | **GET** /api/v2/CartService/Carts/{cartId}/Lines | Get all cart lines |
| [**get_cart_wish_list**](CartsApi.md#get_cart_wish_list) | **GET** /api/v2/CartService/Carts/{cartId}/WishLists | Get all wishlists in a cart |
| [**get_cart_wish_list_details**](CartsApi.md#get_cart_wish_list_details) | **GET** /api/v2/CartService/Carts/{cartId}/WishLists/{wishListId} | Get a wish list by ID |
| [**get_cart_wish_list_item_async**](CartsApi.md#get_cart_wish_list_item_async) | **GET** /api/v2/CartService/Carts/{cartId}/WishLists/{wishListId}/Records/{recordId} | Get a record in a wish list |
| [**get_cart_wish_list_items**](CartsApi.md#get_cart_wish_list_items) | **GET** /api/v2/CartService/Carts/{cartId}/WishLists/{wishListId}/Records | Get all records in a wish list |
| [**get_guest_cart_async**](CartsApi.md#get_guest_cart_async) | **GET** /api/v2/CartService/Carts/GuestCart | Get the guest cart |
| [**get_tenant_cart_async**](CartsApi.md#get_tenant_cart_async) | **GET** /api/v2/CartService/Carts/BusinessCart/{tenantId} | Get the business cart |
| [**get_user_cart**](CartsApi.md#get_user_cart) | **GET** /api/v2/CartService/Carts/UserCart | Get the current user&#39;s cart |
| [**increase_cart_line_async**](CartsApi.md#increase_cart_line_async) | **PUT** /api/v2/CartService/Carts/{cartId}/Lines/{lineId}/Increase | Increase the quantity of a cart line |
| [**increase_item_cart_record_quantity_async**](CartsApi.md#increase_item_cart_record_quantity_async) | **PUT** /api/v2/CartService/Carts/{cartId}/Items/{itemId}/Increase | Increase an Item in a cart |
| [**is_item_already_in_cart_async**](CartsApi.md#is_item_already_in_cart_async) | **GET** /api/v2/CartService/Carts/{cartId}/Contains/{itemId} | Assesses if an Item is already in a cart |
| [**is_item_in_compare_table_async**](CartsApi.md#is_item_in_compare_table_async) | **GET** /api/v2/CartService/Carts/{cartId}/Compare/Contains/{itemId} | Assesses if an Item is already in the compare table |
| [**is_item_in_wish_lists**](CartsApi.md#is_item_in_wish_lists) | **GET** /api/v2/CartService/Carts/{cartId}/WishLists/Contains/{itemId} | Assesses if an Item is already in any of the cart&#39;s wishlists |
| [**patch_cart_async**](CartsApi.md#patch_cart_async) | **PATCH** /api/v2/CartService/Carts/{cartId} | Patch a cart |
| [**remove_cart_line_async**](CartsApi.md#remove_cart_line_async) | **DELETE** /api/v2/CartService/Carts/{cartId}/Lines/{lineId} | Remove a cart line |
| [**remove_item_from_cart_async**](CartsApi.md#remove_item_from_cart_async) | **DELETE** /api/v2/CartService/Carts/{cartId}/Items/{itemId} | Remove an Item from a cart |
| [**remove_item_from_compare_table_async**](CartsApi.md#remove_item_from_compare_table_async) | **DELETE** /api/v2/CartService/Carts/{cartId}/Compare/{itemId} | Remove an item from the compare table |
| [**set_cart_country_async**](CartsApi.md#set_cart_country_async) | **PUT** /api/v2/CartService/Carts/{cartId}/Country | Set the country of a cart |
| [**set_cart_currency_async**](CartsApi.md#set_cart_currency_async) | **PUT** /api/v2/CartService/Carts/{cartId}/Currency | Set the currency of a cart |
| [**submit_cart_async**](CartsApi.md#submit_cart_async) | **POST** /api/v2/CartService/Carts/{cartId}/Submit | Submit a cart for processing |
| [**update_cart_async**](CartsApi.md#update_cart_async) | **PUT** /api/v2/CartService/Carts/{cartId} | Update a cart |
| [**update_cart_line_async**](CartsApi.md#update_cart_line_async) | **PUT** /api/v2/CartService/Carts/{cartId}/Lines/{lineId} | Update a cart line |
| [**update_item_cart_record_async**](CartsApi.md#update_item_cart_record_async) | **PUT** /api/v2/CartService/Carts/{cartId}/Items/{itemId} | Update an Item in a cart |
| [**update_item_to_wish_list**](CartsApi.md#update_item_to_wish_list) | **PUT** /api/v2/CartService/Carts/{cartId}/WishLists/{wishListId} | Update a wish list |
| [**wish_list_exists_async**](CartsApi.md#wish_list_exists_async) | **GET** /api/v2/CartService/Carts/{cartId}/WishLists/{wishListId}/Exists | Assesses if a WishList exists |


## add_item_to_cart_async

> <EmptyEnvelope> add_item_to_cart_async(cart_id, item_id, opts)

Add an Item to a cart

Add an Item to a cart

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  quantity: 56, # Integer | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Add an Item to a cart
  result = api_instance.add_item_to_cart_async(cart_id, item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->add_item_to_cart_async: #{e}"
end
```

#### Using the add_item_to_cart_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> add_item_to_cart_async_with_http_info(cart_id, item_id, opts)

```ruby
begin
  # Add an Item to a cart
  data, status_code, headers = api_instance.add_item_to_cart_async_with_http_info(cart_id, item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->add_item_to_cart_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **quantity** | **Integer** |  | [optional][default to 1] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## add_item_to_cart_compare_table

> <ItemCartRecordDto> add_item_to_cart_compare_table(cart_id, item_id, opts)

Add an item to the compare table

Add an item to the compare table

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Add an item to the compare table
  result = api_instance.add_item_to_cart_compare_table(cart_id, item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->add_item_to_cart_compare_table: #{e}"
end
```

#### Using the add_item_to_cart_compare_table_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemCartRecordDto>, Integer, Hash)> add_item_to_cart_compare_table_with_http_info(cart_id, item_id, opts)

```ruby
begin
  # Add an item to the compare table
  data, status_code, headers = api_instance.add_item_to_cart_compare_table_with_http_info(cart_id, item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemCartRecordDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->add_item_to_cart_compare_table_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemCartRecordDto**](ItemCartRecordDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## add_item_to_wish_list

> <EmptyEnvelope> add_item_to_wish_list(cart_id, wish_list_id, opts)

Add a record to a wish list

Add a record to a wish list

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
wish_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  product_to_wish_list_request: OpenapiClient::ProductToWishListRequest.new # ProductToWishListRequest | 
}

begin
  # Add a record to a wish list
  result = api_instance.add_item_to_wish_list(cart_id, wish_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->add_item_to_wish_list: #{e}"
end
```

#### Using the add_item_to_wish_list_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> add_item_to_wish_list_with_http_info(cart_id, wish_list_id, opts)

```ruby
begin
  # Add a record to a wish list
  data, status_code, headers = api_instance.add_item_to_wish_list_with_http_info(cart_id, wish_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->add_item_to_wish_list_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **wish_list_id** | **String** |  |  |
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


## cart_wish_list_exists_head

> <EmptyEnvelope> cart_wish_list_exists_head(cart_id, wish_list_id, opts)

Assesses if a WishList exists

Assesses if a WishList exists but does not return the content

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
wish_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Assesses if a WishList exists
  result = api_instance.cart_wish_list_exists_head(cart_id, wish_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->cart_wish_list_exists_head: #{e}"
end
```

#### Using the cart_wish_list_exists_head_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> cart_wish_list_exists_head_with_http_info(cart_id, wish_list_id, opts)

```ruby
begin
  # Assesses if a WishList exists
  data, status_code, headers = api_instance.cart_wish_list_exists_head_with_http_info(cart_id, wish_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->cart_wish_list_exists_head_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
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


## clear_cart_records

> <EmptyEnvelope> clear_cart_records(cart_id, opts)

Clear all items from a cart

Clear all items from a cart

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Clear all items from a cart
  result = api_instance.clear_cart_records(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->clear_cart_records: #{e}"
end
```

#### Using the clear_cart_records_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> clear_cart_records_with_http_info(cart_id, opts)

```ruby
begin
  # Clear all items from a cart
  data, status_code, headers = api_instance.clear_cart_records_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->clear_cart_records_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_wish_list_async

> <EmptyEnvelope> create_wish_list_async(cart_id, opts)

Create a new wish list

Create a new wish list

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  new_wish_list_request: OpenapiClient::NewWishListRequest.new # NewWishListRequest | 
}

begin
  # Create a new wish list
  result = api_instance.create_wish_list_async(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->create_wish_list_async: #{e}"
end
```

#### Using the create_wish_list_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_wish_list_async_with_http_info(cart_id, opts)

```ruby
begin
  # Create a new wish list
  data, status_code, headers = api_instance.create_wish_list_async_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->create_wish_list_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
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


## decrease_cart_item_quantity

> <EmptyEnvelope> decrease_cart_item_quantity(cart_id, item_id, opts)

Decrease an Item in a cart

Decrease an Item in a cart

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_cart_record_update_dto: OpenapiClient::ItemCartRecordUpdateDto.new # ItemCartRecordUpdateDto | 
}

begin
  # Decrease an Item in a cart
  result = api_instance.decrease_cart_item_quantity(cart_id, item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->decrease_cart_item_quantity: #{e}"
end
```

#### Using the decrease_cart_item_quantity_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> decrease_cart_item_quantity_with_http_info(cart_id, item_id, opts)

```ruby
begin
  # Decrease an Item in a cart
  data, status_code, headers = api_instance.decrease_cart_item_quantity_with_http_info(cart_id, item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->decrease_cart_item_quantity_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_cart_record_update_dto** | [**ItemCartRecordUpdateDto**](ItemCartRecordUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## decrease_cart_line_async

> <EmptyEnvelope> decrease_cart_line_async(cart_id, line_id, opts)

Decrease the quantity of a cart line

Decrease the quantity of a cart line

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  quantity: 1.2, # Float | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Decrease the quantity of a cart line
  result = api_instance.decrease_cart_line_async(cart_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->decrease_cart_line_async: #{e}"
end
```

#### Using the decrease_cart_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> decrease_cart_line_async_with_http_info(cart_id, line_id, opts)

```ruby
begin
  # Decrease the quantity of a cart line
  data, status_code, headers = api_instance.decrease_cart_line_async_with_http_info(cart_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->decrease_cart_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **line_id** | **String** |  |  |
| **quantity** | **Float** |  | [optional][default to 1] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_cart_wish_list

> <EmptyEnvelope> delete_cart_wish_list(cart_id, wish_list_id, opts)

Delete a wish list

Delete a wish list

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
wish_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a wish list
  result = api_instance.delete_cart_wish_list(cart_id, wish_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->delete_cart_wish_list: #{e}"
end
```

#### Using the delete_cart_wish_list_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_cart_wish_list_with_http_info(cart_id, wish_list_id, opts)

```ruby
begin
  # Delete a wish list
  data, status_code, headers = api_instance.delete_cart_wish_list_with_http_info(cart_id, wish_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->delete_cart_wish_list_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
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


## delete_cart_wish_list_record

> <EmptyEnvelope> delete_cart_wish_list_record(cart_id, wish_list_id, record_id, opts)

Remove a record from a wish list

Remove a record from a wish list

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
wish_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove a record from a wish list
  result = api_instance.delete_cart_wish_list_record(cart_id, wish_list_id, record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->delete_cart_wish_list_record: #{e}"
end
```

#### Using the delete_cart_wish_list_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_cart_wish_list_record_with_http_info(cart_id, wish_list_id, record_id, opts)

```ruby
begin
  # Remove a record from a wish list
  data, status_code, headers = api_instance.delete_cart_wish_list_record_with_http_info(cart_id, wish_list_id, record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->delete_cart_wish_list_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **wish_list_id** | **String** |  |  |
| **record_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_acting_cart

> <CartDtoEnvelope> get_acting_cart(opts)

Get the acting cart

Get the acting cart

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the acting cart
  result = api_instance.get_acting_cart(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_acting_cart: #{e}"
end
```

#### Using the get_acting_cart_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CartDtoEnvelope>, Integer, Hash)> get_acting_cart_with_http_info(opts)

```ruby
begin
  # Get the acting cart
  data, status_code, headers = api_instance.get_acting_cart_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CartDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_acting_cart_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CartDtoEnvelope**](CartDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cart_by_id_async

> <CartDtoEnvelope> get_cart_by_id_async(cart_id, opts)

Get all business owned contacts

Get all business owned contacts

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all business owned contacts
  result = api_instance.get_cart_by_id_async(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_by_id_async: #{e}"
end
```

#### Using the get_cart_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CartDtoEnvelope>, Integer, Hash)> get_cart_by_id_async_with_http_info(cart_id, opts)

```ruby
begin
  # Get all business owned contacts
  data, status_code, headers = api_instance.get_cart_by_id_async_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CartDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CartDtoEnvelope**](CartDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cart_compare_record

> <ItemToCompareCartRecordDtoEnvelope> get_cart_compare_record(cart_id, item_id, opts)

Get an item from the compare table

Get an item from the compare table

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get an item from the compare table
  result = api_instance.get_cart_compare_record(cart_id, item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_compare_record: #{e}"
end
```

#### Using the get_cart_compare_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemToCompareCartRecordDtoEnvelope>, Integer, Hash)> get_cart_compare_record_with_http_info(cart_id, item_id, opts)

```ruby
begin
  # Get an item from the compare table
  data, status_code, headers = api_instance.get_cart_compare_record_with_http_info(cart_id, item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemToCompareCartRecordDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_compare_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemToCompareCartRecordDtoEnvelope**](ItemToCompareCartRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cart_compare_records

> <ItemToCompareCartRecordDtoListEnvelope> get_cart_compare_records(cart_id, opts)

Get all items in the compare table

Get all items in the compare table

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all items in the compare table
  result = api_instance.get_cart_compare_records(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_compare_records: #{e}"
end
```

#### Using the get_cart_compare_records_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemToCompareCartRecordDtoListEnvelope>, Integer, Hash)> get_cart_compare_records_with_http_info(cart_id, opts)

```ruby
begin
  # Get all items in the compare table
  data, status_code, headers = api_instance.get_cart_compare_records_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemToCompareCartRecordDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_compare_records_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemToCompareCartRecordDtoListEnvelope**](ItemToCompareCartRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cart_country_async

> <CountryDtoEnvelope> get_cart_country_async(cart_id, opts)

Get the country of a cart

The country of a cart is used to calculate taxes and shipping costs

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the country of a cart
  result = api_instance.get_cart_country_async(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_country_async: #{e}"
end
```

#### Using the get_cart_country_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CountryDtoEnvelope>, Integer, Hash)> get_cart_country_async_with_http_info(cart_id, opts)

```ruby
begin
  # Get the country of a cart
  data, status_code, headers = api_instance.get_cart_country_async_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CountryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_country_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CountryDtoEnvelope**](CountryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cart_currency_async

> <CurrencyDtoEnvelope> get_cart_currency_async(cart_id, opts)

Get the currency of a cart

The currency of a cart used for display purposes

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the currency of a cart
  result = api_instance.get_cart_currency_async(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_currency_async: #{e}"
end
```

#### Using the get_cart_currency_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CurrencyDtoEnvelope>, Integer, Hash)> get_cart_currency_async_with_http_info(cart_id, opts)

```ruby
begin
  # Get the currency of a cart
  data, status_code, headers = api_instance.get_cart_currency_async_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CurrencyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_currency_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CurrencyDtoEnvelope**](CurrencyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cart_items

> <ItemCartRecordDtoListEnvelope> get_cart_items(cart_id, opts)

Get all cart lines

Get all cart lines

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all cart lines
  result = api_instance.get_cart_items(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_items: #{e}"
end
```

#### Using the get_cart_items_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemCartRecordDtoListEnvelope>, Integer, Hash)> get_cart_items_with_http_info(cart_id, opts)

```ruby
begin
  # Get all cart lines
  data, status_code, headers = api_instance.get_cart_items_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemCartRecordDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_items_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemCartRecordDtoListEnvelope**](ItemCartRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cart_line_async

> <EmptyEnvelope> get_cart_line_async(cart_id, line_id, opts)

Get a cart line by ID

Get a cart line by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a cart line by ID
  result = api_instance.get_cart_line_async(cart_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_line_async: #{e}"
end
```

#### Using the get_cart_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> get_cart_line_async_with_http_info(cart_id, line_id, opts)

```ruby
begin
  # Get a cart line by ID
  data, status_code, headers = api_instance.get_cart_line_async_with_http_info(cart_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **line_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cart_lines_async

> <ItemCartRecordDtoListEnvelope> get_cart_lines_async(cart_id, opts)

Get all cart lines

Get all cart lines

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all cart lines
  result = api_instance.get_cart_lines_async(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_lines_async: #{e}"
end
```

#### Using the get_cart_lines_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemCartRecordDtoListEnvelope>, Integer, Hash)> get_cart_lines_async_with_http_info(cart_id, opts)

```ruby
begin
  # Get all cart lines
  data, status_code, headers = api_instance.get_cart_lines_async_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemCartRecordDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_lines_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemCartRecordDtoListEnvelope**](ItemCartRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cart_wish_list

> <Array<WishListDto>> get_cart_wish_list(cart_id, opts)

Get all wishlists in a cart

Get all wishlists in a cart

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all wishlists in a cart
  result = api_instance.get_cart_wish_list(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_wish_list: #{e}"
end
```

#### Using the get_cart_wish_list_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<WishListDto>>, Integer, Hash)> get_cart_wish_list_with_http_info(cart_id, opts)

```ruby
begin
  # Get all wishlists in a cart
  data, status_code, headers = api_instance.get_cart_wish_list_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<WishListDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_wish_list_with_http_info: #{e}"
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


## get_cart_wish_list_details

> <WishListDtoEnvelope> get_cart_wish_list_details(cart_id, wish_list_id, opts)

Get a wish list by ID

Get a wish list by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
wish_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a wish list by ID
  result = api_instance.get_cart_wish_list_details(cart_id, wish_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_wish_list_details: #{e}"
end
```

#### Using the get_cart_wish_list_details_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WishListDtoEnvelope>, Integer, Hash)> get_cart_wish_list_details_with_http_info(cart_id, wish_list_id, opts)

```ruby
begin
  # Get a wish list by ID
  data, status_code, headers = api_instance.get_cart_wish_list_details_with_http_info(cart_id, wish_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WishListDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_wish_list_details_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **wish_list_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WishListDtoEnvelope**](WishListDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cart_wish_list_item_async

> <Array<WishListItemRecordDto>> get_cart_wish_list_item_async(cart_id, wish_list_id, record_id, opts)

Get a record in a wish list

Get a record in a wish list

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
wish_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a record in a wish list
  result = api_instance.get_cart_wish_list_item_async(cart_id, wish_list_id, record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_wish_list_item_async: #{e}"
end
```

#### Using the get_cart_wish_list_item_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<WishListItemRecordDto>>, Integer, Hash)> get_cart_wish_list_item_async_with_http_info(cart_id, wish_list_id, record_id, opts)

```ruby
begin
  # Get a record in a wish list
  data, status_code, headers = api_instance.get_cart_wish_list_item_async_with_http_info(cart_id, wish_list_id, record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<WishListItemRecordDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_wish_list_item_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **wish_list_id** | **String** |  |  |
| **record_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;WishListItemRecordDto&gt;**](WishListItemRecordDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cart_wish_list_items

> <Array<WishListItemRecordDto>> get_cart_wish_list_items(cart_id, wish_list_id, opts)

Get all records in a wish list

Get all records in a wish list

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
wish_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all records in a wish list
  result = api_instance.get_cart_wish_list_items(cart_id, wish_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_wish_list_items: #{e}"
end
```

#### Using the get_cart_wish_list_items_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<WishListItemRecordDto>>, Integer, Hash)> get_cart_wish_list_items_with_http_info(cart_id, wish_list_id, opts)

```ruby
begin
  # Get all records in a wish list
  data, status_code, headers = api_instance.get_cart_wish_list_items_with_http_info(cart_id, wish_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<WishListItemRecordDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_cart_wish_list_items_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
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


## get_guest_cart_async

> <CartDtoEnvelope> get_guest_cart_async(opts)

Get the guest cart

Get the guest cart

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the guest cart
  result = api_instance.get_guest_cart_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_guest_cart_async: #{e}"
end
```

#### Using the get_guest_cart_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CartDtoEnvelope>, Integer, Hash)> get_guest_cart_async_with_http_info(opts)

```ruby
begin
  # Get the guest cart
  data, status_code, headers = api_instance.get_guest_cart_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CartDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_guest_cart_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CartDtoEnvelope**](CartDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_cart_async

> <CartDtoEnvelope> get_tenant_cart_async(tenant_id, opts)

Get the business cart

Get the business cart

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the business cart
  result = api_instance.get_tenant_cart_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_tenant_cart_async: #{e}"
end
```

#### Using the get_tenant_cart_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CartDtoEnvelope>, Integer, Hash)> get_tenant_cart_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the business cart
  data, status_code, headers = api_instance.get_tenant_cart_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CartDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_tenant_cart_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CartDtoEnvelope**](CartDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_user_cart

> <CartDtoEnvelope> get_user_cart(opts)

Get the current user's cart

Get the current user's cart

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the current user's cart
  result = api_instance.get_user_cart(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_user_cart: #{e}"
end
```

#### Using the get_user_cart_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CartDtoEnvelope>, Integer, Hash)> get_user_cart_with_http_info(opts)

```ruby
begin
  # Get the current user's cart
  data, status_code, headers = api_instance.get_user_cart_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CartDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->get_user_cart_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CartDtoEnvelope**](CartDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## increase_cart_line_async

> <EmptyEnvelope> increase_cart_line_async(cart_id, line_id, opts)

Increase the quantity of a cart line

Increase the quantity of a cart line

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  quantity: 1.2, # Float | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Increase the quantity of a cart line
  result = api_instance.increase_cart_line_async(cart_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->increase_cart_line_async: #{e}"
end
```

#### Using the increase_cart_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> increase_cart_line_async_with_http_info(cart_id, line_id, opts)

```ruby
begin
  # Increase the quantity of a cart line
  data, status_code, headers = api_instance.increase_cart_line_async_with_http_info(cart_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->increase_cart_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **line_id** | **String** |  |  |
| **quantity** | **Float** |  | [optional][default to 1] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## increase_item_cart_record_quantity_async

> <EmptyEnvelope> increase_item_cart_record_quantity_async(cart_id, item_id, opts)

Increase an Item in a cart

Increase an Item in a cart

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_cart_record_update_dto: OpenapiClient::ItemCartRecordUpdateDto.new # ItemCartRecordUpdateDto | 
}

begin
  # Increase an Item in a cart
  result = api_instance.increase_item_cart_record_quantity_async(cart_id, item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->increase_item_cart_record_quantity_async: #{e}"
end
```

#### Using the increase_item_cart_record_quantity_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> increase_item_cart_record_quantity_async_with_http_info(cart_id, item_id, opts)

```ruby
begin
  # Increase an Item in a cart
  data, status_code, headers = api_instance.increase_item_cart_record_quantity_async_with_http_info(cart_id, item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->increase_item_cart_record_quantity_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_cart_record_update_dto** | [**ItemCartRecordUpdateDto**](ItemCartRecordUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## is_item_already_in_cart_async

> <BooleanEnvelope> is_item_already_in_cart_async(cart_id, item_id, opts)

Assesses if an Item is already in a cart

Assesses if an Item is already in a cart

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Assesses if an Item is already in a cart
  result = api_instance.is_item_already_in_cart_async(cart_id, item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->is_item_already_in_cart_async: #{e}"
end
```

#### Using the is_item_already_in_cart_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BooleanEnvelope>, Integer, Hash)> is_item_already_in_cart_async_with_http_info(cart_id, item_id, opts)

```ruby
begin
  # Assesses if an Item is already in a cart
  data, status_code, headers = api_instance.is_item_already_in_cart_async_with_http_info(cart_id, item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BooleanEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->is_item_already_in_cart_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## is_item_in_compare_table_async

> <BooleanEnvelope> is_item_in_compare_table_async(cart_id, item_id, opts)

Assesses if an Item is already in the compare table

Assesses if an Item is already in the compare table

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Assesses if an Item is already in the compare table
  result = api_instance.is_item_in_compare_table_async(cart_id, item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->is_item_in_compare_table_async: #{e}"
end
```

#### Using the is_item_in_compare_table_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BooleanEnvelope>, Integer, Hash)> is_item_in_compare_table_async_with_http_info(cart_id, item_id, opts)

```ruby
begin
  # Assesses if an Item is already in the compare table
  data, status_code, headers = api_instance.is_item_in_compare_table_async_with_http_info(cart_id, item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BooleanEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->is_item_in_compare_table_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## is_item_in_wish_lists

> <BooleanEnvelope> is_item_in_wish_lists(cart_id, item_id, opts)

Assesses if an Item is already in any of the cart's wishlists

Assesses if an Item is already in any of the cart's wishlists

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Assesses if an Item is already in any of the cart's wishlists
  result = api_instance.is_item_in_wish_lists(cart_id, item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->is_item_in_wish_lists: #{e}"
end
```

#### Using the is_item_in_wish_lists_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BooleanEnvelope>, Integer, Hash)> is_item_in_wish_lists_with_http_info(cart_id, item_id, opts)

```ruby
begin
  # Assesses if an Item is already in any of the cart's wishlists
  data, status_code, headers = api_instance.is_item_in_wish_lists_with_http_info(cart_id, item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BooleanEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->is_item_in_wish_lists_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_cart_async

> <EmptyEnvelope> patch_cart_async(cart_id, opts)

Patch a cart

Partially updates a cart using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a cart
  result = api_instance.patch_cart_async(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->patch_cart_async: #{e}"
end
```

#### Using the patch_cart_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_cart_async_with_http_info(cart_id, opts)

```ruby
begin
  # Patch a cart
  data, status_code, headers = api_instance.patch_cart_async_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->patch_cart_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
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


## remove_cart_line_async

> <EmptyEnvelope> remove_cart_line_async(cart_id, line_id, opts)

Remove a cart line

Remove a cart line

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove a cart line
  result = api_instance.remove_cart_line_async(cart_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->remove_cart_line_async: #{e}"
end
```

#### Using the remove_cart_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> remove_cart_line_async_with_http_info(cart_id, line_id, opts)

```ruby
begin
  # Remove a cart line
  data, status_code, headers = api_instance.remove_cart_line_async_with_http_info(cart_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->remove_cart_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **line_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_item_from_cart_async

> <EmptyEnvelope> remove_item_from_cart_async(cart_id, item_id, opts)

Remove an Item from a cart

Remove an Item from a cart

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove an Item from a cart
  result = api_instance.remove_item_from_cart_async(cart_id, item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->remove_item_from_cart_async: #{e}"
end
```

#### Using the remove_item_from_cart_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> remove_item_from_cart_async_with_http_info(cart_id, item_id, opts)

```ruby
begin
  # Remove an Item from a cart
  data, status_code, headers = api_instance.remove_item_from_cart_async_with_http_info(cart_id, item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->remove_item_from_cart_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_item_from_compare_table_async

> <ItemToCompareCartRecordDto> remove_item_from_compare_table_async(cart_id, item_id, opts)

Remove an item from the compare table

Remove an item from the compare table

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove an item from the compare table
  result = api_instance.remove_item_from_compare_table_async(cart_id, item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->remove_item_from_compare_table_async: #{e}"
end
```

#### Using the remove_item_from_compare_table_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemToCompareCartRecordDto>, Integer, Hash)> remove_item_from_compare_table_async_with_http_info(cart_id, item_id, opts)

```ruby
begin
  # Remove an item from the compare table
  data, status_code, headers = api_instance.remove_item_from_compare_table_async_with_http_info(cart_id, item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemToCompareCartRecordDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->remove_item_from_compare_table_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemToCompareCartRecordDto**](ItemToCompareCartRecordDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## set_cart_country_async

> <EmptyEnvelope> set_cart_country_async(cart_id, opts)

Set the country of a cart

Set the country of a cart

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = 'cart_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  country_switch_request: OpenapiClient::CountrySwitchRequest.new # CountrySwitchRequest | 
}

begin
  # Set the country of a cart
  result = api_instance.set_cart_country_async(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->set_cart_country_async: #{e}"
end
```

#### Using the set_cart_country_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> set_cart_country_async_with_http_info(cart_id, opts)

```ruby
begin
  # Set the country of a cart
  data, status_code, headers = api_instance.set_cart_country_async_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->set_cart_country_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **country_switch_request** | [**CountrySwitchRequest**](CountrySwitchRequest.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## set_cart_currency_async

> <EmptyEnvelope> set_cart_currency_async(cart_id, opts)

Set the currency of a cart

Set the currency of a cart

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = 'cart_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  currency_switch_request: OpenapiClient::CurrencySwitchRequest.new # CurrencySwitchRequest | 
}

begin
  # Set the currency of a cart
  result = api_instance.set_cart_currency_async(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->set_cart_currency_async: #{e}"
end
```

#### Using the set_cart_currency_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> set_cart_currency_async_with_http_info(cart_id, opts)

```ruby
begin
  # Set the currency of a cart
  data, status_code, headers = api_instance.set_cart_currency_async_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->set_cart_currency_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **currency_switch_request** | [**CurrencySwitchRequest**](CurrencySwitchRequest.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## submit_cart_async

> <EmptyEnvelope> submit_cart_async(cart_id, opts)

Submit a cart for processing

Submit a cart for processing

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Submit a cart for processing
  result = api_instance.submit_cart_async(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->submit_cart_async: #{e}"
end
```

#### Using the submit_cart_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> submit_cart_async_with_http_info(cart_id, opts)

```ruby
begin
  # Submit a cart for processing
  data, status_code, headers = api_instance.submit_cart_async_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->submit_cart_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_cart_async

> <EmptyEnvelope> update_cart_async(cart_id, opts)

Update a cart

Update a cart

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cart_update_request: OpenapiClient::CartUpdateRequest.new # CartUpdateRequest | 
}

begin
  # Update a cart
  result = api_instance.update_cart_async(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->update_cart_async: #{e}"
end
```

#### Using the update_cart_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_cart_async_with_http_info(cart_id, opts)

```ruby
begin
  # Update a cart
  data, status_code, headers = api_instance.update_cart_async_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->update_cart_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **cart_update_request** | [**CartUpdateRequest**](CartUpdateRequest.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_cart_line_async

> <EmptyEnvelope> update_cart_line_async(cart_id, line_id, opts)

Update a cart line

Update a cart line

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_cart_record_update_dto: OpenapiClient::ItemCartRecordUpdateDto.new # ItemCartRecordUpdateDto | 
}

begin
  # Update a cart line
  result = api_instance.update_cart_line_async(cart_id, line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->update_cart_line_async: #{e}"
end
```

#### Using the update_cart_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_cart_line_async_with_http_info(cart_id, line_id, opts)

```ruby
begin
  # Update a cart line
  data, status_code, headers = api_instance.update_cart_line_async_with_http_info(cart_id, line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->update_cart_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **line_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_cart_record_update_dto** | [**ItemCartRecordUpdateDto**](ItemCartRecordUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_item_cart_record_async

> <EmptyEnvelope> update_item_cart_record_async(cart_id, item_id, opts)

Update an Item in a cart

Update an Item in a cart

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_cart_record_update_dto: OpenapiClient::ItemCartRecordUpdateDto.new # ItemCartRecordUpdateDto | 
}

begin
  # Update an Item in a cart
  result = api_instance.update_item_cart_record_async(cart_id, item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->update_item_cart_record_async: #{e}"
end
```

#### Using the update_item_cart_record_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_item_cart_record_async_with_http_info(cart_id, item_id, opts)

```ruby
begin
  # Update an Item in a cart
  data, status_code, headers = api_instance.update_item_cart_record_async_with_http_info(cart_id, item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->update_item_cart_record_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_cart_record_update_dto** | [**ItemCartRecordUpdateDto**](ItemCartRecordUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_item_to_wish_list

> <EmptyEnvelope> update_item_to_wish_list(cart_id, wish_list_id, opts)

Update a wish list

Update a wish list

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
wish_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  wish_list_update_dto: OpenapiClient::WishListUpdateDto.new({title: 'title_example'}) # WishListUpdateDto | 
}

begin
  # Update a wish list
  result = api_instance.update_item_to_wish_list(cart_id, wish_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->update_item_to_wish_list: #{e}"
end
```

#### Using the update_item_to_wish_list_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_item_to_wish_list_with_http_info(cart_id, wish_list_id, opts)

```ruby
begin
  # Update a wish list
  data, status_code, headers = api_instance.update_item_to_wish_list_with_http_info(cart_id, wish_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->update_item_to_wish_list_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
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


## wish_list_exists_async

> <BooleanEnvelope> wish_list_exists_async(cart_id, wish_list_id, opts)

Assesses if a WishList exists

Assesses if a WishList exists

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CartsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
wish_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Assesses if a WishList exists
  result = api_instance.wish_list_exists_async(cart_id, wish_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->wish_list_exists_async: #{e}"
end
```

#### Using the wish_list_exists_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BooleanEnvelope>, Integer, Hash)> wish_list_exists_async_with_http_info(cart_id, wish_list_id, opts)

```ruby
begin
  # Assesses if a WishList exists
  data, status_code, headers = api_instance.wish_list_exists_async_with_http_info(cart_id, wish_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BooleanEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CartsApi->wish_list_exists_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **wish_list_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

