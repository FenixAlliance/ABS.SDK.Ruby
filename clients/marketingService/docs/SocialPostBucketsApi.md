# OpenapiClient::SocialPostBucketsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_social_post_bucket_async**](SocialPostBucketsApi.md#create_social_post_bucket_async) | **POST** /api/v2/MarketingService/SocialPostBuckets | Create a social post bucket |
| [**delete_social_post_bucket_async**](SocialPostBucketsApi.md#delete_social_post_bucket_async) | **DELETE** /api/v2/MarketingService/SocialPostBuckets/{socialpostbucketId} | Delete a social post bucket |
| [**get_social_post_bucket_details_async**](SocialPostBucketsApi.md#get_social_post_bucket_details_async) | **GET** /api/v2/MarketingService/SocialPostBuckets/{socialpostbucketId} | Get social post bucket by ID |
| [**get_social_post_buckets_count_async**](SocialPostBucketsApi.md#get_social_post_buckets_count_async) | **GET** /api/v2/MarketingService/SocialPostBuckets/Count | Get social post buckets count |
| [**get_social_post_buckets_o_data_async**](SocialPostBucketsApi.md#get_social_post_buckets_o_data_async) | **GET** /api/v2/MarketingService/SocialPostBuckets | Get social post buckets |
| [**patch_social_post_bucket_async**](SocialPostBucketsApi.md#patch_social_post_bucket_async) | **PATCH** /api/v2/MarketingService/SocialPostBuckets/{socialpostbucketId} | Patch a social post bucket |
| [**update_social_post_bucket_async**](SocialPostBucketsApi.md#update_social_post_bucket_async) | **PUT** /api/v2/MarketingService/SocialPostBuckets/{socialpostbucketId} | Update a social post bucket |


## create_social_post_bucket_async

> <EmptyEnvelope> create_social_post_bucket_async(tenant_id, social_post_bucket_create_dto, opts)

Create a social post bucket

Creates a new social post bucket for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostBucketsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_post_bucket_create_dto = OpenapiClient::SocialPostBucketCreateDto.new # SocialPostBucketCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a social post bucket
  result = api_instance.create_social_post_bucket_async(tenant_id, social_post_bucket_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostBucketsApi->create_social_post_bucket_async: #{e}"
end
```

#### Using the create_social_post_bucket_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_social_post_bucket_async_with_http_info(tenant_id, social_post_bucket_create_dto, opts)

```ruby
begin
  # Create a social post bucket
  data, status_code, headers = api_instance.create_social_post_bucket_async_with_http_info(tenant_id, social_post_bucket_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostBucketsApi->create_social_post_bucket_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **social_post_bucket_create_dto** | [**SocialPostBucketCreateDto**](SocialPostBucketCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_social_post_bucket_async

> <EmptyEnvelope> delete_social_post_bucket_async(tenant_id, socialpostbucket_id, opts)

Delete a social post bucket

Deletes a social post bucket by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostBucketsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
socialpostbucket_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a social post bucket
  result = api_instance.delete_social_post_bucket_async(tenant_id, socialpostbucket_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostBucketsApi->delete_social_post_bucket_async: #{e}"
end
```

#### Using the delete_social_post_bucket_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_social_post_bucket_async_with_http_info(tenant_id, socialpostbucket_id, opts)

```ruby
begin
  # Delete a social post bucket
  data, status_code, headers = api_instance.delete_social_post_bucket_async_with_http_info(tenant_id, socialpostbucket_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostBucketsApi->delete_social_post_bucket_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **socialpostbucket_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_social_post_bucket_details_async

> <SocialPostBucketDtoEnvelope> get_social_post_bucket_details_async(tenant_id, socialpostbucket_id, opts)

Get social post bucket by ID

Retrieves the details of a specific social post bucket by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostBucketsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
socialpostbucket_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get social post bucket by ID
  result = api_instance.get_social_post_bucket_details_async(tenant_id, socialpostbucket_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostBucketsApi->get_social_post_bucket_details_async: #{e}"
end
```

#### Using the get_social_post_bucket_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialPostBucketDtoEnvelope>, Integer, Hash)> get_social_post_bucket_details_async_with_http_info(tenant_id, socialpostbucket_id, opts)

```ruby
begin
  # Get social post bucket by ID
  data, status_code, headers = api_instance.get_social_post_bucket_details_async_with_http_info(tenant_id, socialpostbucket_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialPostBucketDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostBucketsApi->get_social_post_bucket_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **socialpostbucket_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialPostBucketDtoEnvelope**](SocialPostBucketDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_social_post_buckets_count_async

> <Int32Envelope> get_social_post_buckets_count_async(tenant_id, opts)

Get social post buckets count

Returns the count of social post buckets for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostBucketsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get social post buckets count
  result = api_instance.get_social_post_buckets_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostBucketsApi->get_social_post_buckets_count_async: #{e}"
end
```

#### Using the get_social_post_buckets_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_social_post_buckets_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get social post buckets count
  data, status_code, headers = api_instance.get_social_post_buckets_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostBucketsApi->get_social_post_buckets_count_async_with_http_info: #{e}"
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


## get_social_post_buckets_o_data_async

> <SocialPostBucketDtoListEnvelope> get_social_post_buckets_o_data_async(tenant_id, opts)

Get social post buckets

Retrieves a collection of social post buckets for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostBucketsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get social post buckets
  result = api_instance.get_social_post_buckets_o_data_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostBucketsApi->get_social_post_buckets_o_data_async: #{e}"
end
```

#### Using the get_social_post_buckets_o_data_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialPostBucketDtoListEnvelope>, Integer, Hash)> get_social_post_buckets_o_data_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get social post buckets
  data, status_code, headers = api_instance.get_social_post_buckets_o_data_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialPostBucketDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostBucketsApi->get_social_post_buckets_o_data_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialPostBucketDtoListEnvelope**](SocialPostBucketDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_social_post_bucket_async

> <EmptyEnvelope> patch_social_post_bucket_async(tenant_id, socialpostbucket_id, opts)

Patch a social post bucket

Partially updates a social post bucket by its ID using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostBucketsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
socialpostbucket_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a social post bucket
  result = api_instance.patch_social_post_bucket_async(tenant_id, socialpostbucket_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostBucketsApi->patch_social_post_bucket_async: #{e}"
end
```

#### Using the patch_social_post_bucket_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_social_post_bucket_async_with_http_info(tenant_id, socialpostbucket_id, opts)

```ruby
begin
  # Patch a social post bucket
  data, status_code, headers = api_instance.patch_social_post_bucket_async_with_http_info(tenant_id, socialpostbucket_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostBucketsApi->patch_social_post_bucket_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **socialpostbucket_id** | **String** |  |  |
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


## update_social_post_bucket_async

> <EmptyEnvelope> update_social_post_bucket_async(tenant_id, socialpostbucket_id, social_post_bucket_update_dto, opts)

Update a social post bucket

Updates an existing social post bucket by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostBucketsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
socialpostbucket_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_post_bucket_update_dto = OpenapiClient::SocialPostBucketUpdateDto.new # SocialPostBucketUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update a social post bucket
  result = api_instance.update_social_post_bucket_async(tenant_id, socialpostbucket_id, social_post_bucket_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostBucketsApi->update_social_post_bucket_async: #{e}"
end
```

#### Using the update_social_post_bucket_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_social_post_bucket_async_with_http_info(tenant_id, socialpostbucket_id, social_post_bucket_update_dto, opts)

```ruby
begin
  # Update a social post bucket
  data, status_code, headers = api_instance.update_social_post_bucket_async_with_http_info(tenant_id, socialpostbucket_id, social_post_bucket_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostBucketsApi->update_social_post_bucket_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **socialpostbucket_id** | **String** |  |  |
| **social_post_bucket_update_dto** | [**SocialPostBucketUpdateDto**](SocialPostBucketUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

