# OpenapiClient::OrdersApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**calculate_order**](OrdersApi.md#calculate_order) | **PUT** /api/v2/OrdersService/Orders/{orderId}/Calculate | Calculates totals for an order. |
| [**calculate_order_line**](OrdersApi.md#calculate_order_line) | **PUT** /api/v2/OrdersService/Orders/{orderId}/Lines/{orderLineId}/Calculate | Calculates totals for an order line. |
| [**create_order**](OrdersApi.md#create_order) | **POST** /api/v2/OrdersService/Orders | Creates a new order. |
| [**create_order_line**](OrdersApi.md#create_order_line) | **POST** /api/v2/OrdersService/Orders/{orderId}/Lines | Creates a new order line. |
| [**delete_order**](OrdersApi.md#delete_order) | **DELETE** /api/v2/OrdersService/Orders/{orderId} | Deletes an order. |
| [**delete_order_line**](OrdersApi.md#delete_order_line) | **DELETE** /api/v2/OrdersService/Orders/{orderId}/Lines/{orderLineId} | Deletes an order line. |
| [**get_extended_orders**](OrdersApi.md#get_extended_orders) | **GET** /api/v2/OrdersService/Orders/Extended | Gets a list of extended orders for a tenant. |
| [**get_order**](OrdersApi.md#get_order) | **GET** /api/v2/OrdersService/Orders/{orderId} | Gets a specific order by ID. |
| [**get_order_line**](OrdersApi.md#get_order_line) | **GET** /api/v2/OrdersService/Orders/{orderId}/Lines/{orderLineId} | Gets a specific order line. |
| [**get_order_lines**](OrdersApi.md#get_order_lines) | **GET** /api/v2/OrdersService/Orders/{orderId}/Lines | Gets order lines for an order. |
| [**get_order_lines_count**](OrdersApi.md#get_order_lines_count) | **GET** /api/v2/OrdersService/Orders/{orderId}/Lines/Count | Gets the count of order lines for an order. |
| [**get_orders**](OrdersApi.md#get_orders) | **GET** /api/v2/OrdersService/Orders | Gets a list of orders for a tenant. |
| [**get_orders_count**](OrdersApi.md#get_orders_count) | **GET** /api/v2/OrdersService/Orders/Count | Gets the count of orders for a tenant. |
| [**patch_order**](OrdersApi.md#patch_order) | **PATCH** /api/v2/OrdersService/Orders/{orderId} | Partially updates an existing order. |
| [**patch_order_line**](OrdersApi.md#patch_order_line) | **PATCH** /api/v2/OrdersService/Orders/{orderId}/Lines/{orderLineId} | Partially updates an order line. |
| [**preview_order_email_template**](OrdersApi.md#preview_order_email_template) | **POST** /api/v2/OrdersService/Orders/{orderId}/Emails/Preview | Preview the rendered email for an Order. |
| [**send_order_email**](OrdersApi.md#send_order_email) | **POST** /api/v2/OrdersService/Orders/{orderId}/Emails/Send | Send a transactional email for an order. |
| [**submit_cart**](OrdersApi.md#submit_cart) | **POST** /api/v2/OrdersService/Orders/SubmitCart | Submits a cart and creates an order. |
| [**update_order**](OrdersApi.md#update_order) | **PUT** /api/v2/OrdersService/Orders/{orderId} | Updates an existing order. |
| [**update_order_line**](OrdersApi.md#update_order_line) | **PUT** /api/v2/OrdersService/Orders/{orderId}/Lines/{orderLineId} | Updates an order line. |


## calculate_order

> <EmptyEnvelope> calculate_order(tenant_id, order_id)

Calculates totals for an order.

Performs calculation of totals and taxes for the specified order.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
order_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Calculates totals for an order.
  result = api_instance.calculate_order(tenant_id, order_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->calculate_order: #{e}"
end
```

#### Using the calculate_order_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> calculate_order_with_http_info(tenant_id, order_id)

```ruby
begin
  # Calculates totals for an order.
  data, status_code, headers = api_instance.calculate_order_with_http_info(tenant_id, order_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->calculate_order_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **order_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## calculate_order_line

> <EmptyEnvelope> calculate_order_line(tenant_id, order_id, order_line_id)

Calculates totals for an order line.

Performs calculation of totals and taxes for the specified order line.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
order_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
order_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Calculates totals for an order line.
  result = api_instance.calculate_order_line(tenant_id, order_id, order_line_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->calculate_order_line: #{e}"
end
```

#### Using the calculate_order_line_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> calculate_order_line_with_http_info(tenant_id, order_id, order_line_id)

```ruby
begin
  # Calculates totals for an order line.
  data, status_code, headers = api_instance.calculate_order_line_with_http_info(tenant_id, order_id, order_line_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->calculate_order_line_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **order_id** | **String** |  |  |
| **order_line_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_order

> <EmptyEnvelope> create_order(tenant_id, opts)

Creates a new order.

Creates a new order for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  order_create_dto: OpenapiClient::OrderCreateDto.new # OrderCreateDto | 
}

begin
  # Creates a new order.
  result = api_instance.create_order(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->create_order: #{e}"
end
```

#### Using the create_order_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_order_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new order.
  data, status_code, headers = api_instance.create_order_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->create_order_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **order_create_dto** | [**OrderCreateDto**](OrderCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_order_line

> <EmptyEnvelope> create_order_line(tenant_id, order_id, opts)

Creates a new order line.

Creates a new line (item) for the specified order.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
order_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  order_line_create_dto: OpenapiClient::OrderLineCreateDto.new # OrderLineCreateDto | 
}

begin
  # Creates a new order line.
  result = api_instance.create_order_line(tenant_id, order_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->create_order_line: #{e}"
end
```

#### Using the create_order_line_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_order_line_with_http_info(tenant_id, order_id, opts)

```ruby
begin
  # Creates a new order line.
  data, status_code, headers = api_instance.create_order_line_with_http_info(tenant_id, order_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->create_order_line_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **order_id** | **String** |  |  |
| **order_line_create_dto** | [**OrderLineCreateDto**](OrderLineCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_order

> <EmptyEnvelope> delete_order(tenant_id, order_id)

Deletes an order.

Deletes the specified order.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
order_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes an order.
  result = api_instance.delete_order(tenant_id, order_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->delete_order: #{e}"
end
```

#### Using the delete_order_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_order_with_http_info(tenant_id, order_id)

```ruby
begin
  # Deletes an order.
  data, status_code, headers = api_instance.delete_order_with_http_info(tenant_id, order_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->delete_order_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **order_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_order_line

> <EmptyEnvelope> delete_order_line(tenant_id, order_id, order_line_id)

Deletes an order line.

Deletes the specified order line.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
order_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
order_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes an order line.
  result = api_instance.delete_order_line(tenant_id, order_id, order_line_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->delete_order_line: #{e}"
end
```

#### Using the delete_order_line_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_order_line_with_http_info(tenant_id, order_id, order_line_id)

```ruby
begin
  # Deletes an order line.
  data, status_code, headers = api_instance.delete_order_line_with_http_info(tenant_id, order_id, order_line_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->delete_order_line_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **order_id** | **String** |  |  |
| **order_line_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_extended_orders

> <ExtendedOrderDtoListEnvelope> get_extended_orders(tenant_id, opts)

Gets a list of extended orders for a tenant.

Retrieves a list of extended order details for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  extended_order_dto_collection_query_parameters: OpenapiClient::ExtendedOrderDtoCollectionQueryParameters.new # ExtendedOrderDtoCollectionQueryParameters | 
}

begin
  # Gets a list of extended orders for a tenant.
  result = api_instance.get_extended_orders(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->get_extended_orders: #{e}"
end
```

#### Using the get_extended_orders_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExtendedOrderDtoListEnvelope>, Integer, Hash)> get_extended_orders_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets a list of extended orders for a tenant.
  data, status_code, headers = api_instance.get_extended_orders_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExtendedOrderDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->get_extended_orders_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **extended_order_dto_collection_query_parameters** | [**ExtendedOrderDtoCollectionQueryParameters**](ExtendedOrderDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ExtendedOrderDtoListEnvelope**](ExtendedOrderDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_order

> <OrderDtoEnvelope> get_order(tenant_id, order_id)

Gets a specific order by ID.

Retrieves the details of a specific order by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
order_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a specific order by ID.
  result = api_instance.get_order(tenant_id, order_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->get_order: #{e}"
end
```

#### Using the get_order_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OrderDtoEnvelope>, Integer, Hash)> get_order_with_http_info(tenant_id, order_id)

```ruby
begin
  # Gets a specific order by ID.
  data, status_code, headers = api_instance.get_order_with_http_info(tenant_id, order_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OrderDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->get_order_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **order_id** | **String** |  |  |

### Return type

[**OrderDtoEnvelope**](OrderDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_order_line

> <OrderLineDtoEnvelope> get_order_line(tenant_id, order_id, order_line_id)

Gets a specific order line.

Retrieves the details of a specific order line by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
order_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
order_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a specific order line.
  result = api_instance.get_order_line(tenant_id, order_id, order_line_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->get_order_line: #{e}"
end
```

#### Using the get_order_line_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OrderLineDtoEnvelope>, Integer, Hash)> get_order_line_with_http_info(tenant_id, order_id, order_line_id)

```ruby
begin
  # Gets a specific order line.
  data, status_code, headers = api_instance.get_order_line_with_http_info(tenant_id, order_id, order_line_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OrderLineDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->get_order_line_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **order_id** | **String** |  |  |
| **order_line_id** | **String** |  |  |

### Return type

[**OrderLineDtoEnvelope**](OrderLineDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_order_lines

> <OrderLineDtoListEnvelope> get_order_lines(tenant_id, order_id, opts)

Gets order lines for an order.

Retrieves the lines (items) for the specified order.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
order_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  order_line_dto_collection_query_parameters: OpenapiClient::OrderLineDtoCollectionQueryParameters.new # OrderLineDtoCollectionQueryParameters | 
}

begin
  # Gets order lines for an order.
  result = api_instance.get_order_lines(tenant_id, order_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->get_order_lines: #{e}"
end
```

#### Using the get_order_lines_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OrderLineDtoListEnvelope>, Integer, Hash)> get_order_lines_with_http_info(tenant_id, order_id, opts)

```ruby
begin
  # Gets order lines for an order.
  data, status_code, headers = api_instance.get_order_lines_with_http_info(tenant_id, order_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OrderLineDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->get_order_lines_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **order_id** | **String** |  |  |
| **item_id** | **String** |  | [optional] |
| **order_line_dto_collection_query_parameters** | [**OrderLineDtoCollectionQueryParameters**](OrderLineDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**OrderLineDtoListEnvelope**](OrderLineDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_order_lines_count

> <Int32Envelope> get_order_lines_count(tenant_id, order_id, opts)

Gets the count of order lines for an order.

Retrieves the total number of lines for the specified order.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
order_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  order_line_dto_collection_query_parameters: OpenapiClient::OrderLineDtoCollectionQueryParameters.new # OrderLineDtoCollectionQueryParameters | 
}

begin
  # Gets the count of order lines for an order.
  result = api_instance.get_order_lines_count(tenant_id, order_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->get_order_lines_count: #{e}"
end
```

#### Using the get_order_lines_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_order_lines_count_with_http_info(tenant_id, order_id, opts)

```ruby
begin
  # Gets the count of order lines for an order.
  data, status_code, headers = api_instance.get_order_lines_count_with_http_info(tenant_id, order_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->get_order_lines_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **order_id** | **String** |  |  |
| **order_line_dto_collection_query_parameters** | [**OrderLineDtoCollectionQueryParameters**](OrderLineDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_orders

> <OrderDtoListEnvelope> get_orders(tenant_id, opts)

Gets a list of orders for a tenant.

Retrieves a list of orders for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  order_dto_collection_query_parameters: OpenapiClient::OrderDtoCollectionQueryParameters.new # OrderDtoCollectionQueryParameters | 
}

begin
  # Gets a list of orders for a tenant.
  result = api_instance.get_orders(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->get_orders: #{e}"
end
```

#### Using the get_orders_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OrderDtoListEnvelope>, Integer, Hash)> get_orders_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets a list of orders for a tenant.
  data, status_code, headers = api_instance.get_orders_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OrderDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->get_orders_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **order_dto_collection_query_parameters** | [**OrderDtoCollectionQueryParameters**](OrderDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**OrderDtoListEnvelope**](OrderDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_orders_count

> <Int32Envelope> get_orders_count(tenant_id, opts)

Gets the count of orders for a tenant.

Retrieves the total number of orders for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  order_dto_collection_query_parameters: OpenapiClient::OrderDtoCollectionQueryParameters.new # OrderDtoCollectionQueryParameters | 
}

begin
  # Gets the count of orders for a tenant.
  result = api_instance.get_orders_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->get_orders_count: #{e}"
end
```

#### Using the get_orders_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_orders_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets the count of orders for a tenant.
  data, status_code, headers = api_instance.get_orders_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->get_orders_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **order_dto_collection_query_parameters** | [**OrderDtoCollectionQueryParameters**](OrderDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_order

> <EmptyEnvelope> patch_order(tenant_id, order_id, opts)

Partially updates an existing order.

Applies a JSON Patch document to partially update an existing order.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
order_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Partially updates an existing order.
  result = api_instance.patch_order(tenant_id, order_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->patch_order: #{e}"
end
```

#### Using the patch_order_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_order_with_http_info(tenant_id, order_id, opts)

```ruby
begin
  # Partially updates an existing order.
  data, status_code, headers = api_instance.patch_order_with_http_info(tenant_id, order_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->patch_order_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **order_id** | **String** |  |  |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_order_line

> <EmptyEnvelope> patch_order_line(tenant_id, order_id, order_line_id, opts)

Partially updates an order line.

Applies a JSON Patch document to partially update a specific order line.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
order_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
order_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Partially updates an order line.
  result = api_instance.patch_order_line(tenant_id, order_id, order_line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->patch_order_line: #{e}"
end
```

#### Using the patch_order_line_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_order_line_with_http_info(tenant_id, order_id, order_line_id, opts)

```ruby
begin
  # Partially updates an order line.
  data, status_code, headers = api_instance.patch_order_line_with_http_info(tenant_id, order_id, order_line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->patch_order_line_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **order_id** | **String** |  |  |
| **order_line_id** | **String** |  |  |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## preview_order_email_template

> preview_order_email_template(order_id, tenant_id, opts)

Preview the rendered email for an Order.

Previews the rendered email template for the specified order. Only users with the 'send_email' permission are permitted.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
order_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  email_dispatch_request: OpenapiClient::EmailDispatchRequest.new({title: 'title_example', message: 'message_example', culture: 'culture_example', ui_culture: 'ui_culture_example', recipients: ['recipients_example']}) # EmailDispatchRequest | 
}

begin
  # Preview the rendered email for an Order.
  api_instance.preview_order_email_template(order_id, tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->preview_order_email_template: #{e}"
end
```

#### Using the preview_order_email_template_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> preview_order_email_template_with_http_info(order_id, tenant_id, opts)

```ruby
begin
  # Preview the rendered email for an Order.
  data, status_code, headers = api_instance.preview_order_email_template_with_http_info(order_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->preview_order_email_template_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **order_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **email_dispatch_request** | [**EmailDispatchRequest**](EmailDispatchRequest.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: Not defined


## send_order_email

> <EmptyEnvelope> send_order_email(tenant_id, order_id, opts)

Send a transactional email for an order.

Sends a transactional email for the specified order. Only users with the 'send_email' permission are permitted.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
order_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  email_dispatch_request: OpenapiClient::EmailDispatchRequest.new({title: 'title_example', message: 'message_example', culture: 'culture_example', ui_culture: 'ui_culture_example', recipients: ['recipients_example']}) # EmailDispatchRequest | 
}

begin
  # Send a transactional email for an order.
  result = api_instance.send_order_email(tenant_id, order_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->send_order_email: #{e}"
end
```

#### Using the send_order_email_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> send_order_email_with_http_info(tenant_id, order_id, opts)

```ruby
begin
  # Send a transactional email for an order.
  data, status_code, headers = api_instance.send_order_email_with_http_info(tenant_id, order_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->send_order_email_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **order_id** | **String** |  |  |
| **email_dispatch_request** | [**EmailDispatchRequest**](EmailDispatchRequest.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## submit_cart

> <OrderDtoEnvelope> submit_cart(cart_id)

Submits a cart and creates an order.

Submits the specified cart and creates an order for the authenticated user.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Submits a cart and creates an order.
  result = api_instance.submit_cart(cart_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->submit_cart: #{e}"
end
```

#### Using the submit_cart_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OrderDtoEnvelope>, Integer, Hash)> submit_cart_with_http_info(cart_id)

```ruby
begin
  # Submits a cart and creates an order.
  data, status_code, headers = api_instance.submit_cart_with_http_info(cart_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OrderDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->submit_cart_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |

### Return type

[**OrderDtoEnvelope**](OrderDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_order

> <EmptyEnvelope> update_order(tenant_id, order_id, opts)

Updates an existing order.

Updates the details of an existing order.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
order_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  order_update_dto: OpenapiClient::OrderUpdateDto.new # OrderUpdateDto | 
}

begin
  # Updates an existing order.
  result = api_instance.update_order(tenant_id, order_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->update_order: #{e}"
end
```

#### Using the update_order_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_order_with_http_info(tenant_id, order_id, opts)

```ruby
begin
  # Updates an existing order.
  data, status_code, headers = api_instance.update_order_with_http_info(tenant_id, order_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->update_order_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **order_id** | **String** |  |  |
| **order_update_dto** | [**OrderUpdateDto**](OrderUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_order_line

> <EmptyEnvelope> update_order_line(tenant_id, order_id, order_line_id, opts)

Updates an order line.

Updates the details of a specific order line.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
order_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
order_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  order_line_update_dto: OpenapiClient::OrderLineUpdateDto.new # OrderLineUpdateDto | 
}

begin
  # Updates an order line.
  result = api_instance.update_order_line(tenant_id, order_id, order_line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->update_order_line: #{e}"
end
```

#### Using the update_order_line_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_order_line_with_http_info(tenant_id, order_id, order_line_id, opts)

```ruby
begin
  # Updates an order line.
  data, status_code, headers = api_instance.update_order_line_with_http_info(tenant_id, order_id, order_line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OrdersApi->update_order_line_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **order_id** | **String** |  |  |
| **order_line_id** | **String** |  |  |
| **order_line_update_dto** | [**OrderLineUpdateDto**](OrderLineUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

