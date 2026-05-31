# OpenapiClient::PointOfSalesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_point_of_sales_async**](PointOfSalesApi.md#count_point_of_sales_async) | **GET** /api/v2/SalesService/PointOfSales/Count | Get point of sales count |
| [**create_point_of_sale_async**](PointOfSalesApi.md#create_point_of_sale_async) | **POST** /api/v2/SalesService/PointOfSales | Create a point of sale |
| [**delete_point_of_sale_async**](PointOfSalesApi.md#delete_point_of_sale_async) | **DELETE** /api/v2/SalesService/PointOfSales/{pointOfSaleId} | Delete a point of sale |
| [**get_point_of_sale_async**](PointOfSalesApi.md#get_point_of_sale_async) | **GET** /api/v2/SalesService/PointOfSales/{pointOfSaleId} | Get point of sale by ID |
| [**get_point_of_sales_async**](PointOfSalesApi.md#get_point_of_sales_async) | **GET** /api/v2/SalesService/PointOfSales | Get point of sales |
| [**update_point_of_sale_async**](PointOfSalesApi.md#update_point_of_sale_async) | **PUT** /api/v2/SalesService/PointOfSales/{pointOfSaleId} | Update a point of sale |


## count_point_of_sales_async

> <Int32Envelope> count_point_of_sales_async(tenant_id)

Get point of sales count

Returns the total count of point of sales for the specified tenant with OData filter support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PointOfSalesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get point of sales count
  result = api_instance.count_point_of_sales_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PointOfSalesApi->count_point_of_sales_async: #{e}"
end
```

#### Using the count_point_of_sales_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_point_of_sales_async_with_http_info(tenant_id)

```ruby
begin
  # Get point of sales count
  data, status_code, headers = api_instance.count_point_of_sales_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PointOfSalesApi->count_point_of_sales_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_point_of_sale_async

> <EmptyEnvelope> create_point_of_sale_async(tenant_id, opts)

Create a point of sale

Creates a new point of sale for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PointOfSalesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  point_of_sale_create_dto: OpenapiClient::PointOfSaleCreateDto.new({title: 'title_example'}) # PointOfSaleCreateDto | 
}

begin
  # Create a point of sale
  result = api_instance.create_point_of_sale_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PointOfSalesApi->create_point_of_sale_async: #{e}"
end
```

#### Using the create_point_of_sale_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_point_of_sale_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a point of sale
  data, status_code, headers = api_instance.create_point_of_sale_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PointOfSalesApi->create_point_of_sale_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **point_of_sale_create_dto** | [**PointOfSaleCreateDto**](PointOfSaleCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_point_of_sale_async

> <EmptyEnvelope> delete_point_of_sale_async(tenant_id, point_of_sale_id)

Delete a point of sale

Deletes an existing point of sale by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PointOfSalesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
point_of_sale_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete a point of sale
  result = api_instance.delete_point_of_sale_async(tenant_id, point_of_sale_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PointOfSalesApi->delete_point_of_sale_async: #{e}"
end
```

#### Using the delete_point_of_sale_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_point_of_sale_async_with_http_info(tenant_id, point_of_sale_id)

```ruby
begin
  # Delete a point of sale
  data, status_code, headers = api_instance.delete_point_of_sale_async_with_http_info(tenant_id, point_of_sale_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PointOfSalesApi->delete_point_of_sale_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **point_of_sale_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_point_of_sale_async

> <PointOfSaleDtoEnvelope> get_point_of_sale_async(tenant_id, point_of_sale_id)

Get point of sale by ID

Retrieves a single point of sale by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PointOfSalesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
point_of_sale_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get point of sale by ID
  result = api_instance.get_point_of_sale_async(tenant_id, point_of_sale_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PointOfSalesApi->get_point_of_sale_async: #{e}"
end
```

#### Using the get_point_of_sale_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PointOfSaleDtoEnvelope>, Integer, Hash)> get_point_of_sale_async_with_http_info(tenant_id, point_of_sale_id)

```ruby
begin
  # Get point of sale by ID
  data, status_code, headers = api_instance.get_point_of_sale_async_with_http_info(tenant_id, point_of_sale_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PointOfSaleDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PointOfSalesApi->get_point_of_sale_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **point_of_sale_id** | **String** |  |  |

### Return type

[**PointOfSaleDtoEnvelope**](PointOfSaleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_point_of_sales_async

> <PointOfSaleDtoListEnvelope> get_point_of_sales_async(tenant_id)

Get point of sales

Retrieves a list of point of sales for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PointOfSalesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get point of sales
  result = api_instance.get_point_of_sales_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PointOfSalesApi->get_point_of_sales_async: #{e}"
end
```

#### Using the get_point_of_sales_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PointOfSaleDtoListEnvelope>, Integer, Hash)> get_point_of_sales_async_with_http_info(tenant_id)

```ruby
begin
  # Get point of sales
  data, status_code, headers = api_instance.get_point_of_sales_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PointOfSaleDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PointOfSalesApi->get_point_of_sales_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**PointOfSaleDtoListEnvelope**](PointOfSaleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_point_of_sale_async

> <EmptyEnvelope> update_point_of_sale_async(tenant_id, point_of_sale_id, opts)

Update a point of sale

Updates an existing point of sale by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PointOfSalesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
point_of_sale_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  point_of_sale_update_dto: OpenapiClient::PointOfSaleUpdateDto.new # PointOfSaleUpdateDto | 
}

begin
  # Update a point of sale
  result = api_instance.update_point_of_sale_async(tenant_id, point_of_sale_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PointOfSalesApi->update_point_of_sale_async: #{e}"
end
```

#### Using the update_point_of_sale_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_point_of_sale_async_with_http_info(tenant_id, point_of_sale_id, opts)

```ruby
begin
  # Update a point of sale
  data, status_code, headers = api_instance.update_point_of_sale_async_with_http_info(tenant_id, point_of_sale_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PointOfSalesApi->update_point_of_sale_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **point_of_sale_id** | **String** |  |  |
| **point_of_sale_update_dto** | [**PointOfSaleUpdateDto**](PointOfSaleUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

