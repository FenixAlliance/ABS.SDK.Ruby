# OpenapiClient::SocialMediaPostsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_social_media_post_async**](SocialMediaPostsApi.md#create_social_media_post_async) | **POST** /api/v2/MarketingService/SocialMediaPosts | Create a social media post |
| [**delete_social_media_post_async**](SocialMediaPostsApi.md#delete_social_media_post_async) | **DELETE** /api/v2/MarketingService/SocialMediaPosts/{socialmediapostId} | Delete a social media post |
| [**get_social_media_post_details_async**](SocialMediaPostsApi.md#get_social_media_post_details_async) | **GET** /api/v2/MarketingService/SocialMediaPosts/{socialmediapostId} | Get social media post by ID |
| [**get_social_media_posts_count_async**](SocialMediaPostsApi.md#get_social_media_posts_count_async) | **GET** /api/v2/MarketingService/SocialMediaPosts/Count | Get social media posts count |
| [**get_social_media_posts_o_data_async**](SocialMediaPostsApi.md#get_social_media_posts_o_data_async) | **GET** /api/v2/MarketingService/SocialMediaPosts | Get social media posts |
| [**patch_social_media_post_async**](SocialMediaPostsApi.md#patch_social_media_post_async) | **PATCH** /api/v2/MarketingService/SocialMediaPosts/{socialmediapostId} | Patch a social media post |
| [**update_social_media_post_async**](SocialMediaPostsApi.md#update_social_media_post_async) | **PUT** /api/v2/MarketingService/SocialMediaPosts/{socialmediapostId} | Update a social media post |


## create_social_media_post_async

> <EmptyEnvelope> create_social_media_post_async(tenant_id, social_media_post_create_dto, opts)

Create a social media post

Creates a new social media post for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialMediaPostsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_media_post_create_dto = OpenapiClient::SocialMediaPostCreateDto.new # SocialMediaPostCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a social media post
  result = api_instance.create_social_media_post_async(tenant_id, social_media_post_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialMediaPostsApi->create_social_media_post_async: #{e}"
end
```

#### Using the create_social_media_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_social_media_post_async_with_http_info(tenant_id, social_media_post_create_dto, opts)

```ruby
begin
  # Create a social media post
  data, status_code, headers = api_instance.create_social_media_post_async_with_http_info(tenant_id, social_media_post_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialMediaPostsApi->create_social_media_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **social_media_post_create_dto** | [**SocialMediaPostCreateDto**](SocialMediaPostCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_social_media_post_async

> <EmptyEnvelope> delete_social_media_post_async(tenant_id, socialmediapost_id, opts)

Delete a social media post

Deletes a social media post by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialMediaPostsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
socialmediapost_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a social media post
  result = api_instance.delete_social_media_post_async(tenant_id, socialmediapost_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialMediaPostsApi->delete_social_media_post_async: #{e}"
end
```

#### Using the delete_social_media_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_social_media_post_async_with_http_info(tenant_id, socialmediapost_id, opts)

```ruby
begin
  # Delete a social media post
  data, status_code, headers = api_instance.delete_social_media_post_async_with_http_info(tenant_id, socialmediapost_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialMediaPostsApi->delete_social_media_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **socialmediapost_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_social_media_post_details_async

> <SocialMediaPostDtoEnvelope> get_social_media_post_details_async(tenant_id, socialmediapost_id, opts)

Get social media post by ID

Retrieves the details of a specific social media post by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialMediaPostsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
socialmediapost_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get social media post by ID
  result = api_instance.get_social_media_post_details_async(tenant_id, socialmediapost_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialMediaPostsApi->get_social_media_post_details_async: #{e}"
end
```

#### Using the get_social_media_post_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialMediaPostDtoEnvelope>, Integer, Hash)> get_social_media_post_details_async_with_http_info(tenant_id, socialmediapost_id, opts)

```ruby
begin
  # Get social media post by ID
  data, status_code, headers = api_instance.get_social_media_post_details_async_with_http_info(tenant_id, socialmediapost_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialMediaPostDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialMediaPostsApi->get_social_media_post_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **socialmediapost_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialMediaPostDtoEnvelope**](SocialMediaPostDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_social_media_posts_count_async

> <Int32Envelope> get_social_media_posts_count_async(tenant_id, opts)

Get social media posts count

Returns the count of social media posts for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialMediaPostsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_media_post_dto_collection_query_parameters: OpenapiClient::SocialMediaPostDtoCollectionQueryParameters.new # SocialMediaPostDtoCollectionQueryParameters | 
}

begin
  # Get social media posts count
  result = api_instance.get_social_media_posts_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialMediaPostsApi->get_social_media_posts_count_async: #{e}"
end
```

#### Using the get_social_media_posts_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_social_media_posts_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get social media posts count
  data, status_code, headers = api_instance.get_social_media_posts_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialMediaPostsApi->get_social_media_posts_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_media_post_dto_collection_query_parameters** | [**SocialMediaPostDtoCollectionQueryParameters**](SocialMediaPostDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_social_media_posts_o_data_async

> <SocialMediaPostDtoListEnvelope> get_social_media_posts_o_data_async(tenant_id, opts)

Get social media posts

Retrieves a collection of social media posts for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialMediaPostsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_media_post_dto_collection_query_parameters: OpenapiClient::SocialMediaPostDtoCollectionQueryParameters.new # SocialMediaPostDtoCollectionQueryParameters | 
}

begin
  # Get social media posts
  result = api_instance.get_social_media_posts_o_data_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialMediaPostsApi->get_social_media_posts_o_data_async: #{e}"
end
```

#### Using the get_social_media_posts_o_data_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialMediaPostDtoListEnvelope>, Integer, Hash)> get_social_media_posts_o_data_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get social media posts
  data, status_code, headers = api_instance.get_social_media_posts_o_data_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialMediaPostDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialMediaPostsApi->get_social_media_posts_o_data_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_media_post_dto_collection_query_parameters** | [**SocialMediaPostDtoCollectionQueryParameters**](SocialMediaPostDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**SocialMediaPostDtoListEnvelope**](SocialMediaPostDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_social_media_post_async

> <EmptyEnvelope> patch_social_media_post_async(tenant_id, socialmediapost_id, opts)

Patch a social media post

Partially updates a social media post by its ID using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialMediaPostsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
socialmediapost_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a social media post
  result = api_instance.patch_social_media_post_async(tenant_id, socialmediapost_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialMediaPostsApi->patch_social_media_post_async: #{e}"
end
```

#### Using the patch_social_media_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_social_media_post_async_with_http_info(tenant_id, socialmediapost_id, opts)

```ruby
begin
  # Patch a social media post
  data, status_code, headers = api_instance.patch_social_media_post_async_with_http_info(tenant_id, socialmediapost_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialMediaPostsApi->patch_social_media_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **socialmediapost_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_social_media_post_async

> <EmptyEnvelope> update_social_media_post_async(tenant_id, socialmediapost_id, social_media_post_update_dto, opts)

Update a social media post

Updates an existing social media post by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialMediaPostsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
socialmediapost_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_media_post_update_dto = OpenapiClient::SocialMediaPostUpdateDto.new # SocialMediaPostUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update a social media post
  result = api_instance.update_social_media_post_async(tenant_id, socialmediapost_id, social_media_post_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialMediaPostsApi->update_social_media_post_async: #{e}"
end
```

#### Using the update_social_media_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_social_media_post_async_with_http_info(tenant_id, socialmediapost_id, social_media_post_update_dto, opts)

```ruby
begin
  # Update a social media post
  data, status_code, headers = api_instance.update_social_media_post_async_with_http_info(tenant_id, socialmediapost_id, social_media_post_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialMediaPostsApi->update_social_media_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **socialmediapost_id** | **String** |  |  |
| **social_media_post_update_dto** | [**SocialMediaPostUpdateDto**](SocialMediaPostUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

