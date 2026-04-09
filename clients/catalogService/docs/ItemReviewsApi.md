# OpenapiClient::ItemReviewsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_item_review_async**](ItemReviewsApi.md#create_item_review_async) | **POST** /api/v2/CatalogService/ItemReviews | Create a new item review |
| [**delete_item_review_async**](ItemReviewsApi.md#delete_item_review_async) | **DELETE** /api/v2/CatalogService/ItemReviews/{itemReviewId} | Delete an item review |
| [**get_item_review_by_id_async**](ItemReviewsApi.md#get_item_review_by_id_async) | **GET** /api/v2/CatalogService/ItemReviews/{itemReviewId} | Get item review by ID |
| [**get_item_reviews_async**](ItemReviewsApi.md#get_item_reviews_async) | **GET** /api/v2/CatalogService/ItemReviews | Get all item reviews |
| [**update_item_review_async**](ItemReviewsApi.md#update_item_review_async) | **PUT** /api/v2/CatalogService/ItemReviews/{itemReviewId} | Update an item review |


## create_item_review_async

> <ItemReviewDtoEnvelope> create_item_review_async(tenant_id, opts)

Create a new item review

Creates a new item review for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemReviewsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_review_create_dto: OpenapiClient::ItemReviewCreateDto.new # ItemReviewCreateDto | 
}

begin
  # Create a new item review
  result = api_instance.create_item_review_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReviewsApi->create_item_review_async: #{e}"
end
```

#### Using the create_item_review_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemReviewDtoEnvelope>, Integer, Hash)> create_item_review_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new item review
  data, status_code, headers = api_instance.create_item_review_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemReviewDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReviewsApi->create_item_review_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_review_create_dto** | [**ItemReviewCreateDto**](ItemReviewCreateDto.md) |  | [optional] |

### Return type

[**ItemReviewDtoEnvelope**](ItemReviewDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_item_review_async

> delete_item_review_async(tenant_id, item_review_id, opts)

Delete an item review

Deletes an item review for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemReviewsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_review_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an item review
  api_instance.delete_item_review_async(tenant_id, item_review_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReviewsApi->delete_item_review_async: #{e}"
end
```

#### Using the delete_item_review_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_item_review_async_with_http_info(tenant_id, item_review_id, opts)

```ruby
begin
  # Delete an item review
  data, status_code, headers = api_instance.delete_item_review_async_with_http_info(tenant_id, item_review_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReviewsApi->delete_item_review_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_review_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_review_by_id_async

> <ItemReviewDtoEnvelope> get_item_review_by_id_async(item_review_id, opts)

Get item review by ID

Retrieves a specific item review by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemReviewsApi.new
item_review_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item review by ID
  result = api_instance.get_item_review_by_id_async(item_review_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReviewsApi->get_item_review_by_id_async: #{e}"
end
```

#### Using the get_item_review_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemReviewDtoEnvelope>, Integer, Hash)> get_item_review_by_id_async_with_http_info(item_review_id, opts)

```ruby
begin
  # Get item review by ID
  data, status_code, headers = api_instance.get_item_review_by_id_async_with_http_info(item_review_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemReviewDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReviewsApi->get_item_review_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_review_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemReviewDtoEnvelope**](ItemReviewDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_reviews_async

> <ItemReviewDtoListEnvelope> get_item_reviews_async(item_id, opts)

Get all item reviews

Retrieves all item reviews for the specified item using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemReviewsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all item reviews
  result = api_instance.get_item_reviews_async(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReviewsApi->get_item_reviews_async: #{e}"
end
```

#### Using the get_item_reviews_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemReviewDtoListEnvelope>, Integer, Hash)> get_item_reviews_async_with_http_info(item_id, opts)

```ruby
begin
  # Get all item reviews
  data, status_code, headers = api_instance.get_item_reviews_async_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemReviewDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReviewsApi->get_item_reviews_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemReviewDtoListEnvelope**](ItemReviewDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_item_review_async

> update_item_review_async(tenant_id, item_review_id, opts)

Update an item review

Updates an existing item review for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemReviewsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_review_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_review_update_dto: OpenapiClient::ItemReviewUpdateDto.new # ItemReviewUpdateDto | 
}

begin
  # Update an item review
  api_instance.update_item_review_async(tenant_id, item_review_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReviewsApi->update_item_review_async: #{e}"
end
```

#### Using the update_item_review_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_item_review_async_with_http_info(tenant_id, item_review_id, opts)

```ruby
begin
  # Update an item review
  data, status_code, headers = api_instance.update_item_review_async_with_http_info(tenant_id, item_review_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReviewsApi->update_item_review_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_review_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_review_update_dto** | [**ItemReviewUpdateDto**](ItemReviewUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

