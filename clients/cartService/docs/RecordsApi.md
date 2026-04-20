# OpenapiClient::RecordsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**add_item_to_cart**](RecordsApi.md#add_item_to_cart) | **POST** /api/v2/CartService/Records/AddItem | Add an item to a cart |
| [**add_product_to_cart_async**](RecordsApi.md#add_product_to_cart_async) | **POST** /api/v2/CartService/Records | Add a product to a cart with tracking |
| [**clear_cart_async**](RecordsApi.md#clear_cart_async) | **POST** /api/v2/CartService/Records/ClearCart | Clear all items from a cart |
| [**decrease_item_cart_record**](RecordsApi.md#decrease_item_cart_record) | **PUT** /api/v2/CartService/Records/{recordId}/Decrease | Decrease cart record quantity |
| [**get_item_cart_record**](RecordsApi.md#get_item_cart_record) | **GET** /api/v2/CartService/Records/{recordId}/Details | Get a cart record by ID |
| [**get_items_in_cart_async**](RecordsApi.md#get_items_in_cart_async) | **GET** /api/v2/CartService/Records/{cartId} | Get all items in a cart |
| [**increase_item_cart_record**](RecordsApi.md#increase_item_cart_record) | **PUT** /api/v2/CartService/Records/{recordId}/Increase | Increase cart record quantity |
| [**is_item_already_in_cart**](RecordsApi.md#is_item_already_in_cart) | **GET** /api/v2/CartService/Records/IsInCart | Check if an item is in a cart |
| [**remove_product_from_cart_by_params**](RecordsApi.md#remove_product_from_cart_by_params) | **DELETE** /api/v2/CartService/Records | Remove a product from a cart |
| [**remove_product_from_cart_by_record_id**](RecordsApi.md#remove_product_from_cart_by_record_id) | **DELETE** /api/v2/CartService/Records/{recordId} | Remove a product from a cart by record ID |
| [**update_item_cart_record**](RecordsApi.md#update_item_cart_record) | **PUT** /api/v2/CartService/Records/{recordId} | Update a cart record |


## add_item_to_cart

> <EmptyEnvelope> add_item_to_cart(opts)

Add an item to a cart

Adds an item with the specified quantity to the given cart.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RecordsApi.new
opts = {
  cart_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  quantity: 56, # Integer | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Add an item to a cart
  result = api_instance.add_item_to_cart(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->add_item_to_cart: #{e}"
end
```

#### Using the add_item_to_cart_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> add_item_to_cart_with_http_info(opts)

```ruby
begin
  # Add an item to a cart
  data, status_code, headers = api_instance.add_item_to_cart_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->add_item_to_cart_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  | [optional] |
| **item_id** | **String** |  | [optional] |
| **quantity** | **Integer** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## add_product_to_cart_async

> <EmptyEnvelope> add_product_to_cart_async(opts)

Add a product to a cart with tracking

Adds a product to the cart using a request body with cart ID, product ID, and quantity.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RecordsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_cart_record_create_dto: OpenapiClient::ItemCartRecordCreateDto.new # ItemCartRecordCreateDto | 
}

begin
  # Add a product to a cart with tracking
  result = api_instance.add_product_to_cart_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->add_product_to_cart_async: #{e}"
end
```

#### Using the add_product_to_cart_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> add_product_to_cart_async_with_http_info(opts)

```ruby
begin
  # Add a product to a cart with tracking
  data, status_code, headers = api_instance.add_product_to_cart_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->add_product_to_cart_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_cart_record_create_dto** | [**ItemCartRecordCreateDto**](ItemCartRecordCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## clear_cart_async

> <EmptyEnvelope> clear_cart_async(cart_id, opts)

Clear all items from a cart

Removes all item records from the specified cart.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RecordsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Clear all items from a cart
  result = api_instance.clear_cart_async(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->clear_cart_async: #{e}"
end
```

#### Using the clear_cart_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> clear_cart_async_with_http_info(cart_id, opts)

```ruby
begin
  # Clear all items from a cart
  data, status_code, headers = api_instance.clear_cart_async_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->clear_cart_async_with_http_info: #{e}"
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


## decrease_item_cart_record

> <EmptyEnvelope> decrease_item_cart_record(record_id, opts)

Decrease cart record quantity

Decreases the quantity of the specified item cart record by the given amount.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RecordsApi.new
record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  quantity: 1.2, # Float | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Decrease cart record quantity
  result = api_instance.decrease_item_cart_record(record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->decrease_item_cart_record: #{e}"
end
```

#### Using the decrease_item_cart_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> decrease_item_cart_record_with_http_info(record_id, opts)

```ruby
begin
  # Decrease cart record quantity
  data, status_code, headers = api_instance.decrease_item_cart_record_with_http_info(record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->decrease_item_cart_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **record_id** | **String** |  |  |
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


## get_item_cart_record

> <EmptyEnvelope> get_item_cart_record(record_id, opts)

Get a cart record by ID

Retrieves the details of a specific item cart record.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RecordsApi.new
record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a cart record by ID
  result = api_instance.get_item_cart_record(record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->get_item_cart_record: #{e}"
end
```

#### Using the get_item_cart_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> get_item_cart_record_with_http_info(record_id, opts)

```ruby
begin
  # Get a cart record by ID
  data, status_code, headers = api_instance.get_item_cart_record_with_http_info(record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->get_item_cart_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
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


## get_items_in_cart_async

> <ItemCartRecordDtoListEnvelope> get_items_in_cart_async(cart_id, opts)

Get all items in a cart

Retrieves all item cart records for the specified cart.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RecordsApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all items in a cart
  result = api_instance.get_items_in_cart_async(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->get_items_in_cart_async: #{e}"
end
```

#### Using the get_items_in_cart_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemCartRecordDtoListEnvelope>, Integer, Hash)> get_items_in_cart_async_with_http_info(cart_id, opts)

```ruby
begin
  # Get all items in a cart
  data, status_code, headers = api_instance.get_items_in_cart_async_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemCartRecordDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->get_items_in_cart_async_with_http_info: #{e}"
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


## increase_item_cart_record

> <EmptyEnvelope> increase_item_cart_record(record_id, opts)

Increase cart record quantity

Increases the quantity of the specified item cart record by the given amount.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RecordsApi.new
record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  quantity: 1.2, # Float | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Increase cart record quantity
  result = api_instance.increase_item_cart_record(record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->increase_item_cart_record: #{e}"
end
```

#### Using the increase_item_cart_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> increase_item_cart_record_with_http_info(record_id, opts)

```ruby
begin
  # Increase cart record quantity
  data, status_code, headers = api_instance.increase_item_cart_record_with_http_info(record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->increase_item_cart_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **record_id** | **String** |  |  |
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


## is_item_already_in_cart

> <BooleanEnvelope> is_item_already_in_cart(item_id, cart_id, opts)

Check if an item is in a cart

Returns a boolean indicating whether the specified item is already in the given cart.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RecordsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Check if an item is in a cart
  result = api_instance.is_item_already_in_cart(item_id, cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->is_item_already_in_cart: #{e}"
end
```

#### Using the is_item_already_in_cart_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BooleanEnvelope>, Integer, Hash)> is_item_already_in_cart_with_http_info(item_id, cart_id, opts)

```ruby
begin
  # Check if an item is in a cart
  data, status_code, headers = api_instance.is_item_already_in_cart_with_http_info(item_id, cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BooleanEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->is_item_already_in_cart_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **cart_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_product_from_cart_by_params

> <EmptyEnvelope> remove_product_from_cart_by_params(opts)

Remove a product from a cart

Removes a product from the cart using cart ID and product ID query parameters.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RecordsApi.new
opts = {
  cart_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  product_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove a product from a cart
  result = api_instance.remove_product_from_cart_by_params(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->remove_product_from_cart_by_params: #{e}"
end
```

#### Using the remove_product_from_cart_by_params_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> remove_product_from_cart_by_params_with_http_info(opts)

```ruby
begin
  # Remove a product from a cart
  data, status_code, headers = api_instance.remove_product_from_cart_by_params_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->remove_product_from_cart_by_params_with_http_info: #{e}"
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

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_product_from_cart_by_record_id

> <EmptyEnvelope> remove_product_from_cart_by_record_id(record_id, opts)

Remove a product from a cart by record ID

Removes a specific item record from the cart by its record ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RecordsApi.new
record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove a product from a cart by record ID
  result = api_instance.remove_product_from_cart_by_record_id(record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->remove_product_from_cart_by_record_id: #{e}"
end
```

#### Using the remove_product_from_cart_by_record_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> remove_product_from_cart_by_record_id_with_http_info(record_id, opts)

```ruby
begin
  # Remove a product from a cart by record ID
  data, status_code, headers = api_instance.remove_product_from_cart_by_record_id_with_http_info(record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->remove_product_from_cart_by_record_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
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


## update_item_cart_record

> <EmptyEnvelope> update_item_cart_record(record_id, opts)

Update a cart record

Updates the specified item cart record with the provided data.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RecordsApi.new
record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_cart_record_update_dto: OpenapiClient::ItemCartRecordUpdateDto.new # ItemCartRecordUpdateDto | 
}

begin
  # Update a cart record
  result = api_instance.update_item_cart_record(record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->update_item_cart_record: #{e}"
end
```

#### Using the update_item_cart_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_item_cart_record_with_http_info(record_id, opts)

```ruby
begin
  # Update a cart record
  data, status_code, headers = api_instance.update_item_cart_record_with_http_info(record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RecordsApi->update_item_cart_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **record_id** | **String** |  |  |
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

